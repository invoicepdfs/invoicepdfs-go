# \TemplateVersionsAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateTemplateVersionApiV1TemplatesTemplateIdVersionsPost**](TemplateVersionsAPI.md#CreateTemplateVersionApiV1TemplatesTemplateIdVersionsPost) | **Post** /api/v1/templates/{template_id}/versions | Create Template Version
[**GetTemplateVersionApiV1TemplatesTemplateIdVersionsVersionGet**](TemplateVersionsAPI.md#GetTemplateVersionApiV1TemplatesTemplateIdVersionsVersionGet) | **Get** /api/v1/templates/{template_id}/versions/{version} | Get Template Version
[**ListTemplateVersionsApiV1TemplatesTemplateIdVersionsGet**](TemplateVersionsAPI.md#ListTemplateVersionsApiV1TemplatesTemplateIdVersionsGet) | **Get** /api/v1/templates/{template_id}/versions | List Template Versions



## CreateTemplateVersionApiV1TemplatesTemplateIdVersionsPost

> TemplateVersionResponse CreateTemplateVersionApiV1TemplatesTemplateIdVersionsPost(ctx, templateId).TemplateVersionCreateRequest(templateVersionCreateRequest).Execute()

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
	resp, r, err := apiClient.TemplateVersionsAPI.CreateTemplateVersionApiV1TemplatesTemplateIdVersionsPost(context.Background(), templateId).TemplateVersionCreateRequest(templateVersionCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TemplateVersionsAPI.CreateTemplateVersionApiV1TemplatesTemplateIdVersionsPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateTemplateVersionApiV1TemplatesTemplateIdVersionsPost`: TemplateVersionResponse
	fmt.Fprintf(os.Stdout, "Response from `TemplateVersionsAPI.CreateTemplateVersionApiV1TemplatesTemplateIdVersionsPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateTemplateVersionApiV1TemplatesTemplateIdVersionsPostRequest struct via the builder pattern


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


## GetTemplateVersionApiV1TemplatesTemplateIdVersionsVersionGet

> TemplateVersionResponse GetTemplateVersionApiV1TemplatesTemplateIdVersionsVersionGet(ctx, templateId, version).Execute()

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
	resp, r, err := apiClient.TemplateVersionsAPI.GetTemplateVersionApiV1TemplatesTemplateIdVersionsVersionGet(context.Background(), templateId, version).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TemplateVersionsAPI.GetTemplateVersionApiV1TemplatesTemplateIdVersionsVersionGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetTemplateVersionApiV1TemplatesTemplateIdVersionsVersionGet`: TemplateVersionResponse
	fmt.Fprintf(os.Stdout, "Response from `TemplateVersionsAPI.GetTemplateVersionApiV1TemplatesTemplateIdVersionsVersionGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** |  | 
**version** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetTemplateVersionApiV1TemplatesTemplateIdVersionsVersionGetRequest struct via the builder pattern


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


## ListTemplateVersionsApiV1TemplatesTemplateIdVersionsGet

> TemplateVersionsListResponse ListTemplateVersionsApiV1TemplatesTemplateIdVersionsGet(ctx, templateId).Execute()

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
	resp, r, err := apiClient.TemplateVersionsAPI.ListTemplateVersionsApiV1TemplatesTemplateIdVersionsGet(context.Background(), templateId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TemplateVersionsAPI.ListTemplateVersionsApiV1TemplatesTemplateIdVersionsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListTemplateVersionsApiV1TemplatesTemplateIdVersionsGet`: TemplateVersionsListResponse
	fmt.Fprintf(os.Stdout, "Response from `TemplateVersionsAPI.ListTemplateVersionsApiV1TemplatesTemplateIdVersionsGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListTemplateVersionsApiV1TemplatesTemplateIdVersionsGetRequest struct via the builder pattern


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

