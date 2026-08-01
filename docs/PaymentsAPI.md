# \PaymentsAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreatePaymentApiV1InvoicesInvoiceIdPaymentsPost**](PaymentsAPI.md#CreatePaymentApiV1InvoicesInvoiceIdPaymentsPost) | **Post** /api/v1/invoices/{invoice_id}/payments | Create Payment
[**DeletePaymentApiV1PaymentsPaymentIdDelete**](PaymentsAPI.md#DeletePaymentApiV1PaymentsPaymentIdDelete) | **Delete** /api/v1/payments/{payment_id} | Delete Payment
[**GetPaymentApiV1PaymentsPaymentIdGet**](PaymentsAPI.md#GetPaymentApiV1PaymentsPaymentIdGet) | **Get** /api/v1/payments/{payment_id} | Get Payment
[**ListInvoicePaymentsApiV1InvoicesInvoiceIdPaymentsGet**](PaymentsAPI.md#ListInvoicePaymentsApiV1InvoicesInvoiceIdPaymentsGet) | **Get** /api/v1/invoices/{invoice_id}/payments | List Invoice Payments
[**UpdatePaymentApiV1PaymentsPaymentIdPatch**](PaymentsAPI.md#UpdatePaymentApiV1PaymentsPaymentIdPatch) | **Patch** /api/v1/payments/{payment_id} | Update Payment



## CreatePaymentApiV1InvoicesInvoiceIdPaymentsPost

> PaymentResponse CreatePaymentApiV1InvoicesInvoiceIdPaymentsPost(ctx, invoiceId).PaymentCreateRequest(paymentCreateRequest).Execute()

Create Payment

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
	invoiceId := "invoiceId_example" // string | 
	paymentCreateRequest := *openapiclient.NewPaymentCreateRequest("53.10", time.Now()) // PaymentCreateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PaymentsAPI.CreatePaymentApiV1InvoicesInvoiceIdPaymentsPost(context.Background(), invoiceId).PaymentCreateRequest(paymentCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PaymentsAPI.CreatePaymentApiV1InvoicesInvoiceIdPaymentsPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreatePaymentApiV1InvoicesInvoiceIdPaymentsPost`: PaymentResponse
	fmt.Fprintf(os.Stdout, "Response from `PaymentsAPI.CreatePaymentApiV1InvoicesInvoiceIdPaymentsPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**invoiceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreatePaymentApiV1InvoicesInvoiceIdPaymentsPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **paymentCreateRequest** | [**PaymentCreateRequest**](PaymentCreateRequest.md) |  | 

### Return type

[**PaymentResponse**](PaymentResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeletePaymentApiV1PaymentsPaymentIdDelete

> SimpleBoolResponse DeletePaymentApiV1PaymentsPaymentIdDelete(ctx, paymentId).Execute()

Delete Payment

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
	paymentId := "paymentId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PaymentsAPI.DeletePaymentApiV1PaymentsPaymentIdDelete(context.Background(), paymentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PaymentsAPI.DeletePaymentApiV1PaymentsPaymentIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeletePaymentApiV1PaymentsPaymentIdDelete`: SimpleBoolResponse
	fmt.Fprintf(os.Stdout, "Response from `PaymentsAPI.DeletePaymentApiV1PaymentsPaymentIdDelete`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**paymentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeletePaymentApiV1PaymentsPaymentIdDeleteRequest struct via the builder pattern


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


## GetPaymentApiV1PaymentsPaymentIdGet

> PaymentResponse GetPaymentApiV1PaymentsPaymentIdGet(ctx, paymentId).Execute()

Get Payment

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
	paymentId := "paymentId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PaymentsAPI.GetPaymentApiV1PaymentsPaymentIdGet(context.Background(), paymentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PaymentsAPI.GetPaymentApiV1PaymentsPaymentIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetPaymentApiV1PaymentsPaymentIdGet`: PaymentResponse
	fmt.Fprintf(os.Stdout, "Response from `PaymentsAPI.GetPaymentApiV1PaymentsPaymentIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**paymentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetPaymentApiV1PaymentsPaymentIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**PaymentResponse**](PaymentResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListInvoicePaymentsApiV1InvoicesInvoiceIdPaymentsGet

> PaymentsListResponse ListInvoicePaymentsApiV1InvoicesInvoiceIdPaymentsGet(ctx, invoiceId).Limit(limit).Cursor(cursor).Execute()

List Invoice Payments

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
	invoiceId := "invoiceId_example" // string | 
	limit := int32(56) // int32 |  (optional) (default to 50)
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PaymentsAPI.ListInvoicePaymentsApiV1InvoicesInvoiceIdPaymentsGet(context.Background(), invoiceId).Limit(limit).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PaymentsAPI.ListInvoicePaymentsApiV1InvoicesInvoiceIdPaymentsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListInvoicePaymentsApiV1InvoicesInvoiceIdPaymentsGet`: PaymentsListResponse
	fmt.Fprintf(os.Stdout, "Response from `PaymentsAPI.ListInvoicePaymentsApiV1InvoicesInvoiceIdPaymentsGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**invoiceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListInvoicePaymentsApiV1InvoicesInvoiceIdPaymentsGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **limit** | **int32** |  | [default to 50]
 **cursor** | **string** |  | 

### Return type

[**PaymentsListResponse**](PaymentsListResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdatePaymentApiV1PaymentsPaymentIdPatch

> PaymentResponse UpdatePaymentApiV1PaymentsPaymentIdPatch(ctx, paymentId).PaymentPatchRequest(paymentPatchRequest).Execute()

Update Payment

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
	paymentId := "paymentId_example" // string | 
	paymentPatchRequest := *openapiclient.NewPaymentPatchRequest() // PaymentPatchRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PaymentsAPI.UpdatePaymentApiV1PaymentsPaymentIdPatch(context.Background(), paymentId).PaymentPatchRequest(paymentPatchRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PaymentsAPI.UpdatePaymentApiV1PaymentsPaymentIdPatch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdatePaymentApiV1PaymentsPaymentIdPatch`: PaymentResponse
	fmt.Fprintf(os.Stdout, "Response from `PaymentsAPI.UpdatePaymentApiV1PaymentsPaymentIdPatch`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**paymentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdatePaymentApiV1PaymentsPaymentIdPatchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **paymentPatchRequest** | [**PaymentPatchRequest**](PaymentPatchRequest.md) |  | 

### Return type

[**PaymentResponse**](PaymentResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

