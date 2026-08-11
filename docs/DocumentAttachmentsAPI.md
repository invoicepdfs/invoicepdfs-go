# \DocumentAttachmentsAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateDocumentAttachment**](DocumentAttachmentsAPI.md#CreateDocumentAttachment) | **Post** /api/v1/documents/{document_id}/attachments | Create Document Attachment
[**DeleteDocumentAttachment**](DocumentAttachmentsAPI.md#DeleteDocumentAttachment) | **Delete** /api/v1/documents/{document_id}/attachments/{attachment_id} | Delete Document Attachment
[**ListDocumentAttachments**](DocumentAttachmentsAPI.md#ListDocumentAttachments) | **Get** /api/v1/documents/{document_id}/attachments | List Document Attachments



## CreateDocumentAttachment

> InvoiceAttachmentResponse CreateDocumentAttachment(ctx, documentId).InvoiceAttachmentCreateRequest(invoiceAttachmentCreateRequest).Execute()

Create Document Attachment

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
	documentId := "documentId_example" // string | 
	invoiceAttachmentCreateRequest := *openapiclient.NewInvoiceAttachmentCreateRequest("fil_01ABC") // InvoiceAttachmentCreateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentAttachmentsAPI.CreateDocumentAttachment(context.Background(), documentId).InvoiceAttachmentCreateRequest(invoiceAttachmentCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentAttachmentsAPI.CreateDocumentAttachment``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateDocumentAttachment`: InvoiceAttachmentResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentAttachmentsAPI.CreateDocumentAttachment`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**documentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateDocumentAttachmentRequest struct via the builder pattern


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


## DeleteDocumentAttachment

> SimpleBoolResponse DeleteDocumentAttachment(ctx, documentId, attachmentId).Execute()

Delete Document Attachment

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
	documentId := "documentId_example" // string | 
	attachmentId := "attachmentId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentAttachmentsAPI.DeleteDocumentAttachment(context.Background(), documentId, attachmentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentAttachmentsAPI.DeleteDocumentAttachment``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteDocumentAttachment`: SimpleBoolResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentAttachmentsAPI.DeleteDocumentAttachment`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**documentId** | **string** |  | 
**attachmentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteDocumentAttachmentRequest struct via the builder pattern


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


## ListDocumentAttachments

> InvoiceAttachmentsListResponse ListDocumentAttachments(ctx, documentId).Execute()

List Document Attachments

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
	documentId := "documentId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentAttachmentsAPI.ListDocumentAttachments(context.Background(), documentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentAttachmentsAPI.ListDocumentAttachments``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListDocumentAttachments`: InvoiceAttachmentsListResponse
	fmt.Fprintf(os.Stdout, "Response from `DocumentAttachmentsAPI.ListDocumentAttachments`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**documentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListDocumentAttachmentsRequest struct via the builder pattern


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

