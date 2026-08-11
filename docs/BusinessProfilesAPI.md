# \BusinessProfilesAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateBusinessProfile**](BusinessProfilesAPI.md#CreateBusinessProfile) | **Post** /api/v1/business-profiles | Create Business Profile
[**DeleteBusinessProfile**](BusinessProfilesAPI.md#DeleteBusinessProfile) | **Delete** /api/v1/business-profiles/{business_profile_id} | Delete Business Profile
[**GetBusinessProfile**](BusinessProfilesAPI.md#GetBusinessProfile) | **Get** /api/v1/business-profiles/{business_profile_id} | Get Business Profile
[**ListBusinessProfiles**](BusinessProfilesAPI.md#ListBusinessProfiles) | **Get** /api/v1/business-profiles | List Business Profiles
[**UpdateBusinessProfile**](BusinessProfilesAPI.md#UpdateBusinessProfile) | **Patch** /api/v1/business-profiles/{business_profile_id} | Update Business Profile



## CreateBusinessProfile

> BusinessProfileResponse CreateBusinessProfile(ctx).BusinessProfileCreate(businessProfileCreate).IdempotencyKey(idempotencyKey).Execute()

Create Business Profile

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
	businessProfileCreate := *openapiclient.NewBusinessProfileCreate("Acme Corp Inc.") // BusinessProfileCreate | 
	idempotencyKey := "idempotencyKey_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BusinessProfilesAPI.CreateBusinessProfile(context.Background()).BusinessProfileCreate(businessProfileCreate).IdempotencyKey(idempotencyKey).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BusinessProfilesAPI.CreateBusinessProfile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateBusinessProfile`: BusinessProfileResponse
	fmt.Fprintf(os.Stdout, "Response from `BusinessProfilesAPI.CreateBusinessProfile`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateBusinessProfileRequest struct via the builder pattern


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


## DeleteBusinessProfile

> SimpleBoolResponse DeleteBusinessProfile(ctx, businessProfileId).Execute()

Delete Business Profile

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
	businessProfileId := "businessProfileId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BusinessProfilesAPI.DeleteBusinessProfile(context.Background(), businessProfileId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BusinessProfilesAPI.DeleteBusinessProfile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteBusinessProfile`: SimpleBoolResponse
	fmt.Fprintf(os.Stdout, "Response from `BusinessProfilesAPI.DeleteBusinessProfile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**businessProfileId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteBusinessProfileRequest struct via the builder pattern


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


## GetBusinessProfile

> BusinessProfileResponse GetBusinessProfile(ctx, businessProfileId).Execute()

Get Business Profile

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
	businessProfileId := "businessProfileId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BusinessProfilesAPI.GetBusinessProfile(context.Background(), businessProfileId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BusinessProfilesAPI.GetBusinessProfile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetBusinessProfile`: BusinessProfileResponse
	fmt.Fprintf(os.Stdout, "Response from `BusinessProfilesAPI.GetBusinessProfile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**businessProfileId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetBusinessProfileRequest struct via the builder pattern


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


## ListBusinessProfiles

> BusinessProfilesListResponse ListBusinessProfiles(ctx).Limit(limit).Cursor(cursor).Execute()

List Business Profiles

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
	resp, r, err := apiClient.BusinessProfilesAPI.ListBusinessProfiles(context.Background()).Limit(limit).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BusinessProfilesAPI.ListBusinessProfiles``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListBusinessProfiles`: BusinessProfilesListResponse
	fmt.Fprintf(os.Stdout, "Response from `BusinessProfilesAPI.ListBusinessProfiles`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListBusinessProfilesRequest struct via the builder pattern


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


## UpdateBusinessProfile

> BusinessProfileResponse UpdateBusinessProfile(ctx, businessProfileId).BusinessProfilePatch(businessProfilePatch).IdempotencyKey(idempotencyKey).Execute()

Update Business Profile

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
	businessProfileId := "businessProfileId_example" // string | 
	businessProfilePatch := *openapiclient.NewBusinessProfilePatch() // BusinessProfilePatch | 
	idempotencyKey := "idempotencyKey_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BusinessProfilesAPI.UpdateBusinessProfile(context.Background(), businessProfileId).BusinessProfilePatch(businessProfilePatch).IdempotencyKey(idempotencyKey).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BusinessProfilesAPI.UpdateBusinessProfile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateBusinessProfile`: BusinessProfileResponse
	fmt.Fprintf(os.Stdout, "Response from `BusinessProfilesAPI.UpdateBusinessProfile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**businessProfileId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateBusinessProfileRequest struct via the builder pattern


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

