# \TemplateVersionsAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateTemplateVersion**](TemplateVersionsAPI.md#CreateTemplateVersion) | **Post** /api/v1/templates/{template_id}/versions | Create Template Version
[**GetTemplateVersion**](TemplateVersionsAPI.md#GetTemplateVersion) | **Get** /api/v1/templates/{template_id}/versions/{version} | Get Template Version
[**ListTemplateVersions**](TemplateVersionsAPI.md#ListTemplateVersions) | **Get** /api/v1/templates/{template_id}/versions | List Template Versions



## CreateTemplateVersion

> TemplateVersionResponse CreateTemplateVersion(ctx, templateId).TemplateVersionCreateRequest(templateVersionCreateRequest).Execute()

Create Template Version

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
	templateId := "templateId_example" // string | 
	templateVersionCreateRequest := *openapiclient.NewTemplateVersionCreateRequest() // TemplateVersionCreateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TemplateVersionsAPI.CreateTemplateVersion(context.Background(), templateId).TemplateVersionCreateRequest(templateVersionCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TemplateVersionsAPI.CreateTemplateVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateTemplateVersion`: TemplateVersionResponse
	fmt.Fprintf(os.Stdout, "Response from `TemplateVersionsAPI.CreateTemplateVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateTemplateVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **templateVersionCreateRequest** | [**TemplateVersionCreateRequest**](TemplateVersionCreateRequest.md) |  | 

### Return type

[**TemplateVersionResponse**](TemplateVersionResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetTemplateVersion

> TemplateVersionResponse GetTemplateVersion(ctx, templateId, version).Execute()

Get Template Version

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
	templateId := "templateId_example" // string | 
	version := int32(56) // int32 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TemplateVersionsAPI.GetTemplateVersion(context.Background(), templateId, version).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TemplateVersionsAPI.GetTemplateVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetTemplateVersion`: TemplateVersionResponse
	fmt.Fprintf(os.Stdout, "Response from `TemplateVersionsAPI.GetTemplateVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** |  | 
**version** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetTemplateVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**TemplateVersionResponse**](TemplateVersionResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListTemplateVersions

> TemplateVersionsListResponse ListTemplateVersions(ctx, templateId).Execute()

List Template Versions

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
	templateId := "templateId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TemplateVersionsAPI.ListTemplateVersions(context.Background(), templateId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TemplateVersionsAPI.ListTemplateVersions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListTemplateVersions`: TemplateVersionsListResponse
	fmt.Fprintf(os.Stdout, "Response from `TemplateVersionsAPI.ListTemplateVersions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListTemplateVersionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**TemplateVersionsListResponse**](TemplateVersionsListResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

