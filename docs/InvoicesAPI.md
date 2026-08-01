# \InvoicesAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ArchiveInvoiceApiV1InvoicesInvoiceIdArchivePost**](InvoicesAPI.md#ArchiveInvoiceApiV1InvoicesInvoiceIdArchivePost) | **Post** /api/v1/invoices/{invoice_id}/archive | Archive Invoice
[**CalculateInvoiceApiV1InvoicesCalculatePost**](InvoicesAPI.md#CalculateInvoiceApiV1InvoicesCalculatePost) | **Post** /api/v1/invoices/calculate | Calculate Invoice
[**CreateInvoiceApiV1InvoicesPost**](InvoicesAPI.md#CreateInvoiceApiV1InvoicesPost) | **Post** /api/v1/invoices | Create Invoice
[**DeleteInvoiceApiV1InvoicesInvoiceIdDelete**](InvoicesAPI.md#DeleteInvoiceApiV1InvoicesInvoiceIdDelete) | **Delete** /api/v1/invoices/{invoice_id} | Delete Invoice
[**DuplicateInvoiceApiV1InvoicesInvoiceIdDuplicatePost**](InvoicesAPI.md#DuplicateInvoiceApiV1InvoicesInvoiceIdDuplicatePost) | **Post** /api/v1/invoices/{invoice_id}/duplicate | Duplicate Invoice
[**FinalizeInvoiceApiV1InvoicesInvoiceIdFinalizePost**](InvoicesAPI.md#FinalizeInvoiceApiV1InvoicesInvoiceIdFinalizePost) | **Post** /api/v1/invoices/{invoice_id}/finalize | Finalize Invoice
[**GetInvoiceApiV1InvoicesInvoiceIdGet**](InvoicesAPI.md#GetInvoiceApiV1InvoicesInvoiceIdGet) | **Get** /api/v1/invoices/{invoice_id} | Get Invoice
[**ListInvoiceDeliveriesApiV1InvoicesInvoiceIdDeliveriesGet**](InvoicesAPI.md#ListInvoiceDeliveriesApiV1InvoicesInvoiceIdDeliveriesGet) | **Get** /api/v1/invoices/{invoice_id}/deliveries | List Invoice Deliveries
[**ListInvoicesApiV1InvoicesGet**](InvoicesAPI.md#ListInvoicesApiV1InvoicesGet) | **Get** /api/v1/invoices | List Invoices
[**MarkPaidApiV1InvoicesInvoiceIdMarkPaidPost**](InvoicesAPI.md#MarkPaidApiV1InvoicesInvoiceIdMarkPaidPost) | **Post** /api/v1/invoices/{invoice_id}/mark-paid | Mark Paid
[**MarkSentApiV1InvoicesInvoiceIdMarkSentPost**](InvoicesAPI.md#MarkSentApiV1InvoicesInvoiceIdMarkSentPost) | **Post** /api/v1/invoices/{invoice_id}/mark-sent | Mark Sent
[**MarkUnpaidApiV1InvoicesInvoiceIdMarkUnpaidPost**](InvoicesAPI.md#MarkUnpaidApiV1InvoicesInvoiceIdMarkUnpaidPost) | **Post** /api/v1/invoices/{invoice_id}/mark-unpaid | Mark Unpaid
[**PatchInvoiceApiV1InvoicesInvoiceIdPatch**](InvoicesAPI.md#PatchInvoiceApiV1InvoicesInvoiceIdPatch) | **Patch** /api/v1/invoices/{invoice_id} | Patch Invoice
[**PreviewInvoiceApiV1InvoicesPreviewPost**](InvoicesAPI.md#PreviewInvoiceApiV1InvoicesPreviewPost) | **Post** /api/v1/invoices/preview | Preview Invoice
[**RenderInvoiceApiV1InvoicesInvoiceIdRendersPost**](InvoicesAPI.md#RenderInvoiceApiV1InvoicesInvoiceIdRendersPost) | **Post** /api/v1/invoices/{invoice_id}/renders | Render Invoice
[**ReplaceInvoiceApiV1InvoicesInvoiceIdPut**](InvoicesAPI.md#ReplaceInvoiceApiV1InvoicesInvoiceIdPut) | **Put** /api/v1/invoices/{invoice_id} | Replace Invoice
[**RestoreInvoiceApiV1InvoicesInvoiceIdRestorePost**](InvoicesAPI.md#RestoreInvoiceApiV1InvoicesInvoiceIdRestorePost) | **Post** /api/v1/invoices/{invoice_id}/restore | Restore Invoice
[**SendInvoiceApiV1InvoicesInvoiceIdSendPost**](InvoicesAPI.md#SendInvoiceApiV1InvoicesInvoiceIdSendPost) | **Post** /api/v1/invoices/{invoice_id}/send | Send Invoice
[**ValidateInvoiceApiV1InvoicesValidatePost**](InvoicesAPI.md#ValidateInvoiceApiV1InvoicesValidatePost) | **Post** /api/v1/invoices/validate | Validate Invoice
[**VoidInvoiceApiV1InvoicesInvoiceIdVoidPost**](InvoicesAPI.md#VoidInvoiceApiV1InvoicesInvoiceIdVoidPost) | **Post** /api/v1/invoices/{invoice_id}/void | Void Invoice



## ArchiveInvoiceApiV1InvoicesInvoiceIdArchivePost

> InvoiceResponse ArchiveInvoiceApiV1InvoicesInvoiceIdArchivePost(ctx, invoiceId).Execute()

Archive Invoice

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	invoiceId := "invoiceId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InvoicesAPI.ArchiveInvoiceApiV1InvoicesInvoiceIdArchivePost(context.Background(), invoiceId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InvoicesAPI.ArchiveInvoiceApiV1InvoicesInvoiceIdArchivePost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ArchiveInvoiceApiV1InvoicesInvoiceIdArchivePost`: InvoiceResponse
	fmt.Fprintf(os.Stdout, "Response from `InvoicesAPI.ArchiveInvoiceApiV1InvoicesInvoiceIdArchivePost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**invoiceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiArchiveInvoiceApiV1InvoicesInvoiceIdArchivePostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**InvoiceResponse**](InvoiceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CalculateInvoiceApiV1InvoicesCalculatePost

> map[string]interface{} CalculateInvoiceApiV1InvoicesCalculatePost(ctx).InvoiceDraftRequest(invoiceDraftRequest).Execute()

Calculate Invoice

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	invoiceDraftRequest := *openapiclient.NewInvoiceDraftRequest("INV-2026-001", time.Now(), "USD", "bp_01ABC", "cus_01XYZ", []openapiclient.InvoiceLineItemInput{*openapiclient.NewInvoiceLineItemInput("Web Development", "2", "150.00")}) // InvoiceDraftRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InvoicesAPI.CalculateInvoiceApiV1InvoicesCalculatePost(context.Background()).InvoiceDraftRequest(invoiceDraftRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InvoicesAPI.CalculateInvoiceApiV1InvoicesCalculatePost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CalculateInvoiceApiV1InvoicesCalculatePost`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `InvoicesAPI.CalculateInvoiceApiV1InvoicesCalculatePost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCalculateInvoiceApiV1InvoicesCalculatePostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoiceDraftRequest** | [**InvoiceDraftRequest**](InvoiceDraftRequest.md) |  | 

### Return type

**map[string]interface{}**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateInvoiceApiV1InvoicesPost

> InvoiceResponse CreateInvoiceApiV1InvoicesPost(ctx).InvoiceCreateRequest(invoiceCreateRequest).IdempotencyKey(idempotencyKey).Execute()

Create Invoice

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	invoiceCreateRequest := *openapiclient.NewInvoiceCreateRequest("INV-2026-001", time.Now(), "USD", "bp_01ABC", "cus_01XYZ", []openapiclient.InvoiceLineItemInput{*openapiclient.NewInvoiceLineItemInput("Web Development", "2", "150.00")}) // InvoiceCreateRequest | 
	idempotencyKey := "idempotencyKey_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InvoicesAPI.CreateInvoiceApiV1InvoicesPost(context.Background()).InvoiceCreateRequest(invoiceCreateRequest).IdempotencyKey(idempotencyKey).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InvoicesAPI.CreateInvoiceApiV1InvoicesPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateInvoiceApiV1InvoicesPost`: InvoiceResponse
	fmt.Fprintf(os.Stdout, "Response from `InvoicesAPI.CreateInvoiceApiV1InvoicesPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateInvoiceApiV1InvoicesPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoiceCreateRequest** | [**InvoiceCreateRequest**](InvoiceCreateRequest.md) |  | 
 **idempotencyKey** | **string** |  | 

### Return type

[**InvoiceResponse**](InvoiceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteInvoiceApiV1InvoicesInvoiceIdDelete

> SimpleBoolResponse DeleteInvoiceApiV1InvoicesInvoiceIdDelete(ctx, invoiceId).Execute()

Delete Invoice

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	invoiceId := "invoiceId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InvoicesAPI.DeleteInvoiceApiV1InvoicesInvoiceIdDelete(context.Background(), invoiceId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InvoicesAPI.DeleteInvoiceApiV1InvoicesInvoiceIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteInvoiceApiV1InvoicesInvoiceIdDelete`: SimpleBoolResponse
	fmt.Fprintf(os.Stdout, "Response from `InvoicesAPI.DeleteInvoiceApiV1InvoicesInvoiceIdDelete`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**invoiceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteInvoiceApiV1InvoicesInvoiceIdDeleteRequest struct via the builder pattern


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


## DuplicateInvoiceApiV1InvoicesInvoiceIdDuplicatePost

> InvoiceResponse DuplicateInvoiceApiV1InvoicesInvoiceIdDuplicatePost(ctx, invoiceId).Execute()

Duplicate Invoice

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	invoiceId := "invoiceId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InvoicesAPI.DuplicateInvoiceApiV1InvoicesInvoiceIdDuplicatePost(context.Background(), invoiceId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InvoicesAPI.DuplicateInvoiceApiV1InvoicesInvoiceIdDuplicatePost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DuplicateInvoiceApiV1InvoicesInvoiceIdDuplicatePost`: InvoiceResponse
	fmt.Fprintf(os.Stdout, "Response from `InvoicesAPI.DuplicateInvoiceApiV1InvoicesInvoiceIdDuplicatePost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**invoiceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDuplicateInvoiceApiV1InvoicesInvoiceIdDuplicatePostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**InvoiceResponse**](InvoiceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## FinalizeInvoiceApiV1InvoicesInvoiceIdFinalizePost

> map[string]interface{} FinalizeInvoiceApiV1InvoicesInvoiceIdFinalizePost(ctx, invoiceId).IdempotencyKey(idempotencyKey).Execute()

Finalize Invoice

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	invoiceId := "invoiceId_example" // string | 
	idempotencyKey := "idempotencyKey_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InvoicesAPI.FinalizeInvoiceApiV1InvoicesInvoiceIdFinalizePost(context.Background(), invoiceId).IdempotencyKey(idempotencyKey).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InvoicesAPI.FinalizeInvoiceApiV1InvoicesInvoiceIdFinalizePost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FinalizeInvoiceApiV1InvoicesInvoiceIdFinalizePost`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `InvoicesAPI.FinalizeInvoiceApiV1InvoicesInvoiceIdFinalizePost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**invoiceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiFinalizeInvoiceApiV1InvoicesInvoiceIdFinalizePostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **idempotencyKey** | **string** |  | 

### Return type

**map[string]interface{}**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetInvoiceApiV1InvoicesInvoiceIdGet

> InvoiceResponse GetInvoiceApiV1InvoicesInvoiceIdGet(ctx, invoiceId).Execute()

Get Invoice

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	invoiceId := "invoiceId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InvoicesAPI.GetInvoiceApiV1InvoicesInvoiceIdGet(context.Background(), invoiceId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InvoicesAPI.GetInvoiceApiV1InvoicesInvoiceIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetInvoiceApiV1InvoicesInvoiceIdGet`: InvoiceResponse
	fmt.Fprintf(os.Stdout, "Response from `InvoicesAPI.GetInvoiceApiV1InvoicesInvoiceIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**invoiceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetInvoiceApiV1InvoicesInvoiceIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**InvoiceResponse**](InvoiceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListInvoiceDeliveriesApiV1InvoicesInvoiceIdDeliveriesGet

> DeliveriesListResponse ListInvoiceDeliveriesApiV1InvoicesInvoiceIdDeliveriesGet(ctx, invoiceId).Limit(limit).Cursor(cursor).Execute()

List Invoice Deliveries

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	invoiceId := "invoiceId_example" // string | 
	limit := int32(56) // int32 |  (optional) (default to 50)
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InvoicesAPI.ListInvoiceDeliveriesApiV1InvoicesInvoiceIdDeliveriesGet(context.Background(), invoiceId).Limit(limit).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InvoicesAPI.ListInvoiceDeliveriesApiV1InvoicesInvoiceIdDeliveriesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListInvoiceDeliveriesApiV1InvoicesInvoiceIdDeliveriesGet`: DeliveriesListResponse
	fmt.Fprintf(os.Stdout, "Response from `InvoicesAPI.ListInvoiceDeliveriesApiV1InvoicesInvoiceIdDeliveriesGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**invoiceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListInvoiceDeliveriesApiV1InvoicesInvoiceIdDeliveriesGetRequest struct via the builder pattern


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


## ListInvoicesApiV1InvoicesGet

> InvoicesListResponse ListInvoicesApiV1InvoicesGet(ctx).Limit(limit).Cursor(cursor).Status(status).Execute()

List Invoices

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	limit := int32(56) // int32 |  (optional) (default to 50)
	cursor := "cursor_example" // string |  (optional)
	status := "status_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InvoicesAPI.ListInvoicesApiV1InvoicesGet(context.Background()).Limit(limit).Cursor(cursor).Status(status).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InvoicesAPI.ListInvoicesApiV1InvoicesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListInvoicesApiV1InvoicesGet`: InvoicesListResponse
	fmt.Fprintf(os.Stdout, "Response from `InvoicesAPI.ListInvoicesApiV1InvoicesGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListInvoicesApiV1InvoicesGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int32** |  | [default to 50]
 **cursor** | **string** |  | 
 **status** | **string** |  | 

### Return type

[**InvoicesListResponse**](InvoicesListResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MarkPaidApiV1InvoicesInvoiceIdMarkPaidPost

> InvoiceResponse MarkPaidApiV1InvoicesInvoiceIdMarkPaidPost(ctx, invoiceId).Execute()

Mark Paid

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	invoiceId := "invoiceId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InvoicesAPI.MarkPaidApiV1InvoicesInvoiceIdMarkPaidPost(context.Background(), invoiceId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InvoicesAPI.MarkPaidApiV1InvoicesInvoiceIdMarkPaidPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MarkPaidApiV1InvoicesInvoiceIdMarkPaidPost`: InvoiceResponse
	fmt.Fprintf(os.Stdout, "Response from `InvoicesAPI.MarkPaidApiV1InvoicesInvoiceIdMarkPaidPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**invoiceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiMarkPaidApiV1InvoicesInvoiceIdMarkPaidPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**InvoiceResponse**](InvoiceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MarkSentApiV1InvoicesInvoiceIdMarkSentPost

> InvoiceResponse MarkSentApiV1InvoicesInvoiceIdMarkSentPost(ctx, invoiceId).Execute()

Mark Sent

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	invoiceId := "invoiceId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InvoicesAPI.MarkSentApiV1InvoicesInvoiceIdMarkSentPost(context.Background(), invoiceId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InvoicesAPI.MarkSentApiV1InvoicesInvoiceIdMarkSentPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MarkSentApiV1InvoicesInvoiceIdMarkSentPost`: InvoiceResponse
	fmt.Fprintf(os.Stdout, "Response from `InvoicesAPI.MarkSentApiV1InvoicesInvoiceIdMarkSentPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**invoiceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiMarkSentApiV1InvoicesInvoiceIdMarkSentPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**InvoiceResponse**](InvoiceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MarkUnpaidApiV1InvoicesInvoiceIdMarkUnpaidPost

> InvoiceResponse MarkUnpaidApiV1InvoicesInvoiceIdMarkUnpaidPost(ctx, invoiceId).Execute()

Mark Unpaid

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	invoiceId := "invoiceId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InvoicesAPI.MarkUnpaidApiV1InvoicesInvoiceIdMarkUnpaidPost(context.Background(), invoiceId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InvoicesAPI.MarkUnpaidApiV1InvoicesInvoiceIdMarkUnpaidPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MarkUnpaidApiV1InvoicesInvoiceIdMarkUnpaidPost`: InvoiceResponse
	fmt.Fprintf(os.Stdout, "Response from `InvoicesAPI.MarkUnpaidApiV1InvoicesInvoiceIdMarkUnpaidPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**invoiceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiMarkUnpaidApiV1InvoicesInvoiceIdMarkUnpaidPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**InvoiceResponse**](InvoiceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PatchInvoiceApiV1InvoicesInvoiceIdPatch

> InvoiceResponse PatchInvoiceApiV1InvoicesInvoiceIdPatch(ctx, invoiceId).InvoicePatchRequest(invoicePatchRequest).IdempotencyKey(idempotencyKey).Execute()

Patch Invoice

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	invoiceId := "invoiceId_example" // string | 
	invoicePatchRequest := *openapiclient.NewInvoicePatchRequest() // InvoicePatchRequest | 
	idempotencyKey := "idempotencyKey_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InvoicesAPI.PatchInvoiceApiV1InvoicesInvoiceIdPatch(context.Background(), invoiceId).InvoicePatchRequest(invoicePatchRequest).IdempotencyKey(idempotencyKey).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InvoicesAPI.PatchInvoiceApiV1InvoicesInvoiceIdPatch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PatchInvoiceApiV1InvoicesInvoiceIdPatch`: InvoiceResponse
	fmt.Fprintf(os.Stdout, "Response from `InvoicesAPI.PatchInvoiceApiV1InvoicesInvoiceIdPatch`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**invoiceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiPatchInvoiceApiV1InvoicesInvoiceIdPatchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **invoicePatchRequest** | [**InvoicePatchRequest**](InvoicePatchRequest.md) |  | 
 **idempotencyKey** | **string** |  | 

### Return type

[**InvoiceResponse**](InvoiceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PreviewInvoiceApiV1InvoicesPreviewPost

> interface{} PreviewInvoiceApiV1InvoicesPreviewPost(ctx).InvoicePreviewRequest(invoicePreviewRequest).Execute()

Preview Invoice

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	invoicePreviewRequest := *openapiclient.NewInvoicePreviewRequest("INV-2026-001", time.Now(), "USD", "bp_01ABC", "cus_01XYZ", []openapiclient.InvoiceLineItemInput{*openapiclient.NewInvoiceLineItemInput("Web Development", "2", "150.00")}) // InvoicePreviewRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InvoicesAPI.PreviewInvoiceApiV1InvoicesPreviewPost(context.Background()).InvoicePreviewRequest(invoicePreviewRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InvoicesAPI.PreviewInvoiceApiV1InvoicesPreviewPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PreviewInvoiceApiV1InvoicesPreviewPost`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `InvoicesAPI.PreviewInvoiceApiV1InvoicesPreviewPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiPreviewInvoiceApiV1InvoicesPreviewPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoicePreviewRequest** | [**InvoicePreviewRequest**](InvoicePreviewRequest.md) |  | 

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


## RenderInvoiceApiV1InvoicesInvoiceIdRendersPost

> interface{} RenderInvoiceApiV1InvoicesInvoiceIdRendersPost(ctx, invoiceId).InvoiceRenderRequest(invoiceRenderRequest).IdempotencyKey(idempotencyKey).Execute()

Render Invoice

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	invoiceId := "invoiceId_example" // string | 
	invoiceRenderRequest := *openapiclient.NewInvoiceRenderRequest() // InvoiceRenderRequest | 
	idempotencyKey := "idempotencyKey_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InvoicesAPI.RenderInvoiceApiV1InvoicesInvoiceIdRendersPost(context.Background(), invoiceId).InvoiceRenderRequest(invoiceRenderRequest).IdempotencyKey(idempotencyKey).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InvoicesAPI.RenderInvoiceApiV1InvoicesInvoiceIdRendersPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RenderInvoiceApiV1InvoicesInvoiceIdRendersPost`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `InvoicesAPI.RenderInvoiceApiV1InvoicesInvoiceIdRendersPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**invoiceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRenderInvoiceApiV1InvoicesInvoiceIdRendersPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **invoiceRenderRequest** | [**InvoiceRenderRequest**](InvoiceRenderRequest.md) |  | 
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


## ReplaceInvoiceApiV1InvoicesInvoiceIdPut

> InvoiceResponse ReplaceInvoiceApiV1InvoicesInvoiceIdPut(ctx, invoiceId).InvoiceCreateRequest(invoiceCreateRequest).IdempotencyKey(idempotencyKey).Execute()

Replace Invoice

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	invoiceId := "invoiceId_example" // string | 
	invoiceCreateRequest := *openapiclient.NewInvoiceCreateRequest("INV-2026-001", time.Now(), "USD", "bp_01ABC", "cus_01XYZ", []openapiclient.InvoiceLineItemInput{*openapiclient.NewInvoiceLineItemInput("Web Development", "2", "150.00")}) // InvoiceCreateRequest | 
	idempotencyKey := "idempotencyKey_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InvoicesAPI.ReplaceInvoiceApiV1InvoicesInvoiceIdPut(context.Background(), invoiceId).InvoiceCreateRequest(invoiceCreateRequest).IdempotencyKey(idempotencyKey).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InvoicesAPI.ReplaceInvoiceApiV1InvoicesInvoiceIdPut``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ReplaceInvoiceApiV1InvoicesInvoiceIdPut`: InvoiceResponse
	fmt.Fprintf(os.Stdout, "Response from `InvoicesAPI.ReplaceInvoiceApiV1InvoicesInvoiceIdPut`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**invoiceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiReplaceInvoiceApiV1InvoicesInvoiceIdPutRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **invoiceCreateRequest** | [**InvoiceCreateRequest**](InvoiceCreateRequest.md) |  | 
 **idempotencyKey** | **string** |  | 

### Return type

[**InvoiceResponse**](InvoiceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RestoreInvoiceApiV1InvoicesInvoiceIdRestorePost

> InvoiceResponse RestoreInvoiceApiV1InvoicesInvoiceIdRestorePost(ctx, invoiceId).Execute()

Restore Invoice

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	invoiceId := "invoiceId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InvoicesAPI.RestoreInvoiceApiV1InvoicesInvoiceIdRestorePost(context.Background(), invoiceId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InvoicesAPI.RestoreInvoiceApiV1InvoicesInvoiceIdRestorePost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RestoreInvoiceApiV1InvoicesInvoiceIdRestorePost`: InvoiceResponse
	fmt.Fprintf(os.Stdout, "Response from `InvoicesAPI.RestoreInvoiceApiV1InvoicesInvoiceIdRestorePost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**invoiceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRestoreInvoiceApiV1InvoicesInvoiceIdRestorePostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**InvoiceResponse**](InvoiceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SendInvoiceApiV1InvoicesInvoiceIdSendPost

> DeliveryResponse SendInvoiceApiV1InvoicesInvoiceIdSendPost(ctx, invoiceId).DeliverySendRequest(deliverySendRequest).Execute()

Send Invoice

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	invoiceId := "invoiceId_example" // string | 
	deliverySendRequest := *openapiclient.NewDeliverySendRequest([]string{"To_example"}) // DeliverySendRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InvoicesAPI.SendInvoiceApiV1InvoicesInvoiceIdSendPost(context.Background(), invoiceId).DeliverySendRequest(deliverySendRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InvoicesAPI.SendInvoiceApiV1InvoicesInvoiceIdSendPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SendInvoiceApiV1InvoicesInvoiceIdSendPost`: DeliveryResponse
	fmt.Fprintf(os.Stdout, "Response from `InvoicesAPI.SendInvoiceApiV1InvoicesInvoiceIdSendPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**invoiceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiSendInvoiceApiV1InvoicesInvoiceIdSendPostRequest struct via the builder pattern


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


## ValidateInvoiceApiV1InvoicesValidatePost

> map[string]interface{} ValidateInvoiceApiV1InvoicesValidatePost(ctx).InvoiceDraftRequest(invoiceDraftRequest).Execute()

Validate Invoice

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	invoiceDraftRequest := *openapiclient.NewInvoiceDraftRequest("INV-2026-001", time.Now(), "USD", "bp_01ABC", "cus_01XYZ", []openapiclient.InvoiceLineItemInput{*openapiclient.NewInvoiceLineItemInput("Web Development", "2", "150.00")}) // InvoiceDraftRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InvoicesAPI.ValidateInvoiceApiV1InvoicesValidatePost(context.Background()).InvoiceDraftRequest(invoiceDraftRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InvoicesAPI.ValidateInvoiceApiV1InvoicesValidatePost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ValidateInvoiceApiV1InvoicesValidatePost`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `InvoicesAPI.ValidateInvoiceApiV1InvoicesValidatePost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiValidateInvoiceApiV1InvoicesValidatePostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoiceDraftRequest** | [**InvoiceDraftRequest**](InvoiceDraftRequest.md) |  | 

### Return type

**map[string]interface{}**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## VoidInvoiceApiV1InvoicesInvoiceIdVoidPost

> InvoiceResponse VoidInvoiceApiV1InvoicesInvoiceIdVoidPost(ctx, invoiceId).Execute()

Void Invoice

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	invoiceId := "invoiceId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InvoicesAPI.VoidInvoiceApiV1InvoicesInvoiceIdVoidPost(context.Background(), invoiceId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InvoicesAPI.VoidInvoiceApiV1InvoicesInvoiceIdVoidPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `VoidInvoiceApiV1InvoicesInvoiceIdVoidPost`: InvoiceResponse
	fmt.Fprintf(os.Stdout, "Response from `InvoicesAPI.VoidInvoiceApiV1InvoicesInvoiceIdVoidPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**invoiceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiVoidInvoiceApiV1InvoicesInvoiceIdVoidPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**InvoiceResponse**](InvoiceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

