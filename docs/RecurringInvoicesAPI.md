# \RecurringInvoicesAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CancelRecurringInvoiceApiV1RecurringInvoicesRecurringIdDelete**](RecurringInvoicesAPI.md#CancelRecurringInvoiceApiV1RecurringInvoicesRecurringIdDelete) | **Delete** /api/v1/recurring-invoices/{recurring_id} | Cancel Recurring Invoice
[**CreateRecurringInvoiceApiV1RecurringInvoicesPost**](RecurringInvoicesAPI.md#CreateRecurringInvoiceApiV1RecurringInvoicesPost) | **Post** /api/v1/recurring-invoices | Create Recurring Invoice
[**GetRecurringInvoiceApiV1RecurringInvoicesRecurringIdGet**](RecurringInvoicesAPI.md#GetRecurringInvoiceApiV1RecurringInvoicesRecurringIdGet) | **Get** /api/v1/recurring-invoices/{recurring_id} | Get Recurring Invoice
[**ListGeneratedInvoicesApiV1RecurringInvoicesRecurringIdInvoicesGet**](RecurringInvoicesAPI.md#ListGeneratedInvoicesApiV1RecurringInvoicesRecurringIdInvoicesGet) | **Get** /api/v1/recurring-invoices/{recurring_id}/invoices | List Generated Invoices
[**ListRecurringInvoicesApiV1RecurringInvoicesGet**](RecurringInvoicesAPI.md#ListRecurringInvoicesApiV1RecurringInvoicesGet) | **Get** /api/v1/recurring-invoices | List Recurring Invoices
[**PatchRecurringInvoiceApiV1RecurringInvoicesRecurringIdPatch**](RecurringInvoicesAPI.md#PatchRecurringInvoiceApiV1RecurringInvoicesRecurringIdPatch) | **Patch** /api/v1/recurring-invoices/{recurring_id} | Patch Recurring Invoice
[**PauseRecurringInvoiceApiV1RecurringInvoicesRecurringIdPausePost**](RecurringInvoicesAPI.md#PauseRecurringInvoiceApiV1RecurringInvoicesRecurringIdPausePost) | **Post** /api/v1/recurring-invoices/{recurring_id}/pause | Pause Recurring Invoice
[**ResumeRecurringInvoiceApiV1RecurringInvoicesRecurringIdResumePost**](RecurringInvoicesAPI.md#ResumeRecurringInvoiceApiV1RecurringInvoicesRecurringIdResumePost) | **Post** /api/v1/recurring-invoices/{recurring_id}/resume | Resume Recurring Invoice



## CancelRecurringInvoiceApiV1RecurringInvoicesRecurringIdDelete

> RecurringInvoiceResponse CancelRecurringInvoiceApiV1RecurringInvoicesRecurringIdDelete(ctx, recurringId).Execute()

Cancel Recurring Invoice

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/invoicepdfs"
)

func main() {
	recurringId := "recurringId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RecurringInvoicesAPI.CancelRecurringInvoiceApiV1RecurringInvoicesRecurringIdDelete(context.Background(), recurringId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RecurringInvoicesAPI.CancelRecurringInvoiceApiV1RecurringInvoicesRecurringIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CancelRecurringInvoiceApiV1RecurringInvoicesRecurringIdDelete`: RecurringInvoiceResponse
	fmt.Fprintf(os.Stdout, "Response from `RecurringInvoicesAPI.CancelRecurringInvoiceApiV1RecurringInvoicesRecurringIdDelete`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**recurringId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCancelRecurringInvoiceApiV1RecurringInvoicesRecurringIdDeleteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**RecurringInvoiceResponse**](RecurringInvoiceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateRecurringInvoiceApiV1RecurringInvoicesPost

> RecurringInvoiceResponse CreateRecurringInvoiceApiV1RecurringInvoicesPost(ctx).RecurringInvoiceCreateRequest(recurringInvoiceCreateRequest).Execute()

Create Recurring Invoice

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/invoicepdfs"
)

func main() {
	recurringInvoiceCreateRequest := *openapiclient.NewRecurringInvoiceCreateRequest("BusinessProfileId_example", "CustomerId_example", "Frequency_example", time.Now(), *openapiclient.NewInvoiceDraftRequest("INV-2026-001", time.Now(), "USD", "bp_01ABC", "cus_01XYZ", []openapiclient.InvoiceLineItemInput{*openapiclient.NewInvoiceLineItemInput("Web Development", "2", "150.00")})) // RecurringInvoiceCreateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RecurringInvoicesAPI.CreateRecurringInvoiceApiV1RecurringInvoicesPost(context.Background()).RecurringInvoiceCreateRequest(recurringInvoiceCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RecurringInvoicesAPI.CreateRecurringInvoiceApiV1RecurringInvoicesPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateRecurringInvoiceApiV1RecurringInvoicesPost`: RecurringInvoiceResponse
	fmt.Fprintf(os.Stdout, "Response from `RecurringInvoicesAPI.CreateRecurringInvoiceApiV1RecurringInvoicesPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateRecurringInvoiceApiV1RecurringInvoicesPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **recurringInvoiceCreateRequest** | [**RecurringInvoiceCreateRequest**](RecurringInvoiceCreateRequest.md) |  | 

### Return type

[**RecurringInvoiceResponse**](RecurringInvoiceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetRecurringInvoiceApiV1RecurringInvoicesRecurringIdGet

> RecurringInvoiceResponse GetRecurringInvoiceApiV1RecurringInvoicesRecurringIdGet(ctx, recurringId).Execute()

Get Recurring Invoice

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/invoicepdfs"
)

func main() {
	recurringId := "recurringId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RecurringInvoicesAPI.GetRecurringInvoiceApiV1RecurringInvoicesRecurringIdGet(context.Background(), recurringId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RecurringInvoicesAPI.GetRecurringInvoiceApiV1RecurringInvoicesRecurringIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetRecurringInvoiceApiV1RecurringInvoicesRecurringIdGet`: RecurringInvoiceResponse
	fmt.Fprintf(os.Stdout, "Response from `RecurringInvoicesAPI.GetRecurringInvoiceApiV1RecurringInvoicesRecurringIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**recurringId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetRecurringInvoiceApiV1RecurringInvoicesRecurringIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**RecurringInvoiceResponse**](RecurringInvoiceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListGeneratedInvoicesApiV1RecurringInvoicesRecurringIdInvoicesGet

> InvoicesListResponse ListGeneratedInvoicesApiV1RecurringInvoicesRecurringIdInvoicesGet(ctx, recurringId).Limit(limit).Cursor(cursor).Execute()

List Generated Invoices

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/invoicepdfs"
)

func main() {
	recurringId := "recurringId_example" // string | 
	limit := int32(56) // int32 |  (optional) (default to 50)
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RecurringInvoicesAPI.ListGeneratedInvoicesApiV1RecurringInvoicesRecurringIdInvoicesGet(context.Background(), recurringId).Limit(limit).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RecurringInvoicesAPI.ListGeneratedInvoicesApiV1RecurringInvoicesRecurringIdInvoicesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListGeneratedInvoicesApiV1RecurringInvoicesRecurringIdInvoicesGet`: InvoicesListResponse
	fmt.Fprintf(os.Stdout, "Response from `RecurringInvoicesAPI.ListGeneratedInvoicesApiV1RecurringInvoicesRecurringIdInvoicesGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**recurringId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListGeneratedInvoicesApiV1RecurringInvoicesRecurringIdInvoicesGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **limit** | **int32** |  | [default to 50]
 **cursor** | **string** |  | 

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


## ListRecurringInvoicesApiV1RecurringInvoicesGet

> RecurringInvoicesListResponse ListRecurringInvoicesApiV1RecurringInvoicesGet(ctx).Limit(limit).Cursor(cursor).Status(status).Execute()

List Recurring Invoices

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/invoicepdfs"
)

func main() {
	limit := int32(56) // int32 |  (optional) (default to 50)
	cursor := "cursor_example" // string |  (optional)
	status := "status_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RecurringInvoicesAPI.ListRecurringInvoicesApiV1RecurringInvoicesGet(context.Background()).Limit(limit).Cursor(cursor).Status(status).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RecurringInvoicesAPI.ListRecurringInvoicesApiV1RecurringInvoicesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListRecurringInvoicesApiV1RecurringInvoicesGet`: RecurringInvoicesListResponse
	fmt.Fprintf(os.Stdout, "Response from `RecurringInvoicesAPI.ListRecurringInvoicesApiV1RecurringInvoicesGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListRecurringInvoicesApiV1RecurringInvoicesGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int32** |  | [default to 50]
 **cursor** | **string** |  | 
 **status** | **string** |  | 

### Return type

[**RecurringInvoicesListResponse**](RecurringInvoicesListResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PatchRecurringInvoiceApiV1RecurringInvoicesRecurringIdPatch

> RecurringInvoiceResponse PatchRecurringInvoiceApiV1RecurringInvoicesRecurringIdPatch(ctx, recurringId).RecurringInvoicePatchRequest(recurringInvoicePatchRequest).Execute()

Patch Recurring Invoice

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/invoicepdfs"
)

func main() {
	recurringId := "recurringId_example" // string | 
	recurringInvoicePatchRequest := *openapiclient.NewRecurringInvoicePatchRequest() // RecurringInvoicePatchRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RecurringInvoicesAPI.PatchRecurringInvoiceApiV1RecurringInvoicesRecurringIdPatch(context.Background(), recurringId).RecurringInvoicePatchRequest(recurringInvoicePatchRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RecurringInvoicesAPI.PatchRecurringInvoiceApiV1RecurringInvoicesRecurringIdPatch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PatchRecurringInvoiceApiV1RecurringInvoicesRecurringIdPatch`: RecurringInvoiceResponse
	fmt.Fprintf(os.Stdout, "Response from `RecurringInvoicesAPI.PatchRecurringInvoiceApiV1RecurringInvoicesRecurringIdPatch`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**recurringId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiPatchRecurringInvoiceApiV1RecurringInvoicesRecurringIdPatchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **recurringInvoicePatchRequest** | [**RecurringInvoicePatchRequest**](RecurringInvoicePatchRequest.md) |  | 

### Return type

[**RecurringInvoiceResponse**](RecurringInvoiceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PauseRecurringInvoiceApiV1RecurringInvoicesRecurringIdPausePost

> RecurringInvoiceResponse PauseRecurringInvoiceApiV1RecurringInvoicesRecurringIdPausePost(ctx, recurringId).Execute()

Pause Recurring Invoice

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/invoicepdfs"
)

func main() {
	recurringId := "recurringId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RecurringInvoicesAPI.PauseRecurringInvoiceApiV1RecurringInvoicesRecurringIdPausePost(context.Background(), recurringId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RecurringInvoicesAPI.PauseRecurringInvoiceApiV1RecurringInvoicesRecurringIdPausePost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PauseRecurringInvoiceApiV1RecurringInvoicesRecurringIdPausePost`: RecurringInvoiceResponse
	fmt.Fprintf(os.Stdout, "Response from `RecurringInvoicesAPI.PauseRecurringInvoiceApiV1RecurringInvoicesRecurringIdPausePost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**recurringId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiPauseRecurringInvoiceApiV1RecurringInvoicesRecurringIdPausePostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**RecurringInvoiceResponse**](RecurringInvoiceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ResumeRecurringInvoiceApiV1RecurringInvoicesRecurringIdResumePost

> RecurringInvoiceResponse ResumeRecurringInvoiceApiV1RecurringInvoicesRecurringIdResumePost(ctx, recurringId).Execute()

Resume Recurring Invoice

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/invoicepdfs"
)

func main() {
	recurringId := "recurringId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RecurringInvoicesAPI.ResumeRecurringInvoiceApiV1RecurringInvoicesRecurringIdResumePost(context.Background(), recurringId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RecurringInvoicesAPI.ResumeRecurringInvoiceApiV1RecurringInvoicesRecurringIdResumePost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ResumeRecurringInvoiceApiV1RecurringInvoicesRecurringIdResumePost`: RecurringInvoiceResponse
	fmt.Fprintf(os.Stdout, "Response from `RecurringInvoicesAPI.ResumeRecurringInvoiceApiV1RecurringInvoicesRecurringIdResumePost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**recurringId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiResumeRecurringInvoiceApiV1RecurringInvoicesRecurringIdResumePostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**RecurringInvoiceResponse**](RecurringInvoiceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

