# \RecurringInvoicesAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CancelRecurringInvoice**](RecurringInvoicesAPI.md#CancelRecurringInvoice) | **Delete** /api/v1/recurring-invoices/{recurring_id} | Cancel Recurring Invoice
[**CreateRecurringInvoice**](RecurringInvoicesAPI.md#CreateRecurringInvoice) | **Post** /api/v1/recurring-invoices | Create Recurring Invoice
[**GetRecurringInvoice**](RecurringInvoicesAPI.md#GetRecurringInvoice) | **Get** /api/v1/recurring-invoices/{recurring_id} | Get Recurring Invoice
[**ListGeneratedInvoices**](RecurringInvoicesAPI.md#ListGeneratedInvoices) | **Get** /api/v1/recurring-invoices/{recurring_id}/invoices | List Generated Invoices
[**ListRecurringInvoices**](RecurringInvoicesAPI.md#ListRecurringInvoices) | **Get** /api/v1/recurring-invoices | List Recurring Invoices
[**PauseRecurringInvoice**](RecurringInvoicesAPI.md#PauseRecurringInvoice) | **Post** /api/v1/recurring-invoices/{recurring_id}/pause | Pause Recurring Invoice
[**ResumeRecurringInvoice**](RecurringInvoicesAPI.md#ResumeRecurringInvoice) | **Post** /api/v1/recurring-invoices/{recurring_id}/resume | Resume Recurring Invoice
[**UpdateRecurringInvoice**](RecurringInvoicesAPI.md#UpdateRecurringInvoice) | **Patch** /api/v1/recurring-invoices/{recurring_id} | Update Recurring Invoice



## CancelRecurringInvoice

> RecurringInvoiceResponse CancelRecurringInvoice(ctx, recurringId).Execute()

Cancel Recurring Invoice

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
	recurringId := "recurringId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RecurringInvoicesAPI.CancelRecurringInvoice(context.Background(), recurringId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RecurringInvoicesAPI.CancelRecurringInvoice``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CancelRecurringInvoice`: RecurringInvoiceResponse
	fmt.Fprintf(os.Stdout, "Response from `RecurringInvoicesAPI.CancelRecurringInvoice`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**recurringId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCancelRecurringInvoiceRequest struct via the builder pattern


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


## CreateRecurringInvoice

> RecurringInvoiceResponse CreateRecurringInvoice(ctx).RecurringInvoiceCreateRequest(recurringInvoiceCreateRequest).Execute()

Create Recurring Invoice

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
	recurringInvoiceCreateRequest := *openapiclient.NewRecurringInvoiceCreateRequest("BusinessProfileId_example", "CustomerId_example", "Frequency_example", time.Now(), *openapiclient.NewInvoiceDraftRequest("INV-2026-001", time.Now(), "USD", "bp_01ABC", "cus_01XYZ", []openapiclient.InvoiceLineItemInput{*openapiclient.NewInvoiceLineItemInput("Web Development", "2", "150.00")})) // RecurringInvoiceCreateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RecurringInvoicesAPI.CreateRecurringInvoice(context.Background()).RecurringInvoiceCreateRequest(recurringInvoiceCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RecurringInvoicesAPI.CreateRecurringInvoice``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateRecurringInvoice`: RecurringInvoiceResponse
	fmt.Fprintf(os.Stdout, "Response from `RecurringInvoicesAPI.CreateRecurringInvoice`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateRecurringInvoiceRequest struct via the builder pattern


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


## GetRecurringInvoice

> RecurringInvoiceResponse GetRecurringInvoice(ctx, recurringId).Execute()

Get Recurring Invoice

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
	recurringId := "recurringId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RecurringInvoicesAPI.GetRecurringInvoice(context.Background(), recurringId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RecurringInvoicesAPI.GetRecurringInvoice``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetRecurringInvoice`: RecurringInvoiceResponse
	fmt.Fprintf(os.Stdout, "Response from `RecurringInvoicesAPI.GetRecurringInvoice`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**recurringId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetRecurringInvoiceRequest struct via the builder pattern


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


## ListGeneratedInvoices

> InvoicesListResponse ListGeneratedInvoices(ctx, recurringId).Limit(limit).Cursor(cursor).Execute()

List Generated Invoices

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
	recurringId := "recurringId_example" // string | 
	limit := int32(56) // int32 |  (optional) (default to 50)
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RecurringInvoicesAPI.ListGeneratedInvoices(context.Background(), recurringId).Limit(limit).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RecurringInvoicesAPI.ListGeneratedInvoices``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListGeneratedInvoices`: InvoicesListResponse
	fmt.Fprintf(os.Stdout, "Response from `RecurringInvoicesAPI.ListGeneratedInvoices`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**recurringId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListGeneratedInvoicesRequest struct via the builder pattern


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


## ListRecurringInvoices

> RecurringInvoicesListResponse ListRecurringInvoices(ctx).Limit(limit).Cursor(cursor).Status(status).Execute()

List Recurring Invoices

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
	status := "status_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RecurringInvoicesAPI.ListRecurringInvoices(context.Background()).Limit(limit).Cursor(cursor).Status(status).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RecurringInvoicesAPI.ListRecurringInvoices``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListRecurringInvoices`: RecurringInvoicesListResponse
	fmt.Fprintf(os.Stdout, "Response from `RecurringInvoicesAPI.ListRecurringInvoices`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListRecurringInvoicesRequest struct via the builder pattern


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


## PauseRecurringInvoice

> RecurringInvoiceResponse PauseRecurringInvoice(ctx, recurringId).Execute()

Pause Recurring Invoice

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
	recurringId := "recurringId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RecurringInvoicesAPI.PauseRecurringInvoice(context.Background(), recurringId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RecurringInvoicesAPI.PauseRecurringInvoice``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PauseRecurringInvoice`: RecurringInvoiceResponse
	fmt.Fprintf(os.Stdout, "Response from `RecurringInvoicesAPI.PauseRecurringInvoice`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**recurringId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiPauseRecurringInvoiceRequest struct via the builder pattern


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


## ResumeRecurringInvoice

> RecurringInvoiceResponse ResumeRecurringInvoice(ctx, recurringId).Execute()

Resume Recurring Invoice

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
	recurringId := "recurringId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RecurringInvoicesAPI.ResumeRecurringInvoice(context.Background(), recurringId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RecurringInvoicesAPI.ResumeRecurringInvoice``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ResumeRecurringInvoice`: RecurringInvoiceResponse
	fmt.Fprintf(os.Stdout, "Response from `RecurringInvoicesAPI.ResumeRecurringInvoice`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**recurringId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiResumeRecurringInvoiceRequest struct via the builder pattern


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


## UpdateRecurringInvoice

> RecurringInvoiceResponse UpdateRecurringInvoice(ctx, recurringId).RecurringInvoicePatchRequest(recurringInvoicePatchRequest).Execute()

Update Recurring Invoice

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
	recurringId := "recurringId_example" // string | 
	recurringInvoicePatchRequest := *openapiclient.NewRecurringInvoicePatchRequest() // RecurringInvoicePatchRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RecurringInvoicesAPI.UpdateRecurringInvoice(context.Background(), recurringId).RecurringInvoicePatchRequest(recurringInvoicePatchRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RecurringInvoicesAPI.UpdateRecurringInvoice``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateRecurringInvoice`: RecurringInvoiceResponse
	fmt.Fprintf(os.Stdout, "Response from `RecurringInvoicesAPI.UpdateRecurringInvoice`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**recurringId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateRecurringInvoiceRequest struct via the builder pattern


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

