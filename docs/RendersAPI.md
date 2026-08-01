# \RendersAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**DownloadRenderApiV1RendersRenderIdDownloadGet**](RendersAPI.md#DownloadRenderApiV1RendersRenderIdDownloadGet) | **Get** /api/v1/renders/{render_id}/download | Download Render
[**GetRenderApiV1RendersRenderIdGet**](RendersAPI.md#GetRenderApiV1RendersRenderIdGet) | **Get** /api/v1/renders/{render_id} | Get Render



## DownloadRenderApiV1RendersRenderIdDownloadGet

> *os.File DownloadRenderApiV1RendersRenderIdDownloadGet(ctx, renderId).Execute()

Download Render

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
	renderId := "renderId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RendersAPI.DownloadRenderApiV1RendersRenderIdDownloadGet(context.Background(), renderId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RendersAPI.DownloadRenderApiV1RendersRenderIdDownloadGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DownloadRenderApiV1RendersRenderIdDownloadGet`: *os.File
	fmt.Fprintf(os.Stdout, "Response from `RendersAPI.DownloadRenderApiV1RendersRenderIdDownloadGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**renderId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDownloadRenderApiV1RendersRenderIdDownloadGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[***os.File**](*os.File.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/pdf, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetRenderApiV1RendersRenderIdGet

> map[string]interface{} GetRenderApiV1RendersRenderIdGet(ctx, renderId).Execute()

Get Render

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
	renderId := "renderId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RendersAPI.GetRenderApiV1RendersRenderIdGet(context.Background(), renderId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RendersAPI.GetRenderApiV1RendersRenderIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetRenderApiV1RendersRenderIdGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `RendersAPI.GetRenderApiV1RendersRenderIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**renderId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetRenderApiV1RendersRenderIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

**map[string]interface{}**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

