# \TaxRatesAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateTaxRate**](TaxRatesAPI.md#CreateTaxRate) | **Post** /api/v1/tax-rates | Create Tax Rate
[**DeleteTaxRate**](TaxRatesAPI.md#DeleteTaxRate) | **Delete** /api/v1/tax-rates/{tax_rate_id} | Delete Tax Rate
[**GetTaxRate**](TaxRatesAPI.md#GetTaxRate) | **Get** /api/v1/tax-rates/{tax_rate_id} | Get Tax Rate
[**ListTaxRates**](TaxRatesAPI.md#ListTaxRates) | **Get** /api/v1/tax-rates | List Tax Rates
[**UpdateTaxRate**](TaxRatesAPI.md#UpdateTaxRate) | **Patch** /api/v1/tax-rates/{tax_rate_id} | Update Tax Rate



## CreateTaxRate

> TaxRateResponse CreateTaxRate(ctx).TaxRateCreateRequest(taxRateCreateRequest).Execute()

Create Tax Rate

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
	taxRateCreateRequest := *openapiclient.NewTaxRateCreateRequest("California sales tax", "8.375") // TaxRateCreateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaxRatesAPI.CreateTaxRate(context.Background()).TaxRateCreateRequest(taxRateCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaxRatesAPI.CreateTaxRate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateTaxRate`: TaxRateResponse
	fmt.Fprintf(os.Stdout, "Response from `TaxRatesAPI.CreateTaxRate`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateTaxRateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **taxRateCreateRequest** | [**TaxRateCreateRequest**](TaxRateCreateRequest.md) |  | 

### Return type

[**TaxRateResponse**](TaxRateResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteTaxRate

> SimpleBoolResponse DeleteTaxRate(ctx, taxRateId).Execute()

Delete Tax Rate

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
	taxRateId := "taxRateId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaxRatesAPI.DeleteTaxRate(context.Background(), taxRateId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaxRatesAPI.DeleteTaxRate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteTaxRate`: SimpleBoolResponse
	fmt.Fprintf(os.Stdout, "Response from `TaxRatesAPI.DeleteTaxRate`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**taxRateId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteTaxRateRequest struct via the builder pattern


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


## GetTaxRate

> TaxRateResponse GetTaxRate(ctx, taxRateId).Execute()

Get Tax Rate

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
	taxRateId := "taxRateId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaxRatesAPI.GetTaxRate(context.Background(), taxRateId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaxRatesAPI.GetTaxRate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetTaxRate`: TaxRateResponse
	fmt.Fprintf(os.Stdout, "Response from `TaxRatesAPI.GetTaxRate`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**taxRateId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetTaxRateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**TaxRateResponse**](TaxRateResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListTaxRates

> TaxRatesListResponse ListTaxRates(ctx).Limit(limit).Cursor(cursor).Execute()

List Tax Rates

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaxRatesAPI.ListTaxRates(context.Background()).Limit(limit).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaxRatesAPI.ListTaxRates``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListTaxRates`: TaxRatesListResponse
	fmt.Fprintf(os.Stdout, "Response from `TaxRatesAPI.ListTaxRates`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListTaxRatesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int32** |  | [default to 50]
 **cursor** | **string** |  | 

### Return type

[**TaxRatesListResponse**](TaxRatesListResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateTaxRate

> TaxRateResponse UpdateTaxRate(ctx, taxRateId).TaxRatePatchRequest(taxRatePatchRequest).Execute()

Update Tax Rate

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
	taxRateId := "taxRateId_example" // string | 
	taxRatePatchRequest := *openapiclient.NewTaxRatePatchRequest() // TaxRatePatchRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaxRatesAPI.UpdateTaxRate(context.Background(), taxRateId).TaxRatePatchRequest(taxRatePatchRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaxRatesAPI.UpdateTaxRate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateTaxRate`: TaxRateResponse
	fmt.Fprintf(os.Stdout, "Response from `TaxRatesAPI.UpdateTaxRate`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**taxRateId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateTaxRateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **taxRatePatchRequest** | [**TaxRatePatchRequest**](TaxRatePatchRequest.md) |  | 

### Return type

[**TaxRateResponse**](TaxRateResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

