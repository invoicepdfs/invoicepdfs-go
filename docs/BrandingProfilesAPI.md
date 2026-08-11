# \BrandingProfilesAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateBrandingProfile**](BrandingProfilesAPI.md#CreateBrandingProfile) | **Post** /api/v1/branding-profiles | Create Branding Profile
[**DeleteBrandingLogo**](BrandingProfilesAPI.md#DeleteBrandingLogo) | **Delete** /api/v1/branding-profiles/{profile_id}/logo | Delete Branding Logo
[**DeleteBrandingProfile**](BrandingProfilesAPI.md#DeleteBrandingProfile) | **Delete** /api/v1/branding-profiles/{profile_id} | Delete Branding Profile
[**GetBrandingProfile**](BrandingProfilesAPI.md#GetBrandingProfile) | **Get** /api/v1/branding-profiles/{profile_id} | Get Branding Profile
[**ListBrandingProfiles**](BrandingProfilesAPI.md#ListBrandingProfiles) | **Get** /api/v1/branding-profiles | List Branding Profiles
[**SetDefaultBrandingProfile**](BrandingProfilesAPI.md#SetDefaultBrandingProfile) | **Post** /api/v1/branding-profiles/{profile_id}/default | Set Default Branding Profile
[**UpdateBrandingProfile**](BrandingProfilesAPI.md#UpdateBrandingProfile) | **Patch** /api/v1/branding-profiles/{profile_id} | Update Branding Profile
[**UploadBrandingLogo**](BrandingProfilesAPI.md#UploadBrandingLogo) | **Post** /api/v1/branding-profiles/{profile_id}/logo | Upload Branding Logo



## CreateBrandingProfile

> BrandingProfileResponse CreateBrandingProfile(ctx).BrandingProfileCreateRequest(brandingProfileCreateRequest).Execute()

Create Branding Profile

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
	resp, r, err := apiClient.BrandingProfilesAPI.CreateBrandingProfile(context.Background()).BrandingProfileCreateRequest(brandingProfileCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BrandingProfilesAPI.CreateBrandingProfile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateBrandingProfile`: BrandingProfileResponse
	fmt.Fprintf(os.Stdout, "Response from `BrandingProfilesAPI.CreateBrandingProfile`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateBrandingProfileRequest struct via the builder pattern


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


## DeleteBrandingLogo

> SimpleBoolResponse DeleteBrandingLogo(ctx, profileId).Execute()

Delete Branding Logo

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
	resp, r, err := apiClient.BrandingProfilesAPI.DeleteBrandingLogo(context.Background(), profileId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BrandingProfilesAPI.DeleteBrandingLogo``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteBrandingLogo`: SimpleBoolResponse
	fmt.Fprintf(os.Stdout, "Response from `BrandingProfilesAPI.DeleteBrandingLogo`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**profileId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteBrandingLogoRequest struct via the builder pattern


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


## DeleteBrandingProfile

> SimpleBoolResponse DeleteBrandingProfile(ctx, profileId).Execute()

Delete Branding Profile

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
	resp, r, err := apiClient.BrandingProfilesAPI.DeleteBrandingProfile(context.Background(), profileId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BrandingProfilesAPI.DeleteBrandingProfile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteBrandingProfile`: SimpleBoolResponse
	fmt.Fprintf(os.Stdout, "Response from `BrandingProfilesAPI.DeleteBrandingProfile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**profileId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteBrandingProfileRequest struct via the builder pattern


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


## GetBrandingProfile

> BrandingProfileResponse GetBrandingProfile(ctx, profileId).Execute()

Get Branding Profile

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
	resp, r, err := apiClient.BrandingProfilesAPI.GetBrandingProfile(context.Background(), profileId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BrandingProfilesAPI.GetBrandingProfile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetBrandingProfile`: BrandingProfileResponse
	fmt.Fprintf(os.Stdout, "Response from `BrandingProfilesAPI.GetBrandingProfile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**profileId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetBrandingProfileRequest struct via the builder pattern


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


## ListBrandingProfiles

> BrandingProfilesListResponse ListBrandingProfiles(ctx).Execute()

List Branding Profiles

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
	resp, r, err := apiClient.BrandingProfilesAPI.ListBrandingProfiles(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BrandingProfilesAPI.ListBrandingProfiles``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListBrandingProfiles`: BrandingProfilesListResponse
	fmt.Fprintf(os.Stdout, "Response from `BrandingProfilesAPI.ListBrandingProfiles`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListBrandingProfilesRequest struct via the builder pattern


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


## SetDefaultBrandingProfile

> BrandingProfileResponse SetDefaultBrandingProfile(ctx, profileId).Execute()

Set Default Branding Profile

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
	resp, r, err := apiClient.BrandingProfilesAPI.SetDefaultBrandingProfile(context.Background(), profileId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BrandingProfilesAPI.SetDefaultBrandingProfile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SetDefaultBrandingProfile`: BrandingProfileResponse
	fmt.Fprintf(os.Stdout, "Response from `BrandingProfilesAPI.SetDefaultBrandingProfile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**profileId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiSetDefaultBrandingProfileRequest struct via the builder pattern


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


## UpdateBrandingProfile

> BrandingProfileResponse UpdateBrandingProfile(ctx, profileId).BrandingProfilePatchRequest(brandingProfilePatchRequest).Execute()

Update Branding Profile

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
	resp, r, err := apiClient.BrandingProfilesAPI.UpdateBrandingProfile(context.Background(), profileId).BrandingProfilePatchRequest(brandingProfilePatchRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BrandingProfilesAPI.UpdateBrandingProfile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateBrandingProfile`: BrandingProfileResponse
	fmt.Fprintf(os.Stdout, "Response from `BrandingProfilesAPI.UpdateBrandingProfile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**profileId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateBrandingProfileRequest struct via the builder pattern


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


## UploadBrandingLogo

> BrandingProfileResponse UploadBrandingLogo(ctx, profileId).File(file).Execute()

Upload Branding Logo

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
	resp, r, err := apiClient.BrandingProfilesAPI.UploadBrandingLogo(context.Background(), profileId).File(file).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BrandingProfilesAPI.UploadBrandingLogo``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UploadBrandingLogo`: BrandingProfileResponse
	fmt.Fprintf(os.Stdout, "Response from `BrandingProfilesAPI.UploadBrandingLogo`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**profileId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUploadBrandingLogoRequest struct via the builder pattern


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

