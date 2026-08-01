# \InvoiceAttachmentsAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateAttachmentApiV1DocumentsInvoiceIdAttachmentsPost**](InvoiceAttachmentsAPI.md#CreateAttachmentApiV1DocumentsInvoiceIdAttachmentsPost) | **Post** /api/v1/documents/{invoice_id}/attachments | Create Attachment
[**DeleteAttachmentApiV1DocumentsInvoiceIdAttachmentsAttachmentIdDelete**](InvoiceAttachmentsAPI.md#DeleteAttachmentApiV1DocumentsInvoiceIdAttachmentsAttachmentIdDelete) | **Delete** /api/v1/documents/{invoice_id}/attachments/{attachment_id} | Delete Attachment
[**ListAttachmentsApiV1DocumentsInvoiceIdAttachmentsGet**](InvoiceAttachmentsAPI.md#ListAttachmentsApiV1DocumentsInvoiceIdAttachmentsGet) | **Get** /api/v1/documents/{invoice_id}/attachments | List Attachments



## CreateAttachmentApiV1DocumentsInvoiceIdAttachmentsPost

> InvoiceAttachmentResponse CreateAttachmentApiV1DocumentsInvoiceIdAttachmentsPost(ctx, invoiceId).InvoiceAttachmentCreateRequest(invoiceAttachmentCreateRequest).Execute()

Create Attachment

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
	invoiceId := "invoiceId_example" // string | 
	invoiceAttachmentCreateRequest := *openapiclient.NewInvoiceAttachmentCreateRequest("fil_01ABC") // InvoiceAttachmentCreateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InvoiceAttachmentsAPI.CreateAttachmentApiV1DocumentsInvoiceIdAttachmentsPost(context.Background(), invoiceId).InvoiceAttachmentCreateRequest(invoiceAttachmentCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InvoiceAttachmentsAPI.CreateAttachmentApiV1DocumentsInvoiceIdAttachmentsPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateAttachmentApiV1DocumentsInvoiceIdAttachmentsPost`: InvoiceAttachmentResponse
	fmt.Fprintf(os.Stdout, "Response from `InvoiceAttachmentsAPI.CreateAttachmentApiV1DocumentsInvoiceIdAttachmentsPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**invoiceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateAttachmentApiV1DocumentsInvoiceIdAttachmentsPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **invoiceAttachmentCreateRequest** | [**InvoiceAttachmentCreateRequest**](InvoiceAttachmentCreateRequest.md) |  | 

### Return type

[**InvoiceAttachmentResponse**](InvoiceAttachmentResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteAttachmentApiV1DocumentsInvoiceIdAttachmentsAttachmentIdDelete

> SimpleBoolResponse DeleteAttachmentApiV1DocumentsInvoiceIdAttachmentsAttachmentIdDelete(ctx, invoiceId, attachmentId).Execute()

Delete Attachment

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
	invoiceId := "invoiceId_example" // string | 
	attachmentId := "attachmentId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InvoiceAttachmentsAPI.DeleteAttachmentApiV1DocumentsInvoiceIdAttachmentsAttachmentIdDelete(context.Background(), invoiceId, attachmentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InvoiceAttachmentsAPI.DeleteAttachmentApiV1DocumentsInvoiceIdAttachmentsAttachmentIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteAttachmentApiV1DocumentsInvoiceIdAttachmentsAttachmentIdDelete`: SimpleBoolResponse
	fmt.Fprintf(os.Stdout, "Response from `InvoiceAttachmentsAPI.DeleteAttachmentApiV1DocumentsInvoiceIdAttachmentsAttachmentIdDelete`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**invoiceId** | **string** |  | 
**attachmentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteAttachmentApiV1DocumentsInvoiceIdAttachmentsAttachmentIdDeleteRequest struct via the builder pattern


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


## ListAttachmentsApiV1DocumentsInvoiceIdAttachmentsGet

> InvoiceAttachmentsListResponse ListAttachmentsApiV1DocumentsInvoiceIdAttachmentsGet(ctx, invoiceId).Execute()

List Attachments

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
	invoiceId := "invoiceId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InvoiceAttachmentsAPI.ListAttachmentsApiV1DocumentsInvoiceIdAttachmentsGet(context.Background(), invoiceId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InvoiceAttachmentsAPI.ListAttachmentsApiV1DocumentsInvoiceIdAttachmentsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListAttachmentsApiV1DocumentsInvoiceIdAttachmentsGet`: InvoiceAttachmentsListResponse
	fmt.Fprintf(os.Stdout, "Response from `InvoiceAttachmentsAPI.ListAttachmentsApiV1DocumentsInvoiceIdAttachmentsGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**invoiceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListAttachmentsApiV1DocumentsInvoiceIdAttachmentsGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**InvoiceAttachmentsListResponse**](InvoiceAttachmentsListResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

