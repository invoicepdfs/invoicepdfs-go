# \DocumentsAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ArchiveDocumentApiV1DocumentsDocumentIdArchivePost**](DocumentsAPI.md#ArchiveDocumentApiV1DocumentsDocumentIdArchivePost) | **Post** /api/v1/documents/{document_id}/archive | Archive Document
[**CalculateDocumentApiV1DocumentsCalculatePost**](DocumentsAPI.md#CalculateDocumentApiV1DocumentsCalculatePost) | **Post** /api/v1/documents/calculate | Calculate Document
[**CreateDocumentApiV1DocumentsPost**](DocumentsAPI.md#CreateDocumentApiV1DocumentsPost) | **Post** /api/v1/documents | Create Document
[**DeleteDocumentApiV1DocumentsDocumentIdDelete**](DocumentsAPI.md#DeleteDocumentApiV1DocumentsDocumentIdDelete) | **Delete** /api/v1/documents/{document_id} | Delete Document
[**FinalizeDocumentApiV1DocumentsDocumentIdFinalizePost**](DocumentsAPI.md#FinalizeDocumentApiV1DocumentsDocumentIdFinalizePost) | **Post** /api/v1/documents/{document_id}/finalize | Finalize Document
[**GetDocumentApiV1DocumentsDocumentIdGet**](DocumentsAPI.md#GetDocumentApiV1DocumentsDocumentIdGet) | **Get** /api/v1/documents/{document_id} | Get Document
[**ListDocumentDeliveriesApiV1DocumentsDocumentIdDeliveriesGet**](DocumentsAPI.md#ListDocumentDeliveriesApiV1DocumentsDocumentIdDeliveriesGet) | **Get** /api/v1/documents/{document_id}/deliveries | List Document Deliveries
[**ListDocumentsApiV1DocumentsGet**](DocumentsAPI.md#ListDocumentsApiV1DocumentsGet) | **Get** /api/v1/documents | List Documents
[**MarkPaidApiV1DocumentsDocumentIdMarkPaidPost**](DocumentsAPI.md#MarkPaidApiV1DocumentsDocumentIdMarkPaidPost) | **Post** /api/v1/documents/{document_id}/mark-paid | Mark Paid
[**MarkSentApiV1DocumentsDocumentIdMarkSentPost**](DocumentsAPI.md#MarkSentApiV1DocumentsDocumentIdMarkSentPost) | **Post** /api/v1/documents/{document_id}/mark-sent | Mark Sent
[**MarkUnpaidApiV1DocumentsDocumentIdMarkUnpaidPost**](DocumentsAPI.md#MarkUnpaidApiV1DocumentsDocumentIdMarkUnpaidPost) | **Post** /api/v1/documents/{document_id}/mark-unpaid | Mark Unpaid
[**PatchDocumentApiV1DocumentsDocumentIdPatch**](DocumentsAPI.md#PatchDocumentApiV1DocumentsDocumentIdPatch) | **Patch** /api/v1/documents/{document_id} | Patch Document
[**RenderDocumentApiV1DocumentsDocumentIdRendersPost**](DocumentsAPI.md#RenderDocumentApiV1DocumentsDocumentIdRendersPost) | **Post** /api/v1/documents/{document_id}/renders | Render Document
[**RenderDocumentApiV1DocumentsRenderPost**](DocumentsAPI.md#RenderDocumentApiV1DocumentsRenderPost) | **Post** /api/v1/documents/render | Render Document
[**RestoreDocumentApiV1DocumentsDocumentIdRestorePost**](DocumentsAPI.md#RestoreDocumentApiV1DocumentsDocumentIdRestorePost) | **Post** /api/v1/documents/{document_id}/restore | Restore Document
[**SendDocumentApiV1DocumentsDocumentIdSendPost**](DocumentsAPI.md#SendDocumentApiV1DocumentsDocumentIdSendPost) | **Post** /api/v1/documents/{document_id}/send | Send Document
[**ValidateDocumentApiV1DocumentsValidatePost**](DocumentsAPI.md#ValidateDocumentApiV1DocumentsValidatePost) | **Post** /api/v1/documents/validate | Validate Document
[**VoidDocumentApiV1DocumentsDocumentIdVoidPost**](DocumentsAPI.md#VoidDocumentApiV1DocumentsDocumentIdVoidPost) | **Post** /api/v1/documents/{document_id}/void | Void Document



## ArchiveDocumentApiV1DocumentsDocumentIdArchivePost

> DocumentResponse ArchiveDocumentApiV1DocumentsDocumentIdArchivePost(ctx, documentId).Execute()

Archive Document

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/invoicepdfs/invoicepdfs-go"
)

func main() {
	documentId := "documentId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.ArchiveDocumentApiV1DocumentsDocumentIdArchivePost(context.Background(), documentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.ArchiveDocumentApiV1DocumentsDocumentIdArchivePost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ArchiveDocumentApiV1DocumentsDocumentIdArchivePost`: DocumentResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.ArchiveDocumentApiV1DocumentsDocumentIdArchivePost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**documentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiArchiveDocumentApiV1DocumentsDocumentIdArchivePostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**DocumentResponse**](DocumentResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CalculateDocumentApiV1DocumentsCalculatePost

> DocumentCalculateResponse CalculateDocumentApiV1DocumentsCalculatePost(ctx).DocumentCalculateRequest(documentCalculateRequest).Execute()

Calculate Document

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/invoicepdfs/invoicepdfs-go"
)

func main() {
	documentCalculateRequest := *openapiclient.NewDocumentCalculateRequest(*openapiclient.NewDocumentInvoiceDataInput("INV-2026-001", time.Now(), "USD", *openapiclient.NewDocumentPartyInput("Acme Corp"), *openapiclient.NewDocumentPartyInput("Acme Corp"), []openapiclient.DocumentLineItemInput{*openapiclient.NewDocumentLineItemInput("Web Development", "2", "150.00")})) // DocumentCalculateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.CalculateDocumentApiV1DocumentsCalculatePost(context.Background()).DocumentCalculateRequest(documentCalculateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.CalculateDocumentApiV1DocumentsCalculatePost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CalculateDocumentApiV1DocumentsCalculatePost`: DocumentCalculateResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.CalculateDocumentApiV1DocumentsCalculatePost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCalculateDocumentApiV1DocumentsCalculatePostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **documentCalculateRequest** | [**DocumentCalculateRequest**](DocumentCalculateRequest.md) |  | 

### Return type

[**DocumentCalculateResponse**](DocumentCalculateResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateDocumentApiV1DocumentsPost

> DocumentResponse CreateDocumentApiV1DocumentsPost(ctx).DocumentCreateRequest(documentCreateRequest).IdempotencyKey(idempotencyKey).Execute()

Create Document

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/invoicepdfs/invoicepdfs-go"
)

func main() {
	documentCreateRequest := *openapiclient.NewDocumentCreateRequest("INV-2026-001", time.Now(), "USD", "bp_01ABC", "cus_01XYZ", []openapiclient.StandardLineItemInput{*openapiclient.NewStandardLineItemInput("Web Development", "2")}) // DocumentCreateRequest | 
	idempotencyKey := "idempotencyKey_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.CreateDocumentApiV1DocumentsPost(context.Background()).DocumentCreateRequest(documentCreateRequest).IdempotencyKey(idempotencyKey).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.CreateDocumentApiV1DocumentsPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateDocumentApiV1DocumentsPost`: DocumentResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.CreateDocumentApiV1DocumentsPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateDocumentApiV1DocumentsPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **documentCreateRequest** | [**DocumentCreateRequest**](DocumentCreateRequest.md) |  | 
 **idempotencyKey** | **string** |  | 

### Return type

[**DocumentResponse**](DocumentResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteDocumentApiV1DocumentsDocumentIdDelete

> SimpleBoolResponse DeleteDocumentApiV1DocumentsDocumentIdDelete(ctx, documentId).Execute()

Delete Document

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/invoicepdfs/invoicepdfs-go"
)

func main() {
	documentId := "documentId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.DeleteDocumentApiV1DocumentsDocumentIdDelete(context.Background(), documentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.DeleteDocumentApiV1DocumentsDocumentIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteDocumentApiV1DocumentsDocumentIdDelete`: SimpleBoolResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.DeleteDocumentApiV1DocumentsDocumentIdDelete`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**documentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteDocumentApiV1DocumentsDocumentIdDeleteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**SimpleBoolResponse**](SimpleBoolResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## FinalizeDocumentApiV1DocumentsDocumentIdFinalizePost

> DocumentResponse FinalizeDocumentApiV1DocumentsDocumentIdFinalizePost(ctx, documentId).Execute()

Finalize Document

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/invoicepdfs/invoicepdfs-go"
)

func main() {
	documentId := "documentId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.FinalizeDocumentApiV1DocumentsDocumentIdFinalizePost(context.Background(), documentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.FinalizeDocumentApiV1DocumentsDocumentIdFinalizePost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FinalizeDocumentApiV1DocumentsDocumentIdFinalizePost`: DocumentResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.FinalizeDocumentApiV1DocumentsDocumentIdFinalizePost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**documentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiFinalizeDocumentApiV1DocumentsDocumentIdFinalizePostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**DocumentResponse**](DocumentResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetDocumentApiV1DocumentsDocumentIdGet

> DocumentResponse GetDocumentApiV1DocumentsDocumentIdGet(ctx, documentId).Execute()

Get Document

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/invoicepdfs/invoicepdfs-go"
)

func main() {
	documentId := "documentId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.GetDocumentApiV1DocumentsDocumentIdGet(context.Background(), documentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.GetDocumentApiV1DocumentsDocumentIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetDocumentApiV1DocumentsDocumentIdGet`: DocumentResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.GetDocumentApiV1DocumentsDocumentIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**documentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetDocumentApiV1DocumentsDocumentIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**DocumentResponse**](DocumentResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListDocumentDeliveriesApiV1DocumentsDocumentIdDeliveriesGet

> DeliveriesListResponse ListDocumentDeliveriesApiV1DocumentsDocumentIdDeliveriesGet(ctx, documentId).Limit(limit).Cursor(cursor).Execute()

List Document Deliveries

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/invoicepdfs/invoicepdfs-go"
)

func main() {
	documentId := "documentId_example" // string | 
	limit := int32(56) // int32 |  (optional) (default to 50)
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.ListDocumentDeliveriesApiV1DocumentsDocumentIdDeliveriesGet(context.Background(), documentId).Limit(limit).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.ListDocumentDeliveriesApiV1DocumentsDocumentIdDeliveriesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListDocumentDeliveriesApiV1DocumentsDocumentIdDeliveriesGet`: DeliveriesListResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.ListDocumentDeliveriesApiV1DocumentsDocumentIdDeliveriesGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**documentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListDocumentDeliveriesApiV1DocumentsDocumentIdDeliveriesGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **limit** | **int32** |  | [default to 50]
 **cursor** | **string** |  | 

### Return type

[**DeliveriesListResponse**](DeliveriesListResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListDocumentsApiV1DocumentsGet

> DocumentsListResponse ListDocumentsApiV1DocumentsGet(ctx).Limit(limit).Cursor(cursor).DocumentType(documentType).Status(status).Execute()

List Documents

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/invoicepdfs/invoicepdfs-go"
)

func main() {
	limit := int32(56) // int32 |  (optional) (default to 50)
	cursor := "cursor_example" // string |  (optional)
	documentType := "documentType_example" // string |  (optional)
	status := "status_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.ListDocumentsApiV1DocumentsGet(context.Background()).Limit(limit).Cursor(cursor).DocumentType(documentType).Status(status).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.ListDocumentsApiV1DocumentsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListDocumentsApiV1DocumentsGet`: DocumentsListResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.ListDocumentsApiV1DocumentsGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListDocumentsApiV1DocumentsGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int32** |  | [default to 50]
 **cursor** | **string** |  | 
 **documentType** | **string** |  | 
 **status** | **string** |  | 

### Return type

[**DocumentsListResponse**](DocumentsListResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MarkPaidApiV1DocumentsDocumentIdMarkPaidPost

> DocumentResponse MarkPaidApiV1DocumentsDocumentIdMarkPaidPost(ctx, documentId).Execute()

Mark Paid

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/invoicepdfs/invoicepdfs-go"
)

func main() {
	documentId := "documentId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.MarkPaidApiV1DocumentsDocumentIdMarkPaidPost(context.Background(), documentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.MarkPaidApiV1DocumentsDocumentIdMarkPaidPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MarkPaidApiV1DocumentsDocumentIdMarkPaidPost`: DocumentResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.MarkPaidApiV1DocumentsDocumentIdMarkPaidPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**documentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiMarkPaidApiV1DocumentsDocumentIdMarkPaidPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**DocumentResponse**](DocumentResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MarkSentApiV1DocumentsDocumentIdMarkSentPost

> DocumentResponse MarkSentApiV1DocumentsDocumentIdMarkSentPost(ctx, documentId).Execute()

Mark Sent

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/invoicepdfs/invoicepdfs-go"
)

func main() {
	documentId := "documentId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.MarkSentApiV1DocumentsDocumentIdMarkSentPost(context.Background(), documentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.MarkSentApiV1DocumentsDocumentIdMarkSentPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MarkSentApiV1DocumentsDocumentIdMarkSentPost`: DocumentResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.MarkSentApiV1DocumentsDocumentIdMarkSentPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**documentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiMarkSentApiV1DocumentsDocumentIdMarkSentPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**DocumentResponse**](DocumentResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MarkUnpaidApiV1DocumentsDocumentIdMarkUnpaidPost

> DocumentResponse MarkUnpaidApiV1DocumentsDocumentIdMarkUnpaidPost(ctx, documentId).Execute()

Mark Unpaid

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/invoicepdfs/invoicepdfs-go"
)

func main() {
	documentId := "documentId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.MarkUnpaidApiV1DocumentsDocumentIdMarkUnpaidPost(context.Background(), documentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.MarkUnpaidApiV1DocumentsDocumentIdMarkUnpaidPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MarkUnpaidApiV1DocumentsDocumentIdMarkUnpaidPost`: DocumentResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.MarkUnpaidApiV1DocumentsDocumentIdMarkUnpaidPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**documentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiMarkUnpaidApiV1DocumentsDocumentIdMarkUnpaidPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**DocumentResponse**](DocumentResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PatchDocumentApiV1DocumentsDocumentIdPatch

> DocumentResponse PatchDocumentApiV1DocumentsDocumentIdPatch(ctx, documentId).DocumentPatchRequest(documentPatchRequest).Execute()

Patch Document

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/invoicepdfs/invoicepdfs-go"
)

func main() {
	documentId := "documentId_example" // string | 
	documentPatchRequest := *openapiclient.NewDocumentPatchRequest() // DocumentPatchRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.PatchDocumentApiV1DocumentsDocumentIdPatch(context.Background(), documentId).DocumentPatchRequest(documentPatchRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.PatchDocumentApiV1DocumentsDocumentIdPatch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PatchDocumentApiV1DocumentsDocumentIdPatch`: DocumentResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.PatchDocumentApiV1DocumentsDocumentIdPatch`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**documentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiPatchDocumentApiV1DocumentsDocumentIdPatchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **documentPatchRequest** | [**DocumentPatchRequest**](DocumentPatchRequest.md) |  | 

### Return type

[**DocumentResponse**](DocumentResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RenderDocumentApiV1DocumentsDocumentIdRendersPost

> interface{} RenderDocumentApiV1DocumentsDocumentIdRendersPost(ctx, documentId).AppDocumentsSchemasDocumentRenderRequest(appDocumentsSchemasDocumentRenderRequest).IdempotencyKey(idempotencyKey).Execute()

Render Document

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/invoicepdfs/invoicepdfs-go"
)

func main() {
	documentId := "documentId_example" // string | 
	appDocumentsSchemasDocumentRenderRequest := *openapiclient.NewAppDocumentsSchemasDocumentRenderRequest() // AppDocumentsSchemasDocumentRenderRequest | 
	idempotencyKey := "idempotencyKey_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.RenderDocumentApiV1DocumentsDocumentIdRendersPost(context.Background(), documentId).AppDocumentsSchemasDocumentRenderRequest(appDocumentsSchemasDocumentRenderRequest).IdempotencyKey(idempotencyKey).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.RenderDocumentApiV1DocumentsDocumentIdRendersPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RenderDocumentApiV1DocumentsDocumentIdRendersPost`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.RenderDocumentApiV1DocumentsDocumentIdRendersPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**documentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRenderDocumentApiV1DocumentsDocumentIdRendersPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **appDocumentsSchemasDocumentRenderRequest** | [**AppDocumentsSchemasDocumentRenderRequest**](AppDocumentsSchemasDocumentRenderRequest.md) |  | 
 **idempotencyKey** | **string** |  | 

### Return type

**interface{}**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RenderDocumentApiV1DocumentsRenderPost

> interface{} RenderDocumentApiV1DocumentsRenderPost(ctx).AppSchemasV1DocumentRenderRequest(appSchemasV1DocumentRenderRequest).IdempotencyKey(idempotencyKey).Execute()

Render Document

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/invoicepdfs/invoicepdfs-go"
)

func main() {
	appSchemasV1DocumentRenderRequest := *openapiclient.NewAppSchemasV1DocumentRenderRequest(*openapiclient.NewDocumentInvoiceDataInput("INV-2026-001", time.Now(), "USD", *openapiclient.NewDocumentPartyInput("Acme Corp"), *openapiclient.NewDocumentPartyInput("Acme Corp"), []openapiclient.DocumentLineItemInput{*openapiclient.NewDocumentLineItemInput("Web Development", "2", "150.00")}), *openapiclient.NewDocumentTemplateRef("Id_example")) // AppSchemasV1DocumentRenderRequest | 
	idempotencyKey := "idempotencyKey_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.RenderDocumentApiV1DocumentsRenderPost(context.Background()).AppSchemasV1DocumentRenderRequest(appSchemasV1DocumentRenderRequest).IdempotencyKey(idempotencyKey).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.RenderDocumentApiV1DocumentsRenderPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RenderDocumentApiV1DocumentsRenderPost`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.RenderDocumentApiV1DocumentsRenderPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRenderDocumentApiV1DocumentsRenderPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **appSchemasV1DocumentRenderRequest** | [**AppSchemasV1DocumentRenderRequest**](AppSchemasV1DocumentRenderRequest.md) |  | 
 **idempotencyKey** | **string** |  | 

### Return type

**interface{}**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RestoreDocumentApiV1DocumentsDocumentIdRestorePost

> DocumentResponse RestoreDocumentApiV1DocumentsDocumentIdRestorePost(ctx, documentId).Execute()

Restore Document

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/invoicepdfs/invoicepdfs-go"
)

func main() {
	documentId := "documentId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.RestoreDocumentApiV1DocumentsDocumentIdRestorePost(context.Background(), documentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.RestoreDocumentApiV1DocumentsDocumentIdRestorePost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RestoreDocumentApiV1DocumentsDocumentIdRestorePost`: DocumentResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.RestoreDocumentApiV1DocumentsDocumentIdRestorePost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**documentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRestoreDocumentApiV1DocumentsDocumentIdRestorePostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**DocumentResponse**](DocumentResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SendDocumentApiV1DocumentsDocumentIdSendPost

> DeliveryResponse SendDocumentApiV1DocumentsDocumentIdSendPost(ctx, documentId).DeliverySendRequest(deliverySendRequest).Execute()

Send Document

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/invoicepdfs/invoicepdfs-go"
)

func main() {
	documentId := "documentId_example" // string | 
	deliverySendRequest := *openapiclient.NewDeliverySendRequest([]string{"To_example"}) // DeliverySendRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.SendDocumentApiV1DocumentsDocumentIdSendPost(context.Background(), documentId).DeliverySendRequest(deliverySendRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.SendDocumentApiV1DocumentsDocumentIdSendPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SendDocumentApiV1DocumentsDocumentIdSendPost`: DeliveryResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.SendDocumentApiV1DocumentsDocumentIdSendPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**documentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiSendDocumentApiV1DocumentsDocumentIdSendPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **deliverySendRequest** | [**DeliverySendRequest**](DeliverySendRequest.md) |  | 

### Return type

[**DeliveryResponse**](DeliveryResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ValidateDocumentApiV1DocumentsValidatePost

> DocumentValidateResponse ValidateDocumentApiV1DocumentsValidatePost(ctx).DocumentValidateRequest(documentValidateRequest).Execute()

Validate Document

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/invoicepdfs/invoicepdfs-go"
)

func main() {
	documentValidateRequest := *openapiclient.NewDocumentValidateRequest(*openapiclient.NewDocumentInvoiceDataInput("INV-2026-001", time.Now(), "USD", *openapiclient.NewDocumentPartyInput("Acme Corp"), *openapiclient.NewDocumentPartyInput("Acme Corp"), []openapiclient.DocumentLineItemInput{*openapiclient.NewDocumentLineItemInput("Web Development", "2", "150.00")})) // DocumentValidateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.ValidateDocumentApiV1DocumentsValidatePost(context.Background()).DocumentValidateRequest(documentValidateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.ValidateDocumentApiV1DocumentsValidatePost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ValidateDocumentApiV1DocumentsValidatePost`: DocumentValidateResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.ValidateDocumentApiV1DocumentsValidatePost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiValidateDocumentApiV1DocumentsValidatePostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **documentValidateRequest** | [**DocumentValidateRequest**](DocumentValidateRequest.md) |  | 

### Return type

[**DocumentValidateResponse**](DocumentValidateResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## VoidDocumentApiV1DocumentsDocumentIdVoidPost

> DocumentResponse VoidDocumentApiV1DocumentsDocumentIdVoidPost(ctx, documentId).Execute()

Void Document

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/invoicepdfs/invoicepdfs-go"
)

func main() {
	documentId := "documentId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.VoidDocumentApiV1DocumentsDocumentIdVoidPost(context.Background(), documentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.VoidDocumentApiV1DocumentsDocumentIdVoidPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `VoidDocumentApiV1DocumentsDocumentIdVoidPost`: DocumentResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.VoidDocumentApiV1DocumentsDocumentIdVoidPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**documentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiVoidDocumentApiV1DocumentsDocumentIdVoidPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**DocumentResponse**](DocumentResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

