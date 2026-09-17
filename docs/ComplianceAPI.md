# \ComplianceAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**DownloadDocumentXml**](ComplianceAPI.md#DownloadDocumentXml) | **Get** /api/v1/documents/{document_id}/xml | Download Document Xml
[**RenderDocumentXml**](ComplianceAPI.md#RenderDocumentXml) | **Post** /api/v1/documents/xml | Render Document Xml
[**ValidateCompliance**](ComplianceAPI.md#ValidateCompliance) | **Post** /api/v1/documents/validate-compliance | Validate Compliance



## DownloadDocumentXml

> string DownloadDocumentXml(ctx, documentId).Profile(profile).Execute()

Download Document Xml



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
	profile := "peppol_bis_billing_3" // string | Which ruleset to write this against. No default: a document valid under one can be rejected by another, so the choice is the request.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ComplianceAPI.DownloadDocumentXml(context.Background(), documentId).Profile(profile).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ComplianceAPI.DownloadDocumentXml``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DownloadDocumentXml`: string
	fmt.Fprintf(os.Stdout, "Response from `ComplianceAPI.DownloadDocumentXml`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**documentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDownloadDocumentXmlRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **profile** | **string** | Which ruleset to write this against. No default: a document valid under one can be rejected by another, so the choice is the request. | 

### Return type

**string**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/xml, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RenderDocumentXml

> string RenderDocumentXml(ctx).DocumentComplianceRequest(documentComplianceRequest).Execute()

Render Document Xml



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
	documentComplianceRequest := *openapiclient.NewDocumentComplianceRequest(*openapiclient.NewDocumentInvoiceDataInput("INV-2026-001", time.Now(), "USD", *openapiclient.NewDocumentPartyInput("Acme Corp"), *openapiclient.NewDocumentPartyInput("Acme Corp"), []openapiclient.DocumentLineItemInput{*openapiclient.NewDocumentLineItemInput("Web Development", "2", "150.00")}), "peppol_bis_billing_3") // DocumentComplianceRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ComplianceAPI.RenderDocumentXml(context.Background()).DocumentComplianceRequest(documentComplianceRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ComplianceAPI.RenderDocumentXml``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RenderDocumentXml`: string
	fmt.Fprintf(os.Stdout, "Response from `ComplianceAPI.RenderDocumentXml`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRenderDocumentXmlRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **documentComplianceRequest** | [**DocumentComplianceRequest**](DocumentComplianceRequest.md) |  | 

### Return type

**string**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/xml, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ValidateCompliance

> DocumentComplianceResponse ValidateCompliance(ctx).DocumentComplianceRequest(documentComplianceRequest).Execute()

Validate Compliance



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
	documentComplianceRequest := *openapiclient.NewDocumentComplianceRequest(*openapiclient.NewDocumentInvoiceDataInput("INV-2026-001", time.Now(), "USD", *openapiclient.NewDocumentPartyInput("Acme Corp"), *openapiclient.NewDocumentPartyInput("Acme Corp"), []openapiclient.DocumentLineItemInput{*openapiclient.NewDocumentLineItemInput("Web Development", "2", "150.00")}), "peppol_bis_billing_3") // DocumentComplianceRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ComplianceAPI.ValidateCompliance(context.Background()).DocumentComplianceRequest(documentComplianceRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ComplianceAPI.ValidateCompliance``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ValidateCompliance`: DocumentComplianceResponse
	fmt.Fprintf(os.Stdout, "Response from `ComplianceAPI.ValidateCompliance`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiValidateComplianceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **documentComplianceRequest** | [**DocumentComplianceRequest**](DocumentComplianceRequest.md) |  | 

### Return type

[**DocumentComplianceResponse**](DocumentComplianceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

