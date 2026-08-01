# \BatchesAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CancelBatchApiV1BatchesBatchIdCancelPost**](BatchesAPI.md#CancelBatchApiV1BatchesBatchIdCancelPost) | **Post** /api/v1/batches/{batch_id}/cancel | Cancel Batch
[**CreateBatchApiV1BatchesPost**](BatchesAPI.md#CreateBatchApiV1BatchesPost) | **Post** /api/v1/batches | Create Batch
[**DownloadBatchApiV1BatchesBatchIdDownloadGet**](BatchesAPI.md#DownloadBatchApiV1BatchesBatchIdDownloadGet) | **Get** /api/v1/batches/{batch_id}/download | Download Batch
[**GetBatchApiV1BatchesBatchIdGet**](BatchesAPI.md#GetBatchApiV1BatchesBatchIdGet) | **Get** /api/v1/batches/{batch_id} | Get Batch
[**ListBatchItemsApiV1BatchesBatchIdItemsGet**](BatchesAPI.md#ListBatchItemsApiV1BatchesBatchIdItemsGet) | **Get** /api/v1/batches/{batch_id}/items | List Batch Items
[**ListBatchesApiV1BatchesGet**](BatchesAPI.md#ListBatchesApiV1BatchesGet) | **Get** /api/v1/batches | List Batches



## CancelBatchApiV1BatchesBatchIdCancelPost

> BatchResponse CancelBatchApiV1BatchesBatchIdCancelPost(ctx, batchId).Execute()

Cancel Batch

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	batchId := "batchId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BatchesAPI.CancelBatchApiV1BatchesBatchIdCancelPost(context.Background(), batchId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BatchesAPI.CancelBatchApiV1BatchesBatchIdCancelPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CancelBatchApiV1BatchesBatchIdCancelPost`: BatchResponse
	fmt.Fprintf(os.Stdout, "Response from `BatchesAPI.CancelBatchApiV1BatchesBatchIdCancelPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**batchId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCancelBatchApiV1BatchesBatchIdCancelPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**BatchResponse**](BatchResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateBatchApiV1BatchesPost

> BatchResponse CreateBatchApiV1BatchesPost(ctx).BatchCreateRequest(batchCreateRequest).Execute()

Create Batch

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	batchCreateRequest := *openapiclient.NewBatchCreateRequest([]openapiclient.BatchItemInput{*openapiclient.NewBatchItemInput(map[string]interface{}{"key": interface{}(123)})}) // BatchCreateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BatchesAPI.CreateBatchApiV1BatchesPost(context.Background()).BatchCreateRequest(batchCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BatchesAPI.CreateBatchApiV1BatchesPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateBatchApiV1BatchesPost`: BatchResponse
	fmt.Fprintf(os.Stdout, "Response from `BatchesAPI.CreateBatchApiV1BatchesPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateBatchApiV1BatchesPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **batchCreateRequest** | [**BatchCreateRequest**](BatchCreateRequest.md) |  | 

### Return type

[**BatchResponse**](BatchResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DownloadBatchApiV1BatchesBatchIdDownloadGet

> interface{} DownloadBatchApiV1BatchesBatchIdDownloadGet(ctx, batchId).Execute()

Download Batch

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	batchId := "batchId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BatchesAPI.DownloadBatchApiV1BatchesBatchIdDownloadGet(context.Background(), batchId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BatchesAPI.DownloadBatchApiV1BatchesBatchIdDownloadGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DownloadBatchApiV1BatchesBatchIdDownloadGet`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BatchesAPI.DownloadBatchApiV1BatchesBatchIdDownloadGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**batchId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDownloadBatchApiV1BatchesBatchIdDownloadGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

**interface{}**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetBatchApiV1BatchesBatchIdGet

> BatchResponse GetBatchApiV1BatchesBatchIdGet(ctx, batchId).Execute()

Get Batch

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	batchId := "batchId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BatchesAPI.GetBatchApiV1BatchesBatchIdGet(context.Background(), batchId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BatchesAPI.GetBatchApiV1BatchesBatchIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetBatchApiV1BatchesBatchIdGet`: BatchResponse
	fmt.Fprintf(os.Stdout, "Response from `BatchesAPI.GetBatchApiV1BatchesBatchIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**batchId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetBatchApiV1BatchesBatchIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**BatchResponse**](BatchResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListBatchItemsApiV1BatchesBatchIdItemsGet

> BatchItemsListResponse ListBatchItemsApiV1BatchesBatchIdItemsGet(ctx, batchId).Limit(limit).Cursor(cursor).Execute()

List Batch Items

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	batchId := "batchId_example" // string | 
	limit := int32(56) // int32 |  (optional) (default to 50)
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BatchesAPI.ListBatchItemsApiV1BatchesBatchIdItemsGet(context.Background(), batchId).Limit(limit).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BatchesAPI.ListBatchItemsApiV1BatchesBatchIdItemsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListBatchItemsApiV1BatchesBatchIdItemsGet`: BatchItemsListResponse
	fmt.Fprintf(os.Stdout, "Response from `BatchesAPI.ListBatchItemsApiV1BatchesBatchIdItemsGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**batchId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListBatchItemsApiV1BatchesBatchIdItemsGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **limit** | **int32** |  | [default to 50]
 **cursor** | **string** |  | 

### Return type

[**BatchItemsListResponse**](BatchItemsListResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListBatchesApiV1BatchesGet

> BatchesListResponse ListBatchesApiV1BatchesGet(ctx).Limit(limit).Cursor(cursor).Execute()

List Batches

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	limit := int32(56) // int32 |  (optional) (default to 50)
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BatchesAPI.ListBatchesApiV1BatchesGet(context.Background()).Limit(limit).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BatchesAPI.ListBatchesApiV1BatchesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListBatchesApiV1BatchesGet`: BatchesListResponse
	fmt.Fprintf(os.Stdout, "Response from `BatchesAPI.ListBatchesApiV1BatchesGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListBatchesApiV1BatchesGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int32** |  | [default to 50]
 **cursor** | **string** |  | 

### Return type

[**BatchesListResponse**](BatchesListResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

