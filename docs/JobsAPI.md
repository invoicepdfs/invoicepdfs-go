# \JobsAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CancelJob**](JobsAPI.md#CancelJob) | **Post** /api/v1/jobs/{job_id}/cancel | Cancel Job
[**GetJob**](JobsAPI.md#GetJob) | **Get** /api/v1/jobs/{job_id} | Get Job
[**ListJobs**](JobsAPI.md#ListJobs) | **Get** /api/v1/jobs | List Jobs
[**RetryJob**](JobsAPI.md#RetryJob) | **Post** /api/v1/jobs/{job_id}/retry | Retry Job



## CancelJob

> JobResponse CancelJob(ctx, jobId).Execute()

Cancel Job

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
	jobId := "jobId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobsAPI.CancelJob(context.Background(), jobId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.CancelJob``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CancelJob`: JobResponse
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.CancelJob`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**jobId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCancelJobRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**JobResponse**](JobResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetJob

> JobResponse GetJob(ctx, jobId).Execute()

Get Job

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
	jobId := "jobId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobsAPI.GetJob(context.Background(), jobId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.GetJob``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetJob`: JobResponse
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.GetJob`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**jobId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetJobRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**JobResponse**](JobResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListJobs

> JobsListResponse ListJobs(ctx).Limit(limit).Cursor(cursor).Execute()

List Jobs



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
	resp, r, err := apiClient.JobsAPI.ListJobs(context.Background()).Limit(limit).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.ListJobs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListJobs`: JobsListResponse
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.ListJobs`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListJobsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int32** |  | [default to 50]
 **cursor** | **string** |  | 

### Return type

[**JobsListResponse**](JobsListResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetryJob

> JobResponse RetryJob(ctx, jobId).Execute()

Retry Job

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
	jobId := "jobId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobsAPI.RetryJob(context.Background(), jobId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobsAPI.RetryJob``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetryJob`: JobResponse
	fmt.Fprintf(os.Stdout, "Response from `JobsAPI.RetryJob`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**jobId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetryJobRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**JobResponse**](JobResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

