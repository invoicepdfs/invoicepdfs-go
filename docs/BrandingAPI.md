# \BrandingAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**DeleteLogoApiV1BrandingLogoDelete**](BrandingAPI.md#DeleteLogoApiV1BrandingLogoDelete) | **Delete** /api/v1/branding/logo | Delete Logo
[**GetBrandingApiV1BrandingGet**](BrandingAPI.md#GetBrandingApiV1BrandingGet) | **Get** /api/v1/branding | Get Branding
[**UpdateBrandingApiV1BrandingPut**](BrandingAPI.md#UpdateBrandingApiV1BrandingPut) | **Put** /api/v1/branding | Update Branding
[**UploadLogoApiV1BrandingLogoPost**](BrandingAPI.md#UploadLogoApiV1BrandingLogoPost) | **Post** /api/v1/branding/logo | Upload Logo



## DeleteLogoApiV1BrandingLogoDelete

> SimpleBoolResponse DeleteLogoApiV1BrandingLogoDelete(ctx).Execute()

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BrandingAPI.DeleteLogoApiV1BrandingLogoDelete(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BrandingAPI.DeleteLogoApiV1BrandingLogoDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteLogoApiV1BrandingLogoDelete`: SimpleBoolResponse
	fmt.Fprintf(os.Stdout, "Response from `BrandingAPI.DeleteLogoApiV1BrandingLogoDelete`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteLogoApiV1BrandingLogoDeleteRequest struct via the builder pattern


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


## GetBrandingApiV1BrandingGet

> BrandingResponse GetBrandingApiV1BrandingGet(ctx).Execute()

Get Branding

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
	resp, r, err := apiClient.BrandingAPI.GetBrandingApiV1BrandingGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BrandingAPI.GetBrandingApiV1BrandingGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetBrandingApiV1BrandingGet`: BrandingResponse
	fmt.Fprintf(os.Stdout, "Response from `BrandingAPI.GetBrandingApiV1BrandingGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetBrandingApiV1BrandingGetRequest struct via the builder pattern


### Return type

[**BrandingResponse**](BrandingResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateBrandingApiV1BrandingPut

> BrandingResponse UpdateBrandingApiV1BrandingPut(ctx).BrandingUpdateRequest(brandingUpdateRequest).Execute()

Update Branding

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
	brandingUpdateRequest := *openapiclient.NewBrandingUpdateRequest() // BrandingUpdateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BrandingAPI.UpdateBrandingApiV1BrandingPut(context.Background()).BrandingUpdateRequest(brandingUpdateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BrandingAPI.UpdateBrandingApiV1BrandingPut``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateBrandingApiV1BrandingPut`: BrandingResponse
	fmt.Fprintf(os.Stdout, "Response from `BrandingAPI.UpdateBrandingApiV1BrandingPut`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiUpdateBrandingApiV1BrandingPutRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **brandingUpdateRequest** | [**BrandingUpdateRequest**](BrandingUpdateRequest.md) |  | 

### Return type

[**BrandingResponse**](BrandingResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UploadLogoApiV1BrandingLogoPost

> BrandingResponse UploadLogoApiV1BrandingLogoPost(ctx).File(file).Execute()

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
	file := os.NewFile(1234, "some_file") // *os.File | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BrandingAPI.UploadLogoApiV1BrandingLogoPost(context.Background()).File(file).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BrandingAPI.UploadLogoApiV1BrandingLogoPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UploadLogoApiV1BrandingLogoPost`: BrandingResponse
	fmt.Fprintf(os.Stdout, "Response from `BrandingAPI.UploadLogoApiV1BrandingLogoPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiUploadLogoApiV1BrandingLogoPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **file** | ***os.File** |  | 

### Return type

[**BrandingResponse**](BrandingResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

