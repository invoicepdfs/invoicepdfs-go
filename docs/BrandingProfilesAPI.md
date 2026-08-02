# \BrandingProfilesAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateProfileApiV1BrandingProfilesPost**](BrandingProfilesAPI.md#CreateProfileApiV1BrandingProfilesPost) | **Post** /api/v1/branding-profiles | Create Profile
[**DeleteLogoApiV1BrandingProfilesProfileIdLogoDelete**](BrandingProfilesAPI.md#DeleteLogoApiV1BrandingProfilesProfileIdLogoDelete) | **Delete** /api/v1/branding-profiles/{profile_id}/logo | Delete Logo
[**DeleteProfileApiV1BrandingProfilesProfileIdDelete**](BrandingProfilesAPI.md#DeleteProfileApiV1BrandingProfilesProfileIdDelete) | **Delete** /api/v1/branding-profiles/{profile_id} | Delete Profile
[**GetProfileApiV1BrandingProfilesProfileIdGet**](BrandingProfilesAPI.md#GetProfileApiV1BrandingProfilesProfileIdGet) | **Get** /api/v1/branding-profiles/{profile_id} | Get Profile
[**ListProfilesApiV1BrandingProfilesGet**](BrandingProfilesAPI.md#ListProfilesApiV1BrandingProfilesGet) | **Get** /api/v1/branding-profiles | List Profiles
[**SetDefaultApiV1BrandingProfilesProfileIdDefaultPost**](BrandingProfilesAPI.md#SetDefaultApiV1BrandingProfilesProfileIdDefaultPost) | **Post** /api/v1/branding-profiles/{profile_id}/default | Set Default
[**UpdateProfileApiV1BrandingProfilesProfileIdPatch**](BrandingProfilesAPI.md#UpdateProfileApiV1BrandingProfilesProfileIdPatch) | **Patch** /api/v1/branding-profiles/{profile_id} | Update Profile
[**UploadLogoApiV1BrandingProfilesProfileIdLogoPost**](BrandingProfilesAPI.md#UploadLogoApiV1BrandingProfilesProfileIdLogoPost) | **Post** /api/v1/branding-profiles/{profile_id}/logo | Upload Logo



## CreateProfileApiV1BrandingProfilesPost

> BrandingProfileResponse CreateProfileApiV1BrandingProfilesPost(ctx).BrandingProfileCreateRequest(brandingProfileCreateRequest).Execute()

Create Profile

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
	brandingProfileCreateRequest := *openapiclient.NewBrandingProfileCreateRequest("Acme Corp") // BrandingProfileCreateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BrandingProfilesAPI.CreateProfileApiV1BrandingProfilesPost(context.Background()).BrandingProfileCreateRequest(brandingProfileCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BrandingProfilesAPI.CreateProfileApiV1BrandingProfilesPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateProfileApiV1BrandingProfilesPost`: BrandingProfileResponse
	fmt.Fprintf(os.Stdout, "Response from `BrandingProfilesAPI.CreateProfileApiV1BrandingProfilesPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateProfileApiV1BrandingProfilesPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **brandingProfileCreateRequest** | [**BrandingProfileCreateRequest**](BrandingProfileCreateRequest.md) |  | 

### Return type

[**BrandingProfileResponse**](BrandingProfileResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteLogoApiV1BrandingProfilesProfileIdLogoDelete

> SimpleBoolResponse DeleteLogoApiV1BrandingProfilesProfileIdLogoDelete(ctx, profileId).Execute()

Delete Logo

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
	profileId := "profileId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BrandingProfilesAPI.DeleteLogoApiV1BrandingProfilesProfileIdLogoDelete(context.Background(), profileId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BrandingProfilesAPI.DeleteLogoApiV1BrandingProfilesProfileIdLogoDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteLogoApiV1BrandingProfilesProfileIdLogoDelete`: SimpleBoolResponse
	fmt.Fprintf(os.Stdout, "Response from `BrandingProfilesAPI.DeleteLogoApiV1BrandingProfilesProfileIdLogoDelete`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**profileId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteLogoApiV1BrandingProfilesProfileIdLogoDeleteRequest struct via the builder pattern


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


## DeleteProfileApiV1BrandingProfilesProfileIdDelete

> SimpleBoolResponse DeleteProfileApiV1BrandingProfilesProfileIdDelete(ctx, profileId).Execute()

Delete Profile

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
	profileId := "profileId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BrandingProfilesAPI.DeleteProfileApiV1BrandingProfilesProfileIdDelete(context.Background(), profileId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BrandingProfilesAPI.DeleteProfileApiV1BrandingProfilesProfileIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteProfileApiV1BrandingProfilesProfileIdDelete`: SimpleBoolResponse
	fmt.Fprintf(os.Stdout, "Response from `BrandingProfilesAPI.DeleteProfileApiV1BrandingProfilesProfileIdDelete`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**profileId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteProfileApiV1BrandingProfilesProfileIdDeleteRequest struct via the builder pattern


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


## GetProfileApiV1BrandingProfilesProfileIdGet

> BrandingProfileResponse GetProfileApiV1BrandingProfilesProfileIdGet(ctx, profileId).Execute()

Get Profile

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
	profileId := "profileId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BrandingProfilesAPI.GetProfileApiV1BrandingProfilesProfileIdGet(context.Background(), profileId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BrandingProfilesAPI.GetProfileApiV1BrandingProfilesProfileIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetProfileApiV1BrandingProfilesProfileIdGet`: BrandingProfileResponse
	fmt.Fprintf(os.Stdout, "Response from `BrandingProfilesAPI.GetProfileApiV1BrandingProfilesProfileIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**profileId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetProfileApiV1BrandingProfilesProfileIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**BrandingProfileResponse**](BrandingProfileResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListProfilesApiV1BrandingProfilesGet

> BrandingProfilesListResponse ListProfilesApiV1BrandingProfilesGet(ctx).Execute()

List Profiles

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BrandingProfilesAPI.ListProfilesApiV1BrandingProfilesGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BrandingProfilesAPI.ListProfilesApiV1BrandingProfilesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListProfilesApiV1BrandingProfilesGet`: BrandingProfilesListResponse
	fmt.Fprintf(os.Stdout, "Response from `BrandingProfilesAPI.ListProfilesApiV1BrandingProfilesGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListProfilesApiV1BrandingProfilesGetRequest struct via the builder pattern


### Return type

[**BrandingProfilesListResponse**](BrandingProfilesListResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SetDefaultApiV1BrandingProfilesProfileIdDefaultPost

> BrandingProfileResponse SetDefaultApiV1BrandingProfilesProfileIdDefaultPost(ctx, profileId).Execute()

Set Default

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
	profileId := "profileId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BrandingProfilesAPI.SetDefaultApiV1BrandingProfilesProfileIdDefaultPost(context.Background(), profileId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BrandingProfilesAPI.SetDefaultApiV1BrandingProfilesProfileIdDefaultPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SetDefaultApiV1BrandingProfilesProfileIdDefaultPost`: BrandingProfileResponse
	fmt.Fprintf(os.Stdout, "Response from `BrandingProfilesAPI.SetDefaultApiV1BrandingProfilesProfileIdDefaultPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**profileId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiSetDefaultApiV1BrandingProfilesProfileIdDefaultPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**BrandingProfileResponse**](BrandingProfileResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateProfileApiV1BrandingProfilesProfileIdPatch

> BrandingProfileResponse UpdateProfileApiV1BrandingProfilesProfileIdPatch(ctx, profileId).BrandingProfilePatchRequest(brandingProfilePatchRequest).Execute()

Update Profile

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
	profileId := "profileId_example" // string | 
	brandingProfilePatchRequest := *openapiclient.NewBrandingProfilePatchRequest() // BrandingProfilePatchRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BrandingProfilesAPI.UpdateProfileApiV1BrandingProfilesProfileIdPatch(context.Background(), profileId).BrandingProfilePatchRequest(brandingProfilePatchRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BrandingProfilesAPI.UpdateProfileApiV1BrandingProfilesProfileIdPatch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateProfileApiV1BrandingProfilesProfileIdPatch`: BrandingProfileResponse
	fmt.Fprintf(os.Stdout, "Response from `BrandingProfilesAPI.UpdateProfileApiV1BrandingProfilesProfileIdPatch`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**profileId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateProfileApiV1BrandingProfilesProfileIdPatchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **brandingProfilePatchRequest** | [**BrandingProfilePatchRequest**](BrandingProfilePatchRequest.md) |  | 

### Return type

[**BrandingProfileResponse**](BrandingProfileResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UploadLogoApiV1BrandingProfilesProfileIdLogoPost

> BrandingProfileResponse UploadLogoApiV1BrandingProfilesProfileIdLogoPost(ctx, profileId).File(file).Execute()

Upload Logo

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
	profileId := "profileId_example" // string | 
	file := os.NewFile(1234, "some_file") // *os.File | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BrandingProfilesAPI.UploadLogoApiV1BrandingProfilesProfileIdLogoPost(context.Background(), profileId).File(file).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BrandingProfilesAPI.UploadLogoApiV1BrandingProfilesProfileIdLogoPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UploadLogoApiV1BrandingProfilesProfileIdLogoPost`: BrandingProfileResponse
	fmt.Fprintf(os.Stdout, "Response from `BrandingProfilesAPI.UploadLogoApiV1BrandingProfilesProfileIdLogoPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**profileId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUploadLogoApiV1BrandingProfilesProfileIdLogoPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **file** | ***os.File** |  | 

### Return type

[**BrandingProfileResponse**](BrandingProfileResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

