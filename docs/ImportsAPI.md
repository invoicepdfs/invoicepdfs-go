# \ImportsAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CancelImportApiV1ImportsImportIdCancelPost**](ImportsAPI.md#CancelImportApiV1ImportsImportIdCancelPost) | **Post** /api/v1/imports/{import_id}/cancel | Cancel Import
[**ConfirmImportApiV1ImportsImportIdConfirmPost**](ImportsAPI.md#ConfirmImportApiV1ImportsImportIdConfirmPost) | **Post** /api/v1/imports/{import_id}/confirm | Confirm Import
[**CreateImportApiV1ImportsPost**](ImportsAPI.md#CreateImportApiV1ImportsPost) | **Post** /api/v1/imports | Create Import
[**GetImportApiV1ImportsImportIdGet**](ImportsAPI.md#GetImportApiV1ImportsImportIdGet) | **Get** /api/v1/imports/{import_id} | Get Import



## CancelImportApiV1ImportsImportIdCancelPost

> ImportResponse CancelImportApiV1ImportsImportIdCancelPost(ctx, importId).Execute()

Cancel Import

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
	importId := "importId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ImportsAPI.CancelImportApiV1ImportsImportIdCancelPost(context.Background(), importId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ImportsAPI.CancelImportApiV1ImportsImportIdCancelPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CancelImportApiV1ImportsImportIdCancelPost`: ImportResponse
	fmt.Fprintf(os.Stdout, "Response from `ImportsAPI.CancelImportApiV1ImportsImportIdCancelPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**importId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCancelImportApiV1ImportsImportIdCancelPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**ImportResponse**](ImportResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ConfirmImportApiV1ImportsImportIdConfirmPost

> ImportResponse ConfirmImportApiV1ImportsImportIdConfirmPost(ctx, importId).Execute()

Confirm Import

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
	importId := "importId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ImportsAPI.ConfirmImportApiV1ImportsImportIdConfirmPost(context.Background(), importId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ImportsAPI.ConfirmImportApiV1ImportsImportIdConfirmPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ConfirmImportApiV1ImportsImportIdConfirmPost`: ImportResponse
	fmt.Fprintf(os.Stdout, "Response from `ImportsAPI.ConfirmImportApiV1ImportsImportIdConfirmPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**importId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiConfirmImportApiV1ImportsImportIdConfirmPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**ImportResponse**](ImportResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateImportApiV1ImportsPost

> ImportResponse CreateImportApiV1ImportsPost(ctx).ImportCreateRequest(importCreateRequest).Execute()

Create Import

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
	importCreateRequest := *openapiclient.NewImportCreateRequest("csv", []map[string]interface{}{map[string]interface{}{"key": interface{}(123)}}) // ImportCreateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ImportsAPI.CreateImportApiV1ImportsPost(context.Background()).ImportCreateRequest(importCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ImportsAPI.CreateImportApiV1ImportsPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateImportApiV1ImportsPost`: ImportResponse
	fmt.Fprintf(os.Stdout, "Response from `ImportsAPI.CreateImportApiV1ImportsPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateImportApiV1ImportsPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **importCreateRequest** | [**ImportCreateRequest**](ImportCreateRequest.md) |  | 

### Return type

[**ImportResponse**](ImportResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetImportApiV1ImportsImportIdGet

> ImportResponse GetImportApiV1ImportsImportIdGet(ctx, importId).Execute()

Get Import

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
	importId := "importId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ImportsAPI.GetImportApiV1ImportsImportIdGet(context.Background(), importId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ImportsAPI.GetImportApiV1ImportsImportIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetImportApiV1ImportsImportIdGet`: ImportResponse
	fmt.Fprintf(os.Stdout, "Response from `ImportsAPI.GetImportApiV1ImportsImportIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**importId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetImportApiV1ImportsImportIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**ImportResponse**](ImportResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

