# \RendersAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**DownloadRender**](RendersAPI.md#DownloadRender) | **Get** /api/v1/renders/{render_id}/download | Download Render
[**GetRender**](RendersAPI.md#GetRender) | **Get** /api/v1/renders/{render_id} | Get Render



## DownloadRender

> *os.File DownloadRender(ctx, renderId).Token(token).Execute()

Download Render



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
	renderId := "renderId_example" // string | 
	token := "token_example" // string | The signature from this render's `download_url`. Present it and no API key is needed — that is what makes the URL a link. Omit it and the request authenticates normally. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RendersAPI.DownloadRender(context.Background(), renderId).Token(token).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RendersAPI.DownloadRender``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DownloadRender`: *os.File
	fmt.Fprintf(os.Stdout, "Response from `RendersAPI.DownloadRender`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**renderId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDownloadRenderRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **token** | **string** | The signature from this render&#39;s &#x60;download_url&#x60;. Present it and no API key is needed — that is what makes the URL a link. Omit it and the request authenticates normally. | 

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


## GetRender

> RenderResponse GetRender(ctx, renderId).Execute()

Get Render

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
	renderId := "renderId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RendersAPI.GetRender(context.Background(), renderId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RendersAPI.GetRender``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetRender`: RenderResponse
	fmt.Fprintf(os.Stdout, "Response from `RendersAPI.GetRender`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**renderId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetRenderRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**RenderResponse**](RenderResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

