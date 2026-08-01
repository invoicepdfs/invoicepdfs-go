# \NumberingSequencesAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ConsumeNextApiV1NumberingSequencesSequenceIdNextPost**](NumberingSequencesAPI.md#ConsumeNextApiV1NumberingSequencesSequenceIdNextPost) | **Post** /api/v1/numbering-sequences/{sequence_id}/next | Consume Next
[**CreateSequenceApiV1NumberingSequencesPost**](NumberingSequencesAPI.md#CreateSequenceApiV1NumberingSequencesPost) | **Post** /api/v1/numbering-sequences | Create Sequence
[**DeleteSequenceApiV1NumberingSequencesSequenceIdDelete**](NumberingSequencesAPI.md#DeleteSequenceApiV1NumberingSequencesSequenceIdDelete) | **Delete** /api/v1/numbering-sequences/{sequence_id} | Delete Sequence
[**GetSequenceApiV1NumberingSequencesSequenceIdGet**](NumberingSequencesAPI.md#GetSequenceApiV1NumberingSequencesSequenceIdGet) | **Get** /api/v1/numbering-sequences/{sequence_id} | Get Sequence
[**ListSequencesApiV1NumberingSequencesGet**](NumberingSequencesAPI.md#ListSequencesApiV1NumberingSequencesGet) | **Get** /api/v1/numbering-sequences | List Sequences
[**PreviewSequenceApiV1NumberingSequencesSequenceIdPreviewPost**](NumberingSequencesAPI.md#PreviewSequenceApiV1NumberingSequencesSequenceIdPreviewPost) | **Post** /api/v1/numbering-sequences/{sequence_id}/preview | Preview Sequence
[**UpdateSequenceApiV1NumberingSequencesSequenceIdPatch**](NumberingSequencesAPI.md#UpdateSequenceApiV1NumberingSequencesSequenceIdPatch) | **Patch** /api/v1/numbering-sequences/{sequence_id} | Update Sequence



## ConsumeNextApiV1NumberingSequencesSequenceIdNextPost

> NumberingSequenceResponse ConsumeNextApiV1NumberingSequencesSequenceIdNextPost(ctx, sequenceId).Execute()

Consume Next



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/invoicepdfs"
)

func main() {
	sequenceId := "sequenceId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NumberingSequencesAPI.ConsumeNextApiV1NumberingSequencesSequenceIdNextPost(context.Background(), sequenceId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NumberingSequencesAPI.ConsumeNextApiV1NumberingSequencesSequenceIdNextPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ConsumeNextApiV1NumberingSequencesSequenceIdNextPost`: NumberingSequenceResponse
	fmt.Fprintf(os.Stdout, "Response from `NumberingSequencesAPI.ConsumeNextApiV1NumberingSequencesSequenceIdNextPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**sequenceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiConsumeNextApiV1NumberingSequencesSequenceIdNextPostRequest struct via the builder pattern


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


## CreateSequenceApiV1NumberingSequencesPost

> NumberingSequenceResponse CreateSequenceApiV1NumberingSequencesPost(ctx).NumberingSequenceCreateRequest(numberingSequenceCreateRequest).Execute()

Create Sequence

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/invoicepdfs"
)

func main() {
	numberingSequenceCreateRequest := *openapiclient.NewNumberingSequenceCreateRequest("Default invoice sequence") // NumberingSequenceCreateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NumberingSequencesAPI.CreateSequenceApiV1NumberingSequencesPost(context.Background()).NumberingSequenceCreateRequest(numberingSequenceCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NumberingSequencesAPI.CreateSequenceApiV1NumberingSequencesPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateSequenceApiV1NumberingSequencesPost`: NumberingSequenceResponse
	fmt.Fprintf(os.Stdout, "Response from `NumberingSequencesAPI.CreateSequenceApiV1NumberingSequencesPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateSequenceApiV1NumberingSequencesPostRequest struct via the builder pattern


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


## DeleteSequenceApiV1NumberingSequencesSequenceIdDelete

> SimpleBoolResponse DeleteSequenceApiV1NumberingSequencesSequenceIdDelete(ctx, sequenceId).Execute()

Delete Sequence

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/invoicepdfs"
)

func main() {
	sequenceId := "sequenceId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NumberingSequencesAPI.DeleteSequenceApiV1NumberingSequencesSequenceIdDelete(context.Background(), sequenceId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NumberingSequencesAPI.DeleteSequenceApiV1NumberingSequencesSequenceIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteSequenceApiV1NumberingSequencesSequenceIdDelete`: SimpleBoolResponse
	fmt.Fprintf(os.Stdout, "Response from `NumberingSequencesAPI.DeleteSequenceApiV1NumberingSequencesSequenceIdDelete`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**sequenceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteSequenceApiV1NumberingSequencesSequenceIdDeleteRequest struct via the builder pattern


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


## GetSequenceApiV1NumberingSequencesSequenceIdGet

> NumberingSequenceResponse GetSequenceApiV1NumberingSequencesSequenceIdGet(ctx, sequenceId).Execute()

Get Sequence

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/invoicepdfs"
)

func main() {
	sequenceId := "sequenceId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NumberingSequencesAPI.GetSequenceApiV1NumberingSequencesSequenceIdGet(context.Background(), sequenceId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NumberingSequencesAPI.GetSequenceApiV1NumberingSequencesSequenceIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetSequenceApiV1NumberingSequencesSequenceIdGet`: NumberingSequenceResponse
	fmt.Fprintf(os.Stdout, "Response from `NumberingSequencesAPI.GetSequenceApiV1NumberingSequencesSequenceIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**sequenceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetSequenceApiV1NumberingSequencesSequenceIdGetRequest struct via the builder pattern


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


## ListSequencesApiV1NumberingSequencesGet

> NumberingSequencesListResponse ListSequencesApiV1NumberingSequencesGet(ctx).Limit(limit).Cursor(cursor).Execute()

List Sequences

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/invoicepdfs"
)

func main() {
	limit := int32(56) // int32 |  (optional) (default to 50)
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NumberingSequencesAPI.ListSequencesApiV1NumberingSequencesGet(context.Background()).Limit(limit).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NumberingSequencesAPI.ListSequencesApiV1NumberingSequencesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListSequencesApiV1NumberingSequencesGet`: NumberingSequencesListResponse
	fmt.Fprintf(os.Stdout, "Response from `NumberingSequencesAPI.ListSequencesApiV1NumberingSequencesGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListSequencesApiV1NumberingSequencesGetRequest struct via the builder pattern


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


## PreviewSequenceApiV1NumberingSequencesSequenceIdPreviewPost

> NumberingSequencePreviewResponse PreviewSequenceApiV1NumberingSequencesSequenceIdPreviewPost(ctx, sequenceId).Execute()

Preview Sequence

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/invoicepdfs"
)

func main() {
	sequenceId := "sequenceId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NumberingSequencesAPI.PreviewSequenceApiV1NumberingSequencesSequenceIdPreviewPost(context.Background(), sequenceId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NumberingSequencesAPI.PreviewSequenceApiV1NumberingSequencesSequenceIdPreviewPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PreviewSequenceApiV1NumberingSequencesSequenceIdPreviewPost`: NumberingSequencePreviewResponse
	fmt.Fprintf(os.Stdout, "Response from `NumberingSequencesAPI.PreviewSequenceApiV1NumberingSequencesSequenceIdPreviewPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**sequenceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiPreviewSequenceApiV1NumberingSequencesSequenceIdPreviewPostRequest struct via the builder pattern


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


## UpdateSequenceApiV1NumberingSequencesSequenceIdPatch

> NumberingSequenceResponse UpdateSequenceApiV1NumberingSequencesSequenceIdPatch(ctx, sequenceId).NumberingSequencePatchRequest(numberingSequencePatchRequest).Execute()

Update Sequence

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/invoicepdfs"
)

func main() {
	sequenceId := "sequenceId_example" // string | 
	numberingSequencePatchRequest := *openapiclient.NewNumberingSequencePatchRequest() // NumberingSequencePatchRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NumberingSequencesAPI.UpdateSequenceApiV1NumberingSequencesSequenceIdPatch(context.Background(), sequenceId).NumberingSequencePatchRequest(numberingSequencePatchRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NumberingSequencesAPI.UpdateSequenceApiV1NumberingSequencesSequenceIdPatch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateSequenceApiV1NumberingSequencesSequenceIdPatch`: NumberingSequenceResponse
	fmt.Fprintf(os.Stdout, "Response from `NumberingSequencesAPI.UpdateSequenceApiV1NumberingSequencesSequenceIdPatch`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**sequenceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateSequenceApiV1NumberingSequencesSequenceIdPatchRequest struct via the builder pattern


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

