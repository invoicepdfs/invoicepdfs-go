# \DocumentsAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ArchiveDocument**](DocumentsAPI.md#ArchiveDocument) | **Post** /api/v1/documents/{document_id}/archive | Archive Document
[**CalculateDocument**](DocumentsAPI.md#CalculateDocument) | **Post** /api/v1/documents/calculate | Calculate Document
[**CreateDocument**](DocumentsAPI.md#CreateDocument) | **Post** /api/v1/documents | Create Document
[**CreateDocumentRender**](DocumentsAPI.md#CreateDocumentRender) | **Post** /api/v1/documents/{document_id}/renders | Create Document Render
[**DeleteDocument**](DocumentsAPI.md#DeleteDocument) | **Delete** /api/v1/documents/{document_id} | Delete Document
[**DuplicateDocument**](DocumentsAPI.md#DuplicateDocument) | **Post** /api/v1/documents/{document_id}/duplicate | Duplicate Document
[**FinalizeDocument**](DocumentsAPI.md#FinalizeDocument) | **Post** /api/v1/documents/{document_id}/finalize | Finalize Document
[**GetDocument**](DocumentsAPI.md#GetDocument) | **Get** /api/v1/documents/{document_id} | Get Document
[**ListDocumentDeliveries**](DocumentsAPI.md#ListDocumentDeliveries) | **Get** /api/v1/documents/{document_id}/deliveries | List Document Deliveries
[**ListDocuments**](DocumentsAPI.md#ListDocuments) | **Get** /api/v1/documents | List Documents
[**MarkPaid**](DocumentsAPI.md#MarkPaid) | **Post** /api/v1/documents/{document_id}/mark-paid | Mark Paid
[**MarkSent**](DocumentsAPI.md#MarkSent) | **Post** /api/v1/documents/{document_id}/mark-sent | Mark Sent
[**MarkUnpaid**](DocumentsAPI.md#MarkUnpaid) | **Post** /api/v1/documents/{document_id}/mark-unpaid | Mark Unpaid
[**RenderDocument**](DocumentsAPI.md#RenderDocument) | **Post** /api/v1/documents/render | Render Document
[**RestoreDocument**](DocumentsAPI.md#RestoreDocument) | **Post** /api/v1/documents/{document_id}/restore | Restore Document
[**SendDocument**](DocumentsAPI.md#SendDocument) | **Post** /api/v1/documents/{document_id}/send | Send Document
[**UpdateDocument**](DocumentsAPI.md#UpdateDocument) | **Patch** /api/v1/documents/{document_id} | Update Document
[**ValidateDocument**](DocumentsAPI.md#ValidateDocument) | **Post** /api/v1/documents/validate | Validate Document
[**VoidDocument**](DocumentsAPI.md#VoidDocument) | **Post** /api/v1/documents/{document_id}/void | Void Document



## ArchiveDocument

> DocumentResponse ArchiveDocument(ctx, documentId).Execute()

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
	resp, r, err := apiClient.DocumentsAPI.ArchiveDocument(context.Background(), documentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.ArchiveDocument``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ArchiveDocument`: DocumentResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.ArchiveDocument`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**documentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiArchiveDocumentRequest struct via the builder pattern


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


## CalculateDocument

> DocumentCalculateResponse CalculateDocument(ctx).DocumentCalculateRequest(documentCalculateRequest).Execute()

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
	resp, r, err := apiClient.DocumentsAPI.CalculateDocument(context.Background()).DocumentCalculateRequest(documentCalculateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.CalculateDocument``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CalculateDocument`: DocumentCalculateResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.CalculateDocument`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCalculateDocumentRequest struct via the builder pattern


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


## CreateDocument

> DocumentResponse CreateDocument(ctx).DocumentCreateRequest(documentCreateRequest).IdempotencyKey(idempotencyKey).Execute()

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
	resp, r, err := apiClient.DocumentsAPI.CreateDocument(context.Background()).DocumentCreateRequest(documentCreateRequest).IdempotencyKey(idempotencyKey).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.CreateDocument``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateDocument`: DocumentResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.CreateDocument`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateDocumentRequest struct via the builder pattern


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


## CreateDocumentRender

> interface{} CreateDocumentRender(ctx, documentId).DocumentRenderOptions(documentRenderOptions).IdempotencyKey(idempotencyKey).Execute()

Create Document Render

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
	documentRenderOptions := *openapiclient.NewDocumentRenderOptions() // DocumentRenderOptions | 
	idempotencyKey := "idempotencyKey_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.CreateDocumentRender(context.Background(), documentId).DocumentRenderOptions(documentRenderOptions).IdempotencyKey(idempotencyKey).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.CreateDocumentRender``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateDocumentRender`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.CreateDocumentRender`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**documentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateDocumentRenderRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **documentRenderOptions** | [**DocumentRenderOptions**](DocumentRenderOptions.md) |  | 
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


## DeleteDocument

> SimpleBoolResponse DeleteDocument(ctx, documentId).Execute()

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
	resp, r, err := apiClient.DocumentsAPI.DeleteDocument(context.Background(), documentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.DeleteDocument``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteDocument`: SimpleBoolResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.DeleteDocument`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**documentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteDocumentRequest struct via the builder pattern


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


## DuplicateDocument

> DocumentResponse DuplicateDocument(ctx, documentId).Execute()

Duplicate Document

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
	resp, r, err := apiClient.DocumentsAPI.DuplicateDocument(context.Background(), documentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.DuplicateDocument``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DuplicateDocument`: DocumentResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.DuplicateDocument`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**documentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDuplicateDocumentRequest struct via the builder pattern


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


## FinalizeDocument

> DocumentResponse FinalizeDocument(ctx, documentId).Execute()

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
	resp, r, err := apiClient.DocumentsAPI.FinalizeDocument(context.Background(), documentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.FinalizeDocument``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FinalizeDocument`: DocumentResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.FinalizeDocument`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**documentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiFinalizeDocumentRequest struct via the builder pattern


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


## GetDocument

> DocumentResponse GetDocument(ctx, documentId).Execute()

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
	resp, r, err := apiClient.DocumentsAPI.GetDocument(context.Background(), documentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.GetDocument``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetDocument`: DocumentResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.GetDocument`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**documentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetDocumentRequest struct via the builder pattern


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


## ListDocumentDeliveries

> DeliveriesListResponse ListDocumentDeliveries(ctx, documentId).Limit(limit).Cursor(cursor).Execute()

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
	resp, r, err := apiClient.DocumentsAPI.ListDocumentDeliveries(context.Background(), documentId).Limit(limit).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.ListDocumentDeliveries``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListDocumentDeliveries`: DeliveriesListResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.ListDocumentDeliveries`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**documentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListDocumentDeliveriesRequest struct via the builder pattern


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


## ListDocuments

> DocumentsListResponse ListDocuments(ctx).Limit(limit).Cursor(cursor).DocumentType(documentType).Status(status).Execute()

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
	resp, r, err := apiClient.DocumentsAPI.ListDocuments(context.Background()).Limit(limit).Cursor(cursor).DocumentType(documentType).Status(status).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.ListDocuments``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListDocuments`: DocumentsListResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.ListDocuments`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListDocumentsRequest struct via the builder pattern


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


## MarkPaid

> DocumentResponse MarkPaid(ctx, documentId).Execute()

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
	resp, r, err := apiClient.DocumentsAPI.MarkPaid(context.Background(), documentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.MarkPaid``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MarkPaid`: DocumentResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.MarkPaid`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**documentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiMarkPaidRequest struct via the builder pattern


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


## MarkSent

> DocumentResponse MarkSent(ctx, documentId).Execute()

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
	resp, r, err := apiClient.DocumentsAPI.MarkSent(context.Background(), documentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.MarkSent``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MarkSent`: DocumentResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.MarkSent`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**documentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiMarkSentRequest struct via the builder pattern


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


## MarkUnpaid

> DocumentResponse MarkUnpaid(ctx, documentId).Execute()

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
	resp, r, err := apiClient.DocumentsAPI.MarkUnpaid(context.Background(), documentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.MarkUnpaid``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MarkUnpaid`: DocumentResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.MarkUnpaid`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**documentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiMarkUnpaidRequest struct via the builder pattern


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


## RenderDocument

> interface{} RenderDocument(ctx).DocumentRenderRequest(documentRenderRequest).IdempotencyKey(idempotencyKey).Execute()

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
	documentRenderRequest := *openapiclient.NewDocumentRenderRequest(*openapiclient.NewDocumentInvoiceDataInput("INV-2026-001", time.Now(), "USD", *openapiclient.NewDocumentPartyInput("Acme Corp"), *openapiclient.NewDocumentPartyInput("Acme Corp"), []openapiclient.DocumentLineItemInput{*openapiclient.NewDocumentLineItemInput("Web Development", "2", "150.00")}), *openapiclient.NewDocumentTemplateRef("Id_example")) // DocumentRenderRequest | 
	idempotencyKey := "idempotencyKey_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.RenderDocument(context.Background()).DocumentRenderRequest(documentRenderRequest).IdempotencyKey(idempotencyKey).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.RenderDocument``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RenderDocument`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.RenderDocument`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRenderDocumentRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **documentRenderRequest** | [**DocumentRenderRequest**](DocumentRenderRequest.md) |  | 
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


## RestoreDocument

> DocumentResponse RestoreDocument(ctx, documentId).Execute()

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
	resp, r, err := apiClient.DocumentsAPI.RestoreDocument(context.Background(), documentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.RestoreDocument``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RestoreDocument`: DocumentResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.RestoreDocument`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**documentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRestoreDocumentRequest struct via the builder pattern


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


## SendDocument

> DeliveryResponse SendDocument(ctx, documentId).DeliverySendRequest(deliverySendRequest).Execute()

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
	resp, r, err := apiClient.DocumentsAPI.SendDocument(context.Background(), documentId).DeliverySendRequest(deliverySendRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.SendDocument``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SendDocument`: DeliveryResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.SendDocument`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**documentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiSendDocumentRequest struct via the builder pattern


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


## UpdateDocument

> DocumentResponse UpdateDocument(ctx, documentId).DocumentPatchRequest(documentPatchRequest).Execute()

Update Document

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
	resp, r, err := apiClient.DocumentsAPI.UpdateDocument(context.Background(), documentId).DocumentPatchRequest(documentPatchRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.UpdateDocument``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateDocument`: DocumentResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.UpdateDocument`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**documentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateDocumentRequest struct via the builder pattern


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


## ValidateDocument

> DocumentValidateResponse ValidateDocument(ctx).DocumentValidateRequest(documentValidateRequest).Execute()

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
	resp, r, err := apiClient.DocumentsAPI.ValidateDocument(context.Background()).DocumentValidateRequest(documentValidateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.ValidateDocument``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ValidateDocument`: DocumentValidateResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.ValidateDocument`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiValidateDocumentRequest struct via the builder pattern


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


## VoidDocument

> DocumentResponse VoidDocument(ctx, documentId).Execute()

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
	resp, r, err := apiClient.DocumentsAPI.VoidDocument(context.Background(), documentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.VoidDocument``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `VoidDocument`: DocumentResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.VoidDocument`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**documentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiVoidDocumentRequest struct via the builder pattern


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

