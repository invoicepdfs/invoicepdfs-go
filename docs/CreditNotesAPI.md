# \CreditNotesAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateCreditNoteApiV1CreditNotesPost**](CreditNotesAPI.md#CreateCreditNoteApiV1CreditNotesPost) | **Post** /api/v1/credit-notes | Create Credit Note
[**FinalizeCreditNoteApiV1CreditNotesCreditNoteIdFinalizePost**](CreditNotesAPI.md#FinalizeCreditNoteApiV1CreditNotesCreditNoteIdFinalizePost) | **Post** /api/v1/credit-notes/{credit_note_id}/finalize | Finalize Credit Note
[**GetCreditNoteApiV1CreditNotesCreditNoteIdGet**](CreditNotesAPI.md#GetCreditNoteApiV1CreditNotesCreditNoteIdGet) | **Get** /api/v1/credit-notes/{credit_note_id} | Get Credit Note
[**ListCreditNotesApiV1CreditNotesGet**](CreditNotesAPI.md#ListCreditNotesApiV1CreditNotesGet) | **Get** /api/v1/credit-notes | List Credit Notes
[**RenderCreditNoteApiV1CreditNotesCreditNoteIdRendersPost**](CreditNotesAPI.md#RenderCreditNoteApiV1CreditNotesCreditNoteIdRendersPost) | **Post** /api/v1/credit-notes/{credit_note_id}/renders | Render Credit Note



## CreateCreditNoteApiV1CreditNotesPost

> CreditNoteResponse CreateCreditNoteApiV1CreditNotesPost(ctx).CreditNoteCreateRequest(creditNoteCreateRequest).Execute()

Create Credit Note

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
	creditNoteCreateRequest := *openapiclient.NewCreditNoteCreateRequest("inv_01ABC", "CN-2026-001", time.Now(), []openapiclient.CreditNoteLineItemInput{*openapiclient.NewCreditNoteLineItemInput("Web Development", "1", "150.00")}) // CreditNoteCreateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CreditNotesAPI.CreateCreditNoteApiV1CreditNotesPost(context.Background()).CreditNoteCreateRequest(creditNoteCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CreditNotesAPI.CreateCreditNoteApiV1CreditNotesPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateCreditNoteApiV1CreditNotesPost`: CreditNoteResponse
	fmt.Fprintf(os.Stdout, "Response from `CreditNotesAPI.CreateCreditNoteApiV1CreditNotesPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateCreditNoteApiV1CreditNotesPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **creditNoteCreateRequest** | [**CreditNoteCreateRequest**](CreditNoteCreateRequest.md) |  | 

### Return type

[**CreditNoteResponse**](CreditNoteResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## FinalizeCreditNoteApiV1CreditNotesCreditNoteIdFinalizePost

> CreditNoteResponse FinalizeCreditNoteApiV1CreditNotesCreditNoteIdFinalizePost(ctx, creditNoteId).Execute()

Finalize Credit Note

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
	creditNoteId := "creditNoteId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CreditNotesAPI.FinalizeCreditNoteApiV1CreditNotesCreditNoteIdFinalizePost(context.Background(), creditNoteId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CreditNotesAPI.FinalizeCreditNoteApiV1CreditNotesCreditNoteIdFinalizePost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FinalizeCreditNoteApiV1CreditNotesCreditNoteIdFinalizePost`: CreditNoteResponse
	fmt.Fprintf(os.Stdout, "Response from `CreditNotesAPI.FinalizeCreditNoteApiV1CreditNotesCreditNoteIdFinalizePost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**creditNoteId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiFinalizeCreditNoteApiV1CreditNotesCreditNoteIdFinalizePostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**CreditNoteResponse**](CreditNoteResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetCreditNoteApiV1CreditNotesCreditNoteIdGet

> CreditNoteResponse GetCreditNoteApiV1CreditNotesCreditNoteIdGet(ctx, creditNoteId).Execute()

Get Credit Note

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
	creditNoteId := "creditNoteId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CreditNotesAPI.GetCreditNoteApiV1CreditNotesCreditNoteIdGet(context.Background(), creditNoteId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CreditNotesAPI.GetCreditNoteApiV1CreditNotesCreditNoteIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetCreditNoteApiV1CreditNotesCreditNoteIdGet`: CreditNoteResponse
	fmt.Fprintf(os.Stdout, "Response from `CreditNotesAPI.GetCreditNoteApiV1CreditNotesCreditNoteIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**creditNoteId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetCreditNoteApiV1CreditNotesCreditNoteIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**CreditNoteResponse**](CreditNoteResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListCreditNotesApiV1CreditNotesGet

> CreditNotesListResponse ListCreditNotesApiV1CreditNotesGet(ctx).Limit(limit).Cursor(cursor).Execute()

List Credit Notes

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
	resp, r, err := apiClient.CreditNotesAPI.ListCreditNotesApiV1CreditNotesGet(context.Background()).Limit(limit).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CreditNotesAPI.ListCreditNotesApiV1CreditNotesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListCreditNotesApiV1CreditNotesGet`: CreditNotesListResponse
	fmt.Fprintf(os.Stdout, "Response from `CreditNotesAPI.ListCreditNotesApiV1CreditNotesGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListCreditNotesApiV1CreditNotesGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int32** |  | [default to 50]
 **cursor** | **string** |  | 

### Return type

[**CreditNotesListResponse**](CreditNotesListResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RenderCreditNoteApiV1CreditNotesCreditNoteIdRendersPost

> interface{} RenderCreditNoteApiV1CreditNotesCreditNoteIdRendersPost(ctx, creditNoteId).CreditNoteRenderRequest(creditNoteRenderRequest).Execute()

Render Credit Note

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
	creditNoteId := "creditNoteId_example" // string | 
	creditNoteRenderRequest := *openapiclient.NewCreditNoteRenderRequest() // CreditNoteRenderRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CreditNotesAPI.RenderCreditNoteApiV1CreditNotesCreditNoteIdRendersPost(context.Background(), creditNoteId).CreditNoteRenderRequest(creditNoteRenderRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CreditNotesAPI.RenderCreditNoteApiV1CreditNotesCreditNoteIdRendersPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RenderCreditNoteApiV1CreditNotesCreditNoteIdRendersPost`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `CreditNotesAPI.RenderCreditNoteApiV1CreditNotesCreditNoteIdRendersPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**creditNoteId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRenderCreditNoteApiV1CreditNotesCreditNoteIdRendersPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **creditNoteRenderRequest** | [**CreditNoteRenderRequest**](CreditNoteRenderRequest.md) |  | 

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

