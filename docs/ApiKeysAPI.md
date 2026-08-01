# \ApiKeysAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateApiKeyApiV1ApiKeysPost**](ApiKeysAPI.md#CreateApiKeyApiV1ApiKeysPost) | **Post** /api/v1/api-keys | Create Api Key
[**GetApiKeyApiV1ApiKeysApiKeyIdGet**](ApiKeysAPI.md#GetApiKeyApiV1ApiKeysApiKeyIdGet) | **Get** /api/v1/api-keys/{api_key_id} | Get Api Key
[**ListApiKeysApiV1ApiKeysGet**](ApiKeysAPI.md#ListApiKeysApiV1ApiKeysGet) | **Get** /api/v1/api-keys | List Api Keys
[**PatchApiKeyApiV1ApiKeysApiKeyIdPatch**](ApiKeysAPI.md#PatchApiKeyApiV1ApiKeysApiKeyIdPatch) | **Patch** /api/v1/api-keys/{api_key_id} | Patch Api Key
[**RevokeApiKeyApiV1ApiKeysApiKeyIdDelete**](ApiKeysAPI.md#RevokeApiKeyApiV1ApiKeysApiKeyIdDelete) | **Delete** /api/v1/api-keys/{api_key_id} | Revoke Api Key
[**RotateApiKeyApiV1ApiKeysApiKeyIdRotatePost**](ApiKeysAPI.md#RotateApiKeyApiV1ApiKeysApiKeyIdRotatePost) | **Post** /api/v1/api-keys/{api_key_id}/rotate | Rotate Api Key



## CreateApiKeyApiV1ApiKeysPost

> ApiKeyCreateResponse CreateApiKeyApiV1ApiKeysPost(ctx).ApiKeyCreateRequest(apiKeyCreateRequest).Execute()

Create Api Key

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
	apiKeyCreateRequest := *openapiclient.NewApiKeyCreateRequest() // ApiKeyCreateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApiKeysAPI.CreateApiKeyApiV1ApiKeysPost(context.Background()).ApiKeyCreateRequest(apiKeyCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApiKeysAPI.CreateApiKeyApiV1ApiKeysPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateApiKeyApiV1ApiKeysPost`: ApiKeyCreateResponse
	fmt.Fprintf(os.Stdout, "Response from `ApiKeysAPI.CreateApiKeyApiV1ApiKeysPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateApiKeyApiV1ApiKeysPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiKeyCreateRequest** | [**ApiKeyCreateRequest**](ApiKeyCreateRequest.md) |  | 

### Return type

[**ApiKeyCreateResponse**](ApiKeyCreateResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetApiKeyApiV1ApiKeysApiKeyIdGet

> ApiKeyDetailResponse GetApiKeyApiV1ApiKeysApiKeyIdGet(ctx, apiKeyId).Execute()

Get Api Key

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
	apiKeyId := "apiKeyId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApiKeysAPI.GetApiKeyApiV1ApiKeysApiKeyIdGet(context.Background(), apiKeyId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApiKeysAPI.GetApiKeyApiV1ApiKeysApiKeyIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetApiKeyApiV1ApiKeysApiKeyIdGet`: ApiKeyDetailResponse
	fmt.Fprintf(os.Stdout, "Response from `ApiKeysAPI.GetApiKeyApiV1ApiKeysApiKeyIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**apiKeyId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetApiKeyApiV1ApiKeysApiKeyIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**ApiKeyDetailResponse**](ApiKeyDetailResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListApiKeysApiV1ApiKeysGet

> ApiKeyListResponse ListApiKeysApiV1ApiKeysGet(ctx).Execute()

List Api Keys

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApiKeysAPI.ListApiKeysApiV1ApiKeysGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApiKeysAPI.ListApiKeysApiV1ApiKeysGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListApiKeysApiV1ApiKeysGet`: ApiKeyListResponse
	fmt.Fprintf(os.Stdout, "Response from `ApiKeysAPI.ListApiKeysApiV1ApiKeysGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListApiKeysApiV1ApiKeysGetRequest struct via the builder pattern


### Return type

[**ApiKeyListResponse**](ApiKeyListResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PatchApiKeyApiV1ApiKeysApiKeyIdPatch

> ApiKeyDetailResponse PatchApiKeyApiV1ApiKeysApiKeyIdPatch(ctx, apiKeyId).ApiKeyPatchRequest(apiKeyPatchRequest).Execute()

Patch Api Key

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
	apiKeyId := "apiKeyId_example" // string | 
	apiKeyPatchRequest := *openapiclient.NewApiKeyPatchRequest("Name_example") // ApiKeyPatchRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApiKeysAPI.PatchApiKeyApiV1ApiKeysApiKeyIdPatch(context.Background(), apiKeyId).ApiKeyPatchRequest(apiKeyPatchRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApiKeysAPI.PatchApiKeyApiV1ApiKeysApiKeyIdPatch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PatchApiKeyApiV1ApiKeysApiKeyIdPatch`: ApiKeyDetailResponse
	fmt.Fprintf(os.Stdout, "Response from `ApiKeysAPI.PatchApiKeyApiV1ApiKeysApiKeyIdPatch`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**apiKeyId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiPatchApiKeyApiV1ApiKeysApiKeyIdPatchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **apiKeyPatchRequest** | [**ApiKeyPatchRequest**](ApiKeyPatchRequest.md) |  | 

### Return type

[**ApiKeyDetailResponse**](ApiKeyDetailResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RevokeApiKeyApiV1ApiKeysApiKeyIdDelete

> ApiKeyRevokeResponse RevokeApiKeyApiV1ApiKeysApiKeyIdDelete(ctx, apiKeyId).Execute()

Revoke Api Key

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
	apiKeyId := "apiKeyId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApiKeysAPI.RevokeApiKeyApiV1ApiKeysApiKeyIdDelete(context.Background(), apiKeyId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApiKeysAPI.RevokeApiKeyApiV1ApiKeysApiKeyIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RevokeApiKeyApiV1ApiKeysApiKeyIdDelete`: ApiKeyRevokeResponse
	fmt.Fprintf(os.Stdout, "Response from `ApiKeysAPI.RevokeApiKeyApiV1ApiKeysApiKeyIdDelete`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**apiKeyId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRevokeApiKeyApiV1ApiKeysApiKeyIdDeleteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**ApiKeyRevokeResponse**](ApiKeyRevokeResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RotateApiKeyApiV1ApiKeysApiKeyIdRotatePost

> ApiKeyRotateResponse RotateApiKeyApiV1ApiKeysApiKeyIdRotatePost(ctx, apiKeyId).Execute()

Rotate Api Key



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
	apiKeyId := "apiKeyId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApiKeysAPI.RotateApiKeyApiV1ApiKeysApiKeyIdRotatePost(context.Background(), apiKeyId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApiKeysAPI.RotateApiKeyApiV1ApiKeysApiKeyIdRotatePost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RotateApiKeyApiV1ApiKeysApiKeyIdRotatePost`: ApiKeyRotateResponse
	fmt.Fprintf(os.Stdout, "Response from `ApiKeysAPI.RotateApiKeyApiV1ApiKeysApiKeyIdRotatePost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**apiKeyId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRotateApiKeyApiV1ApiKeysApiKeyIdRotatePostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**ApiKeyRotateResponse**](ApiKeyRotateResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

