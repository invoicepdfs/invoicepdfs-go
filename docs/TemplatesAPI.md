# \TemplatesAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateTemplateApiV1TemplatesCustomPost**](TemplatesAPI.md#CreateTemplateApiV1TemplatesCustomPost) | **Post** /api/v1/templates/custom | Create Template
[**DeleteTemplateApiV1TemplatesCustomTemplateIdDelete**](TemplatesAPI.md#DeleteTemplateApiV1TemplatesCustomTemplateIdDelete) | **Delete** /api/v1/templates/custom/{template_id} | Delete Template
[**DuplicateTemplateApiV1TemplatesCustomTemplateIdDuplicatePost**](TemplatesAPI.md#DuplicateTemplateApiV1TemplatesCustomTemplateIdDuplicatePost) | **Post** /api/v1/templates/custom/{template_id}/duplicate | Duplicate Template
[**GetBuiltinTemplateApiV1TemplatesBuiltinTemplateIdGet**](TemplatesAPI.md#GetBuiltinTemplateApiV1TemplatesBuiltinTemplateIdGet) | **Get** /api/v1/templates/builtin/{template_id} | Get Builtin Template
[**GetCustomTemplateApiV1TemplatesCustomTemplateIdGet**](TemplatesAPI.md#GetCustomTemplateApiV1TemplatesCustomTemplateIdGet) | **Get** /api/v1/templates/custom/{template_id} | Get Custom Template
[**GetTemplateApiV1TemplatesTemplateIdGet**](TemplatesAPI.md#GetTemplateApiV1TemplatesTemplateIdGet) | **Get** /api/v1/templates/{template_id} | Get Template
[**ListCustomTemplatesApiV1TemplatesCustomGet**](TemplatesAPI.md#ListCustomTemplatesApiV1TemplatesCustomGet) | **Get** /api/v1/templates/custom | List Custom Templates
[**PatchTemplateApiV1TemplatesCustomTemplateIdPatch**](TemplatesAPI.md#PatchTemplateApiV1TemplatesCustomTemplateIdPatch) | **Patch** /api/v1/templates/custom/{template_id} | Patch Template
[**PreviewTemplateApiV1TemplatesTemplateIdPreviewPost**](TemplatesAPI.md#PreviewTemplateApiV1TemplatesTemplateIdPreviewPost) | **Post** /api/v1/templates/{template_id}/preview | Preview Template
[**PublishTemplateApiV1TemplatesCustomTemplateIdPublishPost**](TemplatesAPI.md#PublishTemplateApiV1TemplatesCustomTemplateIdPublishPost) | **Post** /api/v1/templates/custom/{template_id}/publish | Publish Template
[**TemplatesApiV1TemplatesGet**](TemplatesAPI.md#TemplatesApiV1TemplatesGet) | **Get** /api/v1/templates | Templates



## CreateTemplateApiV1TemplatesCustomPost

> CustomTemplateResponse CreateTemplateApiV1TemplatesCustomPost(ctx).TemplateCreateRequest(templateCreateRequest).Execute()

Create Template

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
	templateCreateRequest := *openapiclient.NewTemplateCreateRequest("Name_example") // TemplateCreateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TemplatesAPI.CreateTemplateApiV1TemplatesCustomPost(context.Background()).TemplateCreateRequest(templateCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TemplatesAPI.CreateTemplateApiV1TemplatesCustomPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateTemplateApiV1TemplatesCustomPost`: CustomTemplateResponse
	fmt.Fprintf(os.Stdout, "Response from `TemplatesAPI.CreateTemplateApiV1TemplatesCustomPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateTemplateApiV1TemplatesCustomPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **templateCreateRequest** | [**TemplateCreateRequest**](TemplateCreateRequest.md) |  | 

### Return type

[**CustomTemplateResponse**](CustomTemplateResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteTemplateApiV1TemplatesCustomTemplateIdDelete

> DeleteTemplateApiV1TemplatesCustomTemplateIdDelete(ctx, templateId).Execute()

Delete Template

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
	r, err := apiClient.TemplatesAPI.DeleteTemplateApiV1TemplatesCustomTemplateIdDelete(context.Background(), templateId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TemplatesAPI.DeleteTemplateApiV1TemplatesCustomTemplateIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteTemplateApiV1TemplatesCustomTemplateIdDeleteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

 (empty response body)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DuplicateTemplateApiV1TemplatesCustomTemplateIdDuplicatePost

> CustomTemplateResponse DuplicateTemplateApiV1TemplatesCustomTemplateIdDuplicatePost(ctx, templateId).Execute()

Duplicate Template

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
	resp, r, err := apiClient.TemplatesAPI.DuplicateTemplateApiV1TemplatesCustomTemplateIdDuplicatePost(context.Background(), templateId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TemplatesAPI.DuplicateTemplateApiV1TemplatesCustomTemplateIdDuplicatePost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DuplicateTemplateApiV1TemplatesCustomTemplateIdDuplicatePost`: CustomTemplateResponse
	fmt.Fprintf(os.Stdout, "Response from `TemplatesAPI.DuplicateTemplateApiV1TemplatesCustomTemplateIdDuplicatePost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDuplicateTemplateApiV1TemplatesCustomTemplateIdDuplicatePostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**CustomTemplateResponse**](CustomTemplateResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetBuiltinTemplateApiV1TemplatesBuiltinTemplateIdGet

> TemplateDetailResponse GetBuiltinTemplateApiV1TemplatesBuiltinTemplateIdGet(ctx, templateId).Execute()

Get Builtin Template

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
	resp, r, err := apiClient.TemplatesAPI.GetBuiltinTemplateApiV1TemplatesBuiltinTemplateIdGet(context.Background(), templateId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TemplatesAPI.GetBuiltinTemplateApiV1TemplatesBuiltinTemplateIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetBuiltinTemplateApiV1TemplatesBuiltinTemplateIdGet`: TemplateDetailResponse
	fmt.Fprintf(os.Stdout, "Response from `TemplatesAPI.GetBuiltinTemplateApiV1TemplatesBuiltinTemplateIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetBuiltinTemplateApiV1TemplatesBuiltinTemplateIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**TemplateDetailResponse**](TemplateDetailResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetCustomTemplateApiV1TemplatesCustomTemplateIdGet

> CustomTemplateResponse GetCustomTemplateApiV1TemplatesCustomTemplateIdGet(ctx, templateId).Execute()

Get Custom Template

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
	resp, r, err := apiClient.TemplatesAPI.GetCustomTemplateApiV1TemplatesCustomTemplateIdGet(context.Background(), templateId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TemplatesAPI.GetCustomTemplateApiV1TemplatesCustomTemplateIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetCustomTemplateApiV1TemplatesCustomTemplateIdGet`: CustomTemplateResponse
	fmt.Fprintf(os.Stdout, "Response from `TemplatesAPI.GetCustomTemplateApiV1TemplatesCustomTemplateIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetCustomTemplateApiV1TemplatesCustomTemplateIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**CustomTemplateResponse**](CustomTemplateResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetTemplateApiV1TemplatesTemplateIdGet

> TemplateDetailResponse GetTemplateApiV1TemplatesTemplateIdGet(ctx, templateId).Execute()

Get Template

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
	resp, r, err := apiClient.TemplatesAPI.GetTemplateApiV1TemplatesTemplateIdGet(context.Background(), templateId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TemplatesAPI.GetTemplateApiV1TemplatesTemplateIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetTemplateApiV1TemplatesTemplateIdGet`: TemplateDetailResponse
	fmt.Fprintf(os.Stdout, "Response from `TemplatesAPI.GetTemplateApiV1TemplatesTemplateIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetTemplateApiV1TemplatesTemplateIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**TemplateDetailResponse**](TemplateDetailResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListCustomTemplatesApiV1TemplatesCustomGet

> CustomTemplatesListResponse ListCustomTemplatesApiV1TemplatesCustomGet(ctx).Limit(limit).Cursor(cursor).Execute()

List Custom Templates

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
	resp, r, err := apiClient.TemplatesAPI.ListCustomTemplatesApiV1TemplatesCustomGet(context.Background()).Limit(limit).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TemplatesAPI.ListCustomTemplatesApiV1TemplatesCustomGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListCustomTemplatesApiV1TemplatesCustomGet`: CustomTemplatesListResponse
	fmt.Fprintf(os.Stdout, "Response from `TemplatesAPI.ListCustomTemplatesApiV1TemplatesCustomGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListCustomTemplatesApiV1TemplatesCustomGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int32** |  | [default to 50]
 **cursor** | **string** |  | 

### Return type

[**CustomTemplatesListResponse**](CustomTemplatesListResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PatchTemplateApiV1TemplatesCustomTemplateIdPatch

> CustomTemplateResponse PatchTemplateApiV1TemplatesCustomTemplateIdPatch(ctx, templateId).TemplatePatchRequest(templatePatchRequest).Execute()

Patch Template

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
	templatePatchRequest := *openapiclient.NewTemplatePatchRequest() // TemplatePatchRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TemplatesAPI.PatchTemplateApiV1TemplatesCustomTemplateIdPatch(context.Background(), templateId).TemplatePatchRequest(templatePatchRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TemplatesAPI.PatchTemplateApiV1TemplatesCustomTemplateIdPatch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PatchTemplateApiV1TemplatesCustomTemplateIdPatch`: CustomTemplateResponse
	fmt.Fprintf(os.Stdout, "Response from `TemplatesAPI.PatchTemplateApiV1TemplatesCustomTemplateIdPatch`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiPatchTemplateApiV1TemplatesCustomTemplateIdPatchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **templatePatchRequest** | [**TemplatePatchRequest**](TemplatePatchRequest.md) |  | 

### Return type

[**CustomTemplateResponse**](CustomTemplateResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PreviewTemplateApiV1TemplatesTemplateIdPreviewPost

> interface{} PreviewTemplateApiV1TemplatesTemplateIdPreviewPost(ctx, templateId).AppSchemasV1DocumentRenderRequest(appSchemasV1DocumentRenderRequest).IdempotencyKey(idempotencyKey).Execute()

Preview Template

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/invoicepdfs/invoicepdfs-go"
)

func main() {
	templateId := "templateId_example" // string | 
	appSchemasV1DocumentRenderRequest := *openapiclient.NewAppSchemasV1DocumentRenderRequest(*openapiclient.NewDocumentInvoiceDataInput("INV-2026-001", time.Now(), "USD", *openapiclient.NewDocumentPartyInput("Acme Corp"), *openapiclient.NewDocumentPartyInput("Acme Corp"), []openapiclient.DocumentLineItemInput{*openapiclient.NewDocumentLineItemInput("Web Development", "2", "150.00")}), *openapiclient.NewDocumentTemplateRef("Id_example")) // AppSchemasV1DocumentRenderRequest | 
	idempotencyKey := "idempotencyKey_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TemplatesAPI.PreviewTemplateApiV1TemplatesTemplateIdPreviewPost(context.Background(), templateId).AppSchemasV1DocumentRenderRequest(appSchemasV1DocumentRenderRequest).IdempotencyKey(idempotencyKey).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TemplatesAPI.PreviewTemplateApiV1TemplatesTemplateIdPreviewPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PreviewTemplateApiV1TemplatesTemplateIdPreviewPost`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TemplatesAPI.PreviewTemplateApiV1TemplatesTemplateIdPreviewPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiPreviewTemplateApiV1TemplatesTemplateIdPreviewPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **appSchemasV1DocumentRenderRequest** | [**AppSchemasV1DocumentRenderRequest**](AppSchemasV1DocumentRenderRequest.md) |  | 
 **idempotencyKey** | **string** |  | 

### Return type

**interface{}**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PublishTemplateApiV1TemplatesCustomTemplateIdPublishPost

> CustomTemplateResponse PublishTemplateApiV1TemplatesCustomTemplateIdPublishPost(ctx, templateId).Execute()

Publish Template

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
	resp, r, err := apiClient.TemplatesAPI.PublishTemplateApiV1TemplatesCustomTemplateIdPublishPost(context.Background(), templateId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TemplatesAPI.PublishTemplateApiV1TemplatesCustomTemplateIdPublishPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PublishTemplateApiV1TemplatesCustomTemplateIdPublishPost`: CustomTemplateResponse
	fmt.Fprintf(os.Stdout, "Response from `TemplatesAPI.PublishTemplateApiV1TemplatesCustomTemplateIdPublishPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiPublishTemplateApiV1TemplatesCustomTemplateIdPublishPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**CustomTemplateResponse**](CustomTemplateResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## TemplatesApiV1TemplatesGet

> TemplatesListResponse TemplatesApiV1TemplatesGet(ctx).Execute()

Templates

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
	resp, r, err := apiClient.TemplatesAPI.TemplatesApiV1TemplatesGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TemplatesAPI.TemplatesApiV1TemplatesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TemplatesApiV1TemplatesGet`: TemplatesListResponse
	fmt.Fprintf(os.Stdout, "Response from `TemplatesAPI.TemplatesApiV1TemplatesGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiTemplatesApiV1TemplatesGetRequest struct via the builder pattern


### Return type

[**TemplatesListResponse**](TemplatesListResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

