# \ImportsAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CancelImport**](ImportsAPI.md#CancelImport) | **Post** /api/v1/imports/{import_id}/cancel | Cancel Import
[**ConfirmImport**](ImportsAPI.md#ConfirmImport) | **Post** /api/v1/imports/{import_id}/confirm | Confirm Import
[**CreateImport**](ImportsAPI.md#CreateImport) | **Post** /api/v1/imports | Create Import
[**GetImport**](ImportsAPI.md#GetImport) | **Get** /api/v1/imports/{import_id} | Get Import



## CancelImport

> ImportResponse CancelImport(ctx, importId).Execute()

Cancel Import

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
	importId := "importId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ImportsAPI.CancelImport(context.Background(), importId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ImportsAPI.CancelImport``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CancelImport`: ImportResponse
	fmt.Fprintf(os.Stdout, "Response from `ImportsAPI.CancelImport`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**importId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCancelImportRequest struct via the builder pattern


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


## ConfirmImport

> ImportResponse ConfirmImport(ctx, importId).Execute()

Confirm Import

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
	importId := "importId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ImportsAPI.ConfirmImport(context.Background(), importId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ImportsAPI.ConfirmImport``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ConfirmImport`: ImportResponse
	fmt.Fprintf(os.Stdout, "Response from `ImportsAPI.ConfirmImport`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**importId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiConfirmImportRequest struct via the builder pattern


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


## CreateImport

> ImportResponse CreateImport(ctx).ImportCreateRequest(importCreateRequest).Execute()

Create Import

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
	importCreateRequest := *openapiclient.NewImportCreateRequest("csv", []map[string]interface{}{map[string]interface{}{"key": interface{}(123)}}) // ImportCreateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ImportsAPI.CreateImport(context.Background()).ImportCreateRequest(importCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ImportsAPI.CreateImport``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateImport`: ImportResponse
	fmt.Fprintf(os.Stdout, "Response from `ImportsAPI.CreateImport`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateImportRequest struct via the builder pattern


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


## GetImport

> ImportResponse GetImport(ctx, importId).Execute()

Get Import

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
	importId := "importId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ImportsAPI.GetImport(context.Background(), importId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ImportsAPI.GetImport``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetImport`: ImportResponse
	fmt.Fprintf(os.Stdout, "Response from `ImportsAPI.GetImport`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**importId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetImportRequest struct via the builder pattern


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

