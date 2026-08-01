# \TaxRatesAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateTaxRateApiV1TaxRatesPost**](TaxRatesAPI.md#CreateTaxRateApiV1TaxRatesPost) | **Post** /api/v1/tax-rates | Create Tax Rate
[**DeleteTaxRateApiV1TaxRatesTaxRateIdDelete**](TaxRatesAPI.md#DeleteTaxRateApiV1TaxRatesTaxRateIdDelete) | **Delete** /api/v1/tax-rates/{tax_rate_id} | Delete Tax Rate
[**GetTaxRateApiV1TaxRatesTaxRateIdGet**](TaxRatesAPI.md#GetTaxRateApiV1TaxRatesTaxRateIdGet) | **Get** /api/v1/tax-rates/{tax_rate_id} | Get Tax Rate
[**ListTaxRatesApiV1TaxRatesGet**](TaxRatesAPI.md#ListTaxRatesApiV1TaxRatesGet) | **Get** /api/v1/tax-rates | List Tax Rates
[**UpdateTaxRateApiV1TaxRatesTaxRateIdPatch**](TaxRatesAPI.md#UpdateTaxRateApiV1TaxRatesTaxRateIdPatch) | **Patch** /api/v1/tax-rates/{tax_rate_id} | Update Tax Rate



## CreateTaxRateApiV1TaxRatesPost

> TaxRateResponse CreateTaxRateApiV1TaxRatesPost(ctx).TaxRateCreateRequest(taxRateCreateRequest).Execute()

Create Tax Rate

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
	taxRateCreateRequest := *openapiclient.NewTaxRateCreateRequest("California sales tax", "8.375") // TaxRateCreateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaxRatesAPI.CreateTaxRateApiV1TaxRatesPost(context.Background()).TaxRateCreateRequest(taxRateCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaxRatesAPI.CreateTaxRateApiV1TaxRatesPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateTaxRateApiV1TaxRatesPost`: TaxRateResponse
	fmt.Fprintf(os.Stdout, "Response from `TaxRatesAPI.CreateTaxRateApiV1TaxRatesPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateTaxRateApiV1TaxRatesPostRequest struct via the builder pattern


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


## DeleteTaxRateApiV1TaxRatesTaxRateIdDelete

> SimpleBoolResponse DeleteTaxRateApiV1TaxRatesTaxRateIdDelete(ctx, taxRateId).Execute()

Delete Tax Rate

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
	taxRateId := "taxRateId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaxRatesAPI.DeleteTaxRateApiV1TaxRatesTaxRateIdDelete(context.Background(), taxRateId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaxRatesAPI.DeleteTaxRateApiV1TaxRatesTaxRateIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteTaxRateApiV1TaxRatesTaxRateIdDelete`: SimpleBoolResponse
	fmt.Fprintf(os.Stdout, "Response from `TaxRatesAPI.DeleteTaxRateApiV1TaxRatesTaxRateIdDelete`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**taxRateId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteTaxRateApiV1TaxRatesTaxRateIdDeleteRequest struct via the builder pattern


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


## GetTaxRateApiV1TaxRatesTaxRateIdGet

> TaxRateResponse GetTaxRateApiV1TaxRatesTaxRateIdGet(ctx, taxRateId).Execute()

Get Tax Rate

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
	taxRateId := "taxRateId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaxRatesAPI.GetTaxRateApiV1TaxRatesTaxRateIdGet(context.Background(), taxRateId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaxRatesAPI.GetTaxRateApiV1TaxRatesTaxRateIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetTaxRateApiV1TaxRatesTaxRateIdGet`: TaxRateResponse
	fmt.Fprintf(os.Stdout, "Response from `TaxRatesAPI.GetTaxRateApiV1TaxRatesTaxRateIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**taxRateId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetTaxRateApiV1TaxRatesTaxRateIdGetRequest struct via the builder pattern


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


## ListTaxRatesApiV1TaxRatesGet

> TaxRatesListResponse ListTaxRatesApiV1TaxRatesGet(ctx).Limit(limit).Cursor(cursor).Execute()

List Tax Rates

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaxRatesAPI.ListTaxRatesApiV1TaxRatesGet(context.Background()).Limit(limit).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaxRatesAPI.ListTaxRatesApiV1TaxRatesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListTaxRatesApiV1TaxRatesGet`: TaxRatesListResponse
	fmt.Fprintf(os.Stdout, "Response from `TaxRatesAPI.ListTaxRatesApiV1TaxRatesGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListTaxRatesApiV1TaxRatesGetRequest struct via the builder pattern


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


## UpdateTaxRateApiV1TaxRatesTaxRateIdPatch

> TaxRateResponse UpdateTaxRateApiV1TaxRatesTaxRateIdPatch(ctx, taxRateId).TaxRatePatchRequest(taxRatePatchRequest).Execute()

Update Tax Rate

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
	taxRateId := "taxRateId_example" // string | 
	taxRatePatchRequest := *openapiclient.NewTaxRatePatchRequest() // TaxRatePatchRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaxRatesAPI.UpdateTaxRateApiV1TaxRatesTaxRateIdPatch(context.Background(), taxRateId).TaxRatePatchRequest(taxRatePatchRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaxRatesAPI.UpdateTaxRateApiV1TaxRatesTaxRateIdPatch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateTaxRateApiV1TaxRatesTaxRateIdPatch`: TaxRateResponse
	fmt.Fprintf(os.Stdout, "Response from `TaxRatesAPI.UpdateTaxRateApiV1TaxRatesTaxRateIdPatch`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**taxRateId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateTaxRateApiV1TaxRatesTaxRateIdPatchRequest struct via the builder pattern


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

