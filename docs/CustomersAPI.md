# \CustomersAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateCustomerApiV1CustomersPost**](CustomersAPI.md#CreateCustomerApiV1CustomersPost) | **Post** /api/v1/customers | Create Customer
[**DeleteCustomerApiV1CustomersCustomerIdDelete**](CustomersAPI.md#DeleteCustomerApiV1CustomersCustomerIdDelete) | **Delete** /api/v1/customers/{customer_id} | Delete Customer
[**GetCustomerApiV1CustomersCustomerIdGet**](CustomersAPI.md#GetCustomerApiV1CustomersCustomerIdGet) | **Get** /api/v1/customers/{customer_id} | Get Customer
[**ListCustomersApiV1CustomersGet**](CustomersAPI.md#ListCustomersApiV1CustomersGet) | **Get** /api/v1/customers | List Customers
[**PatchCustomerApiV1CustomersCustomerIdPatch**](CustomersAPI.md#PatchCustomerApiV1CustomersCustomerIdPatch) | **Patch** /api/v1/customers/{customer_id} | Patch Customer



## CreateCustomerApiV1CustomersPost

> CustomerResponse CreateCustomerApiV1CustomersPost(ctx).CustomerCreate(customerCreate).IdempotencyKey(idempotencyKey).Execute()

Create Customer

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
	customerCreate := *openapiclient.NewCustomerCreate("Jane Smith") // CustomerCreate | 
	idempotencyKey := "idempotencyKey_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CustomersAPI.CreateCustomerApiV1CustomersPost(context.Background()).CustomerCreate(customerCreate).IdempotencyKey(idempotencyKey).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CustomersAPI.CreateCustomerApiV1CustomersPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateCustomerApiV1CustomersPost`: CustomerResponse
	fmt.Fprintf(os.Stdout, "Response from `CustomersAPI.CreateCustomerApiV1CustomersPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateCustomerApiV1CustomersPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customerCreate** | [**CustomerCreate**](CustomerCreate.md) |  | 
 **idempotencyKey** | **string** |  | 

### Return type

[**CustomerResponse**](CustomerResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteCustomerApiV1CustomersCustomerIdDelete

> SimpleBoolResponse DeleteCustomerApiV1CustomersCustomerIdDelete(ctx, customerId).Execute()

Delete Customer

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
	customerId := "customerId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CustomersAPI.DeleteCustomerApiV1CustomersCustomerIdDelete(context.Background(), customerId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CustomersAPI.DeleteCustomerApiV1CustomersCustomerIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteCustomerApiV1CustomersCustomerIdDelete`: SimpleBoolResponse
	fmt.Fprintf(os.Stdout, "Response from `CustomersAPI.DeleteCustomerApiV1CustomersCustomerIdDelete`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**customerId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteCustomerApiV1CustomersCustomerIdDeleteRequest struct via the builder pattern


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


## GetCustomerApiV1CustomersCustomerIdGet

> CustomerResponse GetCustomerApiV1CustomersCustomerIdGet(ctx, customerId).Execute()

Get Customer

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
	customerId := "customerId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CustomersAPI.GetCustomerApiV1CustomersCustomerIdGet(context.Background(), customerId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CustomersAPI.GetCustomerApiV1CustomersCustomerIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetCustomerApiV1CustomersCustomerIdGet`: CustomerResponse
	fmt.Fprintf(os.Stdout, "Response from `CustomersAPI.GetCustomerApiV1CustomersCustomerIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**customerId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetCustomerApiV1CustomersCustomerIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**CustomerResponse**](CustomerResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListCustomersApiV1CustomersGet

> CustomersListResponse ListCustomersApiV1CustomersGet(ctx).Limit(limit).Cursor(cursor).Execute()

List Customers

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
	resp, r, err := apiClient.CustomersAPI.ListCustomersApiV1CustomersGet(context.Background()).Limit(limit).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CustomersAPI.ListCustomersApiV1CustomersGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListCustomersApiV1CustomersGet`: CustomersListResponse
	fmt.Fprintf(os.Stdout, "Response from `CustomersAPI.ListCustomersApiV1CustomersGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListCustomersApiV1CustomersGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int32** |  | [default to 50]
 **cursor** | **string** |  | 

### Return type

[**CustomersListResponse**](CustomersListResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PatchCustomerApiV1CustomersCustomerIdPatch

> CustomerResponse PatchCustomerApiV1CustomersCustomerIdPatch(ctx, customerId).CustomerPatch(customerPatch).IdempotencyKey(idempotencyKey).Execute()

Patch Customer

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
	customerId := "customerId_example" // string | 
	customerPatch := *openapiclient.NewCustomerPatch() // CustomerPatch | 
	idempotencyKey := "idempotencyKey_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CustomersAPI.PatchCustomerApiV1CustomersCustomerIdPatch(context.Background(), customerId).CustomerPatch(customerPatch).IdempotencyKey(idempotencyKey).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CustomersAPI.PatchCustomerApiV1CustomersCustomerIdPatch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PatchCustomerApiV1CustomersCustomerIdPatch`: CustomerResponse
	fmt.Fprintf(os.Stdout, "Response from `CustomersAPI.PatchCustomerApiV1CustomersCustomerIdPatch`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**customerId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiPatchCustomerApiV1CustomersCustomerIdPatchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **customerPatch** | [**CustomerPatch**](CustomerPatch.md) |  | 
 **idempotencyKey** | **string** |  | 

### Return type

[**CustomerResponse**](CustomerResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

