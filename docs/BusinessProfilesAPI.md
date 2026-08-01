# \BusinessProfilesAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateBusinessProfileApiV1BusinessProfilesPost**](BusinessProfilesAPI.md#CreateBusinessProfileApiV1BusinessProfilesPost) | **Post** /api/v1/business-profiles | Create Business Profile
[**DeleteBusinessProfileApiV1BusinessProfilesBusinessProfileIdDelete**](BusinessProfilesAPI.md#DeleteBusinessProfileApiV1BusinessProfilesBusinessProfileIdDelete) | **Delete** /api/v1/business-profiles/{business_profile_id} | Delete Business Profile
[**GetBusinessProfileApiV1BusinessProfilesBusinessProfileIdGet**](BusinessProfilesAPI.md#GetBusinessProfileApiV1BusinessProfilesBusinessProfileIdGet) | **Get** /api/v1/business-profiles/{business_profile_id} | Get Business Profile
[**ListBusinessProfilesApiV1BusinessProfilesGet**](BusinessProfilesAPI.md#ListBusinessProfilesApiV1BusinessProfilesGet) | **Get** /api/v1/business-profiles | List Business Profiles
[**PatchBusinessProfileApiV1BusinessProfilesBusinessProfileIdPatch**](BusinessProfilesAPI.md#PatchBusinessProfileApiV1BusinessProfilesBusinessProfileIdPatch) | **Patch** /api/v1/business-profiles/{business_profile_id} | Patch Business Profile



## CreateBusinessProfileApiV1BusinessProfilesPost

> BusinessProfileResponse CreateBusinessProfileApiV1BusinessProfilesPost(ctx).BusinessProfileCreate(businessProfileCreate).IdempotencyKey(idempotencyKey).Execute()

Create Business Profile

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
	businessProfileCreate := *openapiclient.NewBusinessProfileCreate("Acme Corp Inc.") // BusinessProfileCreate | 
	idempotencyKey := "idempotencyKey_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BusinessProfilesAPI.CreateBusinessProfileApiV1BusinessProfilesPost(context.Background()).BusinessProfileCreate(businessProfileCreate).IdempotencyKey(idempotencyKey).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BusinessProfilesAPI.CreateBusinessProfileApiV1BusinessProfilesPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateBusinessProfileApiV1BusinessProfilesPost`: BusinessProfileResponse
	fmt.Fprintf(os.Stdout, "Response from `BusinessProfilesAPI.CreateBusinessProfileApiV1BusinessProfilesPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateBusinessProfileApiV1BusinessProfilesPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **businessProfileCreate** | [**BusinessProfileCreate**](BusinessProfileCreate.md) |  | 
 **idempotencyKey** | **string** |  | 

### Return type

[**BusinessProfileResponse**](BusinessProfileResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteBusinessProfileApiV1BusinessProfilesBusinessProfileIdDelete

> SimpleBoolResponse DeleteBusinessProfileApiV1BusinessProfilesBusinessProfileIdDelete(ctx, businessProfileId).Execute()

Delete Business Profile

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
	businessProfileId := "businessProfileId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BusinessProfilesAPI.DeleteBusinessProfileApiV1BusinessProfilesBusinessProfileIdDelete(context.Background(), businessProfileId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BusinessProfilesAPI.DeleteBusinessProfileApiV1BusinessProfilesBusinessProfileIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteBusinessProfileApiV1BusinessProfilesBusinessProfileIdDelete`: SimpleBoolResponse
	fmt.Fprintf(os.Stdout, "Response from `BusinessProfilesAPI.DeleteBusinessProfileApiV1BusinessProfilesBusinessProfileIdDelete`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**businessProfileId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteBusinessProfileApiV1BusinessProfilesBusinessProfileIdDeleteRequest struct via the builder pattern


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


## GetBusinessProfileApiV1BusinessProfilesBusinessProfileIdGet

> BusinessProfileResponse GetBusinessProfileApiV1BusinessProfilesBusinessProfileIdGet(ctx, businessProfileId).Execute()

Get Business Profile

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
	businessProfileId := "businessProfileId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BusinessProfilesAPI.GetBusinessProfileApiV1BusinessProfilesBusinessProfileIdGet(context.Background(), businessProfileId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BusinessProfilesAPI.GetBusinessProfileApiV1BusinessProfilesBusinessProfileIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetBusinessProfileApiV1BusinessProfilesBusinessProfileIdGet`: BusinessProfileResponse
	fmt.Fprintf(os.Stdout, "Response from `BusinessProfilesAPI.GetBusinessProfileApiV1BusinessProfilesBusinessProfileIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**businessProfileId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetBusinessProfileApiV1BusinessProfilesBusinessProfileIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**BusinessProfileResponse**](BusinessProfileResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListBusinessProfilesApiV1BusinessProfilesGet

> BusinessProfilesListResponse ListBusinessProfilesApiV1BusinessProfilesGet(ctx).Limit(limit).Cursor(cursor).Execute()

List Business Profiles

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BusinessProfilesAPI.ListBusinessProfilesApiV1BusinessProfilesGet(context.Background()).Limit(limit).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BusinessProfilesAPI.ListBusinessProfilesApiV1BusinessProfilesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListBusinessProfilesApiV1BusinessProfilesGet`: BusinessProfilesListResponse
	fmt.Fprintf(os.Stdout, "Response from `BusinessProfilesAPI.ListBusinessProfilesApiV1BusinessProfilesGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListBusinessProfilesApiV1BusinessProfilesGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int32** |  | [default to 50]
 **cursor** | **string** |  | 

### Return type

[**BusinessProfilesListResponse**](BusinessProfilesListResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PatchBusinessProfileApiV1BusinessProfilesBusinessProfileIdPatch

> BusinessProfileResponse PatchBusinessProfileApiV1BusinessProfilesBusinessProfileIdPatch(ctx, businessProfileId).BusinessProfilePatch(businessProfilePatch).IdempotencyKey(idempotencyKey).Execute()

Patch Business Profile

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
	businessProfileId := "businessProfileId_example" // string | 
	businessProfilePatch := *openapiclient.NewBusinessProfilePatch() // BusinessProfilePatch | 
	idempotencyKey := "idempotencyKey_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BusinessProfilesAPI.PatchBusinessProfileApiV1BusinessProfilesBusinessProfileIdPatch(context.Background(), businessProfileId).BusinessProfilePatch(businessProfilePatch).IdempotencyKey(idempotencyKey).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BusinessProfilesAPI.PatchBusinessProfileApiV1BusinessProfilesBusinessProfileIdPatch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PatchBusinessProfileApiV1BusinessProfilesBusinessProfileIdPatch`: BusinessProfileResponse
	fmt.Fprintf(os.Stdout, "Response from `BusinessProfilesAPI.PatchBusinessProfileApiV1BusinessProfilesBusinessProfileIdPatch`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**businessProfileId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiPatchBusinessProfileApiV1BusinessProfilesBusinessProfileIdPatchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **businessProfilePatch** | [**BusinessProfilePatch**](BusinessProfilePatch.md) |  | 
 **idempotencyKey** | **string** |  | 

### Return type

[**BusinessProfileResponse**](BusinessProfileResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

