# \NumberingSequencesAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ConsumeSequenceNumber**](NumberingSequencesAPI.md#ConsumeSequenceNumber) | **Post** /api/v1/numbering-sequences/{sequence_id}/next | Consume Sequence Number
[**CreateSequence**](NumberingSequencesAPI.md#CreateSequence) | **Post** /api/v1/numbering-sequences | Create Sequence
[**DeleteSequence**](NumberingSequencesAPI.md#DeleteSequence) | **Delete** /api/v1/numbering-sequences/{sequence_id} | Delete Sequence
[**GetSequence**](NumberingSequencesAPI.md#GetSequence) | **Get** /api/v1/numbering-sequences/{sequence_id} | Get Sequence
[**ListSequences**](NumberingSequencesAPI.md#ListSequences) | **Get** /api/v1/numbering-sequences | List Sequences
[**PreviewSequence**](NumberingSequencesAPI.md#PreviewSequence) | **Post** /api/v1/numbering-sequences/{sequence_id}/preview | Preview Sequence
[**UpdateSequence**](NumberingSequencesAPI.md#UpdateSequence) | **Patch** /api/v1/numbering-sequences/{sequence_id} | Update Sequence



## ConsumeSequenceNumber

> NumberingSequenceResponse ConsumeSequenceNumber(ctx, sequenceId).Execute()

Consume Sequence Number



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
	sequenceId := "sequenceId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NumberingSequencesAPI.ConsumeSequenceNumber(context.Background(), sequenceId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NumberingSequencesAPI.ConsumeSequenceNumber``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ConsumeSequenceNumber`: NumberingSequenceResponse
	fmt.Fprintf(os.Stdout, "Response from `NumberingSequencesAPI.ConsumeSequenceNumber`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**sequenceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiConsumeSequenceNumberRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**NumberingSequenceResponse**](NumberingSequenceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateSequence

> NumberingSequenceResponse CreateSequence(ctx).NumberingSequenceCreateRequest(numberingSequenceCreateRequest).Execute()

Create Sequence

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
	numberingSequenceCreateRequest := *openapiclient.NewNumberingSequenceCreateRequest("Default invoice sequence") // NumberingSequenceCreateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NumberingSequencesAPI.CreateSequence(context.Background()).NumberingSequenceCreateRequest(numberingSequenceCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NumberingSequencesAPI.CreateSequence``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateSequence`: NumberingSequenceResponse
	fmt.Fprintf(os.Stdout, "Response from `NumberingSequencesAPI.CreateSequence`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateSequenceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **numberingSequenceCreateRequest** | [**NumberingSequenceCreateRequest**](NumberingSequenceCreateRequest.md) |  | 

### Return type

[**NumberingSequenceResponse**](NumberingSequenceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteSequence

> SimpleBoolResponse DeleteSequence(ctx, sequenceId).Execute()

Delete Sequence

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
	sequenceId := "sequenceId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NumberingSequencesAPI.DeleteSequence(context.Background(), sequenceId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NumberingSequencesAPI.DeleteSequence``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteSequence`: SimpleBoolResponse
	fmt.Fprintf(os.Stdout, "Response from `NumberingSequencesAPI.DeleteSequence`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**sequenceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteSequenceRequest struct via the builder pattern


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


## GetSequence

> NumberingSequenceResponse GetSequence(ctx, sequenceId).Execute()

Get Sequence

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
	sequenceId := "sequenceId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NumberingSequencesAPI.GetSequence(context.Background(), sequenceId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NumberingSequencesAPI.GetSequence``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetSequence`: NumberingSequenceResponse
	fmt.Fprintf(os.Stdout, "Response from `NumberingSequencesAPI.GetSequence`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**sequenceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetSequenceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**NumberingSequenceResponse**](NumberingSequenceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListSequences

> NumberingSequencesListResponse ListSequences(ctx).Limit(limit).Cursor(cursor).Execute()

List Sequences

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
	resp, r, err := apiClient.NumberingSequencesAPI.ListSequences(context.Background()).Limit(limit).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NumberingSequencesAPI.ListSequences``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListSequences`: NumberingSequencesListResponse
	fmt.Fprintf(os.Stdout, "Response from `NumberingSequencesAPI.ListSequences`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListSequencesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int32** |  | [default to 50]
 **cursor** | **string** |  | 

### Return type

[**NumberingSequencesListResponse**](NumberingSequencesListResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PreviewSequence

> NumberingSequencePreviewResponse PreviewSequence(ctx, sequenceId).Execute()

Preview Sequence

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
	sequenceId := "sequenceId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NumberingSequencesAPI.PreviewSequence(context.Background(), sequenceId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NumberingSequencesAPI.PreviewSequence``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PreviewSequence`: NumberingSequencePreviewResponse
	fmt.Fprintf(os.Stdout, "Response from `NumberingSequencesAPI.PreviewSequence`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**sequenceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiPreviewSequenceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**NumberingSequencePreviewResponse**](NumberingSequencePreviewResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateSequence

> NumberingSequenceResponse UpdateSequence(ctx, sequenceId).NumberingSequencePatchRequest(numberingSequencePatchRequest).Execute()

Update Sequence

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
	sequenceId := "sequenceId_example" // string | 
	numberingSequencePatchRequest := *openapiclient.NewNumberingSequencePatchRequest() // NumberingSequencePatchRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NumberingSequencesAPI.UpdateSequence(context.Background(), sequenceId).NumberingSequencePatchRequest(numberingSequencePatchRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NumberingSequencesAPI.UpdateSequence``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateSequence`: NumberingSequenceResponse
	fmt.Fprintf(os.Stdout, "Response from `NumberingSequencesAPI.UpdateSequence`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**sequenceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateSequenceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **numberingSequencePatchRequest** | [**NumberingSequencePatchRequest**](NumberingSequencePatchRequest.md) |  | 

### Return type

[**NumberingSequenceResponse**](NumberingSequenceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

