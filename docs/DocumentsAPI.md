# \DocumentsAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CalculateDocumentApiV1DocumentsCalculatePost**](DocumentsAPI.md#CalculateDocumentApiV1DocumentsCalculatePost) | **Post** /api/v1/documents/calculate | Calculate Document
[**RenderDocumentApiV1DocumentsRenderPost**](DocumentsAPI.md#RenderDocumentApiV1DocumentsRenderPost) | **Post** /api/v1/documents/render | Render Document
[**ValidateDocumentApiV1DocumentsValidatePost**](DocumentsAPI.md#ValidateDocumentApiV1DocumentsValidatePost) | **Post** /api/v1/documents/validate | Validate Document



## CalculateDocumentApiV1DocumentsCalculatePost

> DocumentCalculateResponse CalculateDocumentApiV1DocumentsCalculatePost(ctx).DocumentCalculateRequest(documentCalculateRequest).Execute()

Calculate Document

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/invoicepdfs"
)

func main() {
	documentCalculateRequest := *openapiclient.NewDocumentCalculateRequest(*openapiclient.NewDocumentInvoiceDataInput("INV-2026-001", time.Now(), "USD", *openapiclient.NewDocumentPartyInput("Acme Corp"), *openapiclient.NewDocumentPartyInput("Acme Corp"), []openapiclient.DocumentLineItemInput{*openapiclient.NewDocumentLineItemInput("Web Development", "2", "150.00")})) // DocumentCalculateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.CalculateDocumentApiV1DocumentsCalculatePost(context.Background()).DocumentCalculateRequest(documentCalculateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.CalculateDocumentApiV1DocumentsCalculatePost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CalculateDocumentApiV1DocumentsCalculatePost`: DocumentCalculateResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.CalculateDocumentApiV1DocumentsCalculatePost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCalculateDocumentApiV1DocumentsCalculatePostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **documentCalculateRequest** | [**DocumentCalculateRequest**](DocumentCalculateRequest.md) |  | 

### Return type

[**DocumentCalculateResponse**](DocumentCalculateResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RenderDocumentApiV1DocumentsRenderPost

> interface{} RenderDocumentApiV1DocumentsRenderPost(ctx).DocumentRenderRequest(documentRenderRequest).IdempotencyKey(idempotencyKey).Execute()

Render Document

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/invoicepdfs"
)

func main() {
	documentRenderRequest := *openapiclient.NewDocumentRenderRequest(*openapiclient.NewDocumentInvoiceDataInput("INV-2026-001", time.Now(), "USD", *openapiclient.NewDocumentPartyInput("Acme Corp"), *openapiclient.NewDocumentPartyInput("Acme Corp"), []openapiclient.DocumentLineItemInput{*openapiclient.NewDocumentLineItemInput("Web Development", "2", "150.00")}), *openapiclient.NewDocumentTemplateRef("Id_example")) // DocumentRenderRequest | 
	idempotencyKey := "idempotencyKey_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.RenderDocumentApiV1DocumentsRenderPost(context.Background()).DocumentRenderRequest(documentRenderRequest).IdempotencyKey(idempotencyKey).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.RenderDocumentApiV1DocumentsRenderPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RenderDocumentApiV1DocumentsRenderPost`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.RenderDocumentApiV1DocumentsRenderPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRenderDocumentApiV1DocumentsRenderPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **documentRenderRequest** | [**DocumentRenderRequest**](DocumentRenderRequest.md) |  | 
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


## ValidateDocumentApiV1DocumentsValidatePost

> DocumentValidateResponse ValidateDocumentApiV1DocumentsValidatePost(ctx).DocumentValidateRequest(documentValidateRequest).Execute()

Validate Document

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/invoicepdfs"
)

func main() {
	documentValidateRequest := *openapiclient.NewDocumentValidateRequest(*openapiclient.NewDocumentInvoiceDataInput("INV-2026-001", time.Now(), "USD", *openapiclient.NewDocumentPartyInput("Acme Corp"), *openapiclient.NewDocumentPartyInput("Acme Corp"), []openapiclient.DocumentLineItemInput{*openapiclient.NewDocumentLineItemInput("Web Development", "2", "150.00")})) // DocumentValidateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.ValidateDocumentApiV1DocumentsValidatePost(context.Background()).DocumentValidateRequest(documentValidateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.ValidateDocumentApiV1DocumentsValidatePost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ValidateDocumentApiV1DocumentsValidatePost`: DocumentValidateResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.ValidateDocumentApiV1DocumentsValidatePost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiValidateDocumentApiV1DocumentsValidatePostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **documentValidateRequest** | [**DocumentValidateRequest**](DocumentValidateRequest.md) |  | 

### Return type

[**DocumentValidateResponse**](DocumentValidateResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

