# \WebhooksAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateWebhookEndpointApiV1WebhookEndpointsPost**](WebhooksAPI.md#CreateWebhookEndpointApiV1WebhookEndpointsPost) | **Post** /api/v1/webhook-endpoints | Create Webhook Endpoint
[**DeleteWebhookEndpointApiV1WebhookEndpointsEndpointIdDelete**](WebhooksAPI.md#DeleteWebhookEndpointApiV1WebhookEndpointsEndpointIdDelete) | **Delete** /api/v1/webhook-endpoints/{endpoint_id} | Delete Webhook Endpoint
[**GetWebhookDeliveryApiV1WebhookDeliveriesDeliveryIdGet**](WebhooksAPI.md#GetWebhookDeliveryApiV1WebhookDeliveriesDeliveryIdGet) | **Get** /api/v1/webhook-deliveries/{delivery_id} | Get Webhook Delivery
[**GetWebhookEndpointApiV1WebhookEndpointsEndpointIdGet**](WebhooksAPI.md#GetWebhookEndpointApiV1WebhookEndpointsEndpointIdGet) | **Get** /api/v1/webhook-endpoints/{endpoint_id} | Get Webhook Endpoint
[**ListWebhookDeliveriesApiV1WebhookDeliveriesGet**](WebhooksAPI.md#ListWebhookDeliveriesApiV1WebhookDeliveriesGet) | **Get** /api/v1/webhook-deliveries | List Webhook Deliveries
[**ListWebhookEndpointsApiV1WebhookEndpointsGet**](WebhooksAPI.md#ListWebhookEndpointsApiV1WebhookEndpointsGet) | **Get** /api/v1/webhook-endpoints | List Webhook Endpoints
[**RetryWebhookDeliveryApiV1WebhookDeliveriesDeliveryIdRetryPost**](WebhooksAPI.md#RetryWebhookDeliveryApiV1WebhookDeliveriesDeliveryIdRetryPost) | **Post** /api/v1/webhook-deliveries/{delivery_id}/retry | Retry Webhook Delivery
[**RotateWebhookSecretApiV1WebhookEndpointsEndpointIdRotateSecretPost**](WebhooksAPI.md#RotateWebhookSecretApiV1WebhookEndpointsEndpointIdRotateSecretPost) | **Post** /api/v1/webhook-endpoints/{endpoint_id}/rotate-secret | Rotate Webhook Secret
[**TestWebhookEndpointApiV1WebhookEndpointsEndpointIdTestPost**](WebhooksAPI.md#TestWebhookEndpointApiV1WebhookEndpointsEndpointIdTestPost) | **Post** /api/v1/webhook-endpoints/{endpoint_id}/test | Test Webhook Endpoint
[**UpdateWebhookEndpointApiV1WebhookEndpointsEndpointIdPatch**](WebhooksAPI.md#UpdateWebhookEndpointApiV1WebhookEndpointsEndpointIdPatch) | **Patch** /api/v1/webhook-endpoints/{endpoint_id} | Update Webhook Endpoint



## CreateWebhookEndpointApiV1WebhookEndpointsPost

> WebhookEndpointResponse CreateWebhookEndpointApiV1WebhookEndpointsPost(ctx).WebhookEndpointCreateRequest(webhookEndpointCreateRequest).Execute()

Create Webhook Endpoint

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
	webhookEndpointCreateRequest := *openapiclient.NewWebhookEndpointCreateRequest("https://example.com/webhooks", []string{"Events_example"}) // WebhookEndpointCreateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WebhooksAPI.CreateWebhookEndpointApiV1WebhookEndpointsPost(context.Background()).WebhookEndpointCreateRequest(webhookEndpointCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WebhooksAPI.CreateWebhookEndpointApiV1WebhookEndpointsPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateWebhookEndpointApiV1WebhookEndpointsPost`: WebhookEndpointResponse
	fmt.Fprintf(os.Stdout, "Response from `WebhooksAPI.CreateWebhookEndpointApiV1WebhookEndpointsPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateWebhookEndpointApiV1WebhookEndpointsPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **webhookEndpointCreateRequest** | [**WebhookEndpointCreateRequest**](WebhookEndpointCreateRequest.md) |  | 

### Return type

[**WebhookEndpointResponse**](WebhookEndpointResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteWebhookEndpointApiV1WebhookEndpointsEndpointIdDelete

> SimpleBoolResponse DeleteWebhookEndpointApiV1WebhookEndpointsEndpointIdDelete(ctx, endpointId).Execute()

Delete Webhook Endpoint

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
	endpointId := "endpointId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WebhooksAPI.DeleteWebhookEndpointApiV1WebhookEndpointsEndpointIdDelete(context.Background(), endpointId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WebhooksAPI.DeleteWebhookEndpointApiV1WebhookEndpointsEndpointIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteWebhookEndpointApiV1WebhookEndpointsEndpointIdDelete`: SimpleBoolResponse
	fmt.Fprintf(os.Stdout, "Response from `WebhooksAPI.DeleteWebhookEndpointApiV1WebhookEndpointsEndpointIdDelete`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**endpointId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteWebhookEndpointApiV1WebhookEndpointsEndpointIdDeleteRequest struct via the builder pattern


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


## GetWebhookDeliveryApiV1WebhookDeliveriesDeliveryIdGet

> WebhookDeliveryResponse GetWebhookDeliveryApiV1WebhookDeliveriesDeliveryIdGet(ctx, deliveryId).Execute()

Get Webhook Delivery

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
	deliveryId := "deliveryId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WebhooksAPI.GetWebhookDeliveryApiV1WebhookDeliveriesDeliveryIdGet(context.Background(), deliveryId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WebhooksAPI.GetWebhookDeliveryApiV1WebhookDeliveriesDeliveryIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetWebhookDeliveryApiV1WebhookDeliveriesDeliveryIdGet`: WebhookDeliveryResponse
	fmt.Fprintf(os.Stdout, "Response from `WebhooksAPI.GetWebhookDeliveryApiV1WebhookDeliveriesDeliveryIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**deliveryId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetWebhookDeliveryApiV1WebhookDeliveriesDeliveryIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**WebhookDeliveryResponse**](WebhookDeliveryResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetWebhookEndpointApiV1WebhookEndpointsEndpointIdGet

> WebhookEndpointResponse GetWebhookEndpointApiV1WebhookEndpointsEndpointIdGet(ctx, endpointId).Execute()

Get Webhook Endpoint

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
	endpointId := "endpointId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WebhooksAPI.GetWebhookEndpointApiV1WebhookEndpointsEndpointIdGet(context.Background(), endpointId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WebhooksAPI.GetWebhookEndpointApiV1WebhookEndpointsEndpointIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetWebhookEndpointApiV1WebhookEndpointsEndpointIdGet`: WebhookEndpointResponse
	fmt.Fprintf(os.Stdout, "Response from `WebhooksAPI.GetWebhookEndpointApiV1WebhookEndpointsEndpointIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**endpointId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetWebhookEndpointApiV1WebhookEndpointsEndpointIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**WebhookEndpointResponse**](WebhookEndpointResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListWebhookDeliveriesApiV1WebhookDeliveriesGet

> WebhookDeliveriesListResponse ListWebhookDeliveriesApiV1WebhookDeliveriesGet(ctx).Limit(limit).Cursor(cursor).Execute()

List Webhook Deliveries

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
	resp, r, err := apiClient.WebhooksAPI.ListWebhookDeliveriesApiV1WebhookDeliveriesGet(context.Background()).Limit(limit).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WebhooksAPI.ListWebhookDeliveriesApiV1WebhookDeliveriesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListWebhookDeliveriesApiV1WebhookDeliveriesGet`: WebhookDeliveriesListResponse
	fmt.Fprintf(os.Stdout, "Response from `WebhooksAPI.ListWebhookDeliveriesApiV1WebhookDeliveriesGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListWebhookDeliveriesApiV1WebhookDeliveriesGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int32** |  | [default to 50]
 **cursor** | **string** |  | 

### Return type

[**WebhookDeliveriesListResponse**](WebhookDeliveriesListResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListWebhookEndpointsApiV1WebhookEndpointsGet

> WebhookEndpointsListResponse ListWebhookEndpointsApiV1WebhookEndpointsGet(ctx).Limit(limit).Cursor(cursor).Execute()

List Webhook Endpoints

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
	resp, r, err := apiClient.WebhooksAPI.ListWebhookEndpointsApiV1WebhookEndpointsGet(context.Background()).Limit(limit).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WebhooksAPI.ListWebhookEndpointsApiV1WebhookEndpointsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListWebhookEndpointsApiV1WebhookEndpointsGet`: WebhookEndpointsListResponse
	fmt.Fprintf(os.Stdout, "Response from `WebhooksAPI.ListWebhookEndpointsApiV1WebhookEndpointsGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListWebhookEndpointsApiV1WebhookEndpointsGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int32** |  | [default to 50]
 **cursor** | **string** |  | 

### Return type

[**WebhookEndpointsListResponse**](WebhookEndpointsListResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetryWebhookDeliveryApiV1WebhookDeliveriesDeliveryIdRetryPost

> WebhookDeliveryResponse RetryWebhookDeliveryApiV1WebhookDeliveriesDeliveryIdRetryPost(ctx, deliveryId).Execute()

Retry Webhook Delivery

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
	deliveryId := "deliveryId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WebhooksAPI.RetryWebhookDeliveryApiV1WebhookDeliveriesDeliveryIdRetryPost(context.Background(), deliveryId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WebhooksAPI.RetryWebhookDeliveryApiV1WebhookDeliveriesDeliveryIdRetryPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetryWebhookDeliveryApiV1WebhookDeliveriesDeliveryIdRetryPost`: WebhookDeliveryResponse
	fmt.Fprintf(os.Stdout, "Response from `WebhooksAPI.RetryWebhookDeliveryApiV1WebhookDeliveriesDeliveryIdRetryPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**deliveryId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetryWebhookDeliveryApiV1WebhookDeliveriesDeliveryIdRetryPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**WebhookDeliveryResponse**](WebhookDeliveryResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RotateWebhookSecretApiV1WebhookEndpointsEndpointIdRotateSecretPost

> WebhookSecretResponse RotateWebhookSecretApiV1WebhookEndpointsEndpointIdRotateSecretPost(ctx, endpointId).Execute()

Rotate Webhook Secret

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
	endpointId := "endpointId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WebhooksAPI.RotateWebhookSecretApiV1WebhookEndpointsEndpointIdRotateSecretPost(context.Background(), endpointId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WebhooksAPI.RotateWebhookSecretApiV1WebhookEndpointsEndpointIdRotateSecretPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RotateWebhookSecretApiV1WebhookEndpointsEndpointIdRotateSecretPost`: WebhookSecretResponse
	fmt.Fprintf(os.Stdout, "Response from `WebhooksAPI.RotateWebhookSecretApiV1WebhookEndpointsEndpointIdRotateSecretPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**endpointId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRotateWebhookSecretApiV1WebhookEndpointsEndpointIdRotateSecretPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**WebhookSecretResponse**](WebhookSecretResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## TestWebhookEndpointApiV1WebhookEndpointsEndpointIdTestPost

> WebhookDeliveryResponse TestWebhookEndpointApiV1WebhookEndpointsEndpointIdTestPost(ctx, endpointId).Execute()

Test Webhook Endpoint

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
	endpointId := "endpointId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WebhooksAPI.TestWebhookEndpointApiV1WebhookEndpointsEndpointIdTestPost(context.Background(), endpointId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WebhooksAPI.TestWebhookEndpointApiV1WebhookEndpointsEndpointIdTestPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TestWebhookEndpointApiV1WebhookEndpointsEndpointIdTestPost`: WebhookDeliveryResponse
	fmt.Fprintf(os.Stdout, "Response from `WebhooksAPI.TestWebhookEndpointApiV1WebhookEndpointsEndpointIdTestPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**endpointId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTestWebhookEndpointApiV1WebhookEndpointsEndpointIdTestPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**WebhookDeliveryResponse**](WebhookDeliveryResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateWebhookEndpointApiV1WebhookEndpointsEndpointIdPatch

> WebhookEndpointResponse UpdateWebhookEndpointApiV1WebhookEndpointsEndpointIdPatch(ctx, endpointId).WebhookEndpointPatchRequest(webhookEndpointPatchRequest).Execute()

Update Webhook Endpoint

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
	endpointId := "endpointId_example" // string | 
	webhookEndpointPatchRequest := *openapiclient.NewWebhookEndpointPatchRequest() // WebhookEndpointPatchRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WebhooksAPI.UpdateWebhookEndpointApiV1WebhookEndpointsEndpointIdPatch(context.Background(), endpointId).WebhookEndpointPatchRequest(webhookEndpointPatchRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WebhooksAPI.UpdateWebhookEndpointApiV1WebhookEndpointsEndpointIdPatch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateWebhookEndpointApiV1WebhookEndpointsEndpointIdPatch`: WebhookEndpointResponse
	fmt.Fprintf(os.Stdout, "Response from `WebhooksAPI.UpdateWebhookEndpointApiV1WebhookEndpointsEndpointIdPatch`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**endpointId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateWebhookEndpointApiV1WebhookEndpointsEndpointIdPatchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **webhookEndpointPatchRequest** | [**WebhookEndpointPatchRequest**](WebhookEndpointPatchRequest.md) |  | 

### Return type

[**WebhookEndpointResponse**](WebhookEndpointResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

