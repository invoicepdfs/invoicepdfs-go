# \WebhooksAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateWebhookEndpoint**](WebhooksAPI.md#CreateWebhookEndpoint) | **Post** /api/v1/webhook-endpoints | Create Webhook Endpoint
[**DeleteWebhookEndpoint**](WebhooksAPI.md#DeleteWebhookEndpoint) | **Delete** /api/v1/webhook-endpoints/{endpoint_id} | Delete Webhook Endpoint
[**GetWebhookDelivery**](WebhooksAPI.md#GetWebhookDelivery) | **Get** /api/v1/webhook-deliveries/{delivery_id} | Get Webhook Delivery
[**GetWebhookEndpoint**](WebhooksAPI.md#GetWebhookEndpoint) | **Get** /api/v1/webhook-endpoints/{endpoint_id} | Get Webhook Endpoint
[**ListWebhookDeliveries**](WebhooksAPI.md#ListWebhookDeliveries) | **Get** /api/v1/webhook-deliveries | List Webhook Deliveries
[**ListWebhookEndpoints**](WebhooksAPI.md#ListWebhookEndpoints) | **Get** /api/v1/webhook-endpoints | List Webhook Endpoints
[**RetryWebhookDelivery**](WebhooksAPI.md#RetryWebhookDelivery) | **Post** /api/v1/webhook-deliveries/{delivery_id}/retry | Retry Webhook Delivery
[**RotateWebhookSecret**](WebhooksAPI.md#RotateWebhookSecret) | **Post** /api/v1/webhook-endpoints/{endpoint_id}/rotate-secret | Rotate Webhook Secret
[**TestWebhookEndpoint**](WebhooksAPI.md#TestWebhookEndpoint) | **Post** /api/v1/webhook-endpoints/{endpoint_id}/test | Test Webhook Endpoint
[**UpdateWebhookEndpoint**](WebhooksAPI.md#UpdateWebhookEndpoint) | **Patch** /api/v1/webhook-endpoints/{endpoint_id} | Update Webhook Endpoint



## CreateWebhookEndpoint

> WebhookEndpointResponse CreateWebhookEndpoint(ctx).WebhookEndpointCreateRequest(webhookEndpointCreateRequest).Execute()

Create Webhook Endpoint

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
	webhookEndpointCreateRequest := *openapiclient.NewWebhookEndpointCreateRequest("https://example.com/webhooks", []string{"Events_example"}) // WebhookEndpointCreateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WebhooksAPI.CreateWebhookEndpoint(context.Background()).WebhookEndpointCreateRequest(webhookEndpointCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WebhooksAPI.CreateWebhookEndpoint``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateWebhookEndpoint`: WebhookEndpointResponse
	fmt.Fprintf(os.Stdout, "Response from `WebhooksAPI.CreateWebhookEndpoint`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateWebhookEndpointRequest struct via the builder pattern


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


## DeleteWebhookEndpoint

> SimpleBoolResponse DeleteWebhookEndpoint(ctx, endpointId).Execute()

Delete Webhook Endpoint

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
	endpointId := "endpointId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WebhooksAPI.DeleteWebhookEndpoint(context.Background(), endpointId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WebhooksAPI.DeleteWebhookEndpoint``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteWebhookEndpoint`: SimpleBoolResponse
	fmt.Fprintf(os.Stdout, "Response from `WebhooksAPI.DeleteWebhookEndpoint`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**endpointId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteWebhookEndpointRequest struct via the builder pattern


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


## GetWebhookDelivery

> WebhookDeliveryResponse GetWebhookDelivery(ctx, deliveryId).Execute()

Get Webhook Delivery

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
	deliveryId := "deliveryId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WebhooksAPI.GetWebhookDelivery(context.Background(), deliveryId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WebhooksAPI.GetWebhookDelivery``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetWebhookDelivery`: WebhookDeliveryResponse
	fmt.Fprintf(os.Stdout, "Response from `WebhooksAPI.GetWebhookDelivery`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**deliveryId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetWebhookDeliveryRequest struct via the builder pattern


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


## GetWebhookEndpoint

> WebhookEndpointResponse GetWebhookEndpoint(ctx, endpointId).Execute()

Get Webhook Endpoint

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
	endpointId := "endpointId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WebhooksAPI.GetWebhookEndpoint(context.Background(), endpointId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WebhooksAPI.GetWebhookEndpoint``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetWebhookEndpoint`: WebhookEndpointResponse
	fmt.Fprintf(os.Stdout, "Response from `WebhooksAPI.GetWebhookEndpoint`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**endpointId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetWebhookEndpointRequest struct via the builder pattern


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


## ListWebhookDeliveries

> WebhookDeliveriesListResponse ListWebhookDeliveries(ctx).Limit(limit).Cursor(cursor).Execute()

List Webhook Deliveries

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
	resp, r, err := apiClient.WebhooksAPI.ListWebhookDeliveries(context.Background()).Limit(limit).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WebhooksAPI.ListWebhookDeliveries``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListWebhookDeliveries`: WebhookDeliveriesListResponse
	fmt.Fprintf(os.Stdout, "Response from `WebhooksAPI.ListWebhookDeliveries`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListWebhookDeliveriesRequest struct via the builder pattern


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


## ListWebhookEndpoints

> WebhookEndpointsListResponse ListWebhookEndpoints(ctx).Limit(limit).Cursor(cursor).Execute()

List Webhook Endpoints

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
	resp, r, err := apiClient.WebhooksAPI.ListWebhookEndpoints(context.Background()).Limit(limit).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WebhooksAPI.ListWebhookEndpoints``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListWebhookEndpoints`: WebhookEndpointsListResponse
	fmt.Fprintf(os.Stdout, "Response from `WebhooksAPI.ListWebhookEndpoints`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListWebhookEndpointsRequest struct via the builder pattern


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


## RetryWebhookDelivery

> WebhookDeliveryResponse RetryWebhookDelivery(ctx, deliveryId).Execute()

Retry Webhook Delivery

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
	deliveryId := "deliveryId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WebhooksAPI.RetryWebhookDelivery(context.Background(), deliveryId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WebhooksAPI.RetryWebhookDelivery``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetryWebhookDelivery`: WebhookDeliveryResponse
	fmt.Fprintf(os.Stdout, "Response from `WebhooksAPI.RetryWebhookDelivery`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**deliveryId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetryWebhookDeliveryRequest struct via the builder pattern


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


## RotateWebhookSecret

> WebhookSecretResponse RotateWebhookSecret(ctx, endpointId).Execute()

Rotate Webhook Secret

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
	endpointId := "endpointId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WebhooksAPI.RotateWebhookSecret(context.Background(), endpointId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WebhooksAPI.RotateWebhookSecret``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RotateWebhookSecret`: WebhookSecretResponse
	fmt.Fprintf(os.Stdout, "Response from `WebhooksAPI.RotateWebhookSecret`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**endpointId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRotateWebhookSecretRequest struct via the builder pattern


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


## TestWebhookEndpoint

> WebhookDeliveryResponse TestWebhookEndpoint(ctx, endpointId).Execute()

Test Webhook Endpoint

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
	endpointId := "endpointId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WebhooksAPI.TestWebhookEndpoint(context.Background(), endpointId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WebhooksAPI.TestWebhookEndpoint``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TestWebhookEndpoint`: WebhookDeliveryResponse
	fmt.Fprintf(os.Stdout, "Response from `WebhooksAPI.TestWebhookEndpoint`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**endpointId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTestWebhookEndpointRequest struct via the builder pattern


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


## UpdateWebhookEndpoint

> WebhookEndpointResponse UpdateWebhookEndpoint(ctx, endpointId).WebhookEndpointPatchRequest(webhookEndpointPatchRequest).Execute()

Update Webhook Endpoint

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
	endpointId := "endpointId_example" // string | 
	webhookEndpointPatchRequest := *openapiclient.NewWebhookEndpointPatchRequest() // WebhookEndpointPatchRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WebhooksAPI.UpdateWebhookEndpoint(context.Background(), endpointId).WebhookEndpointPatchRequest(webhookEndpointPatchRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WebhooksAPI.UpdateWebhookEndpoint``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateWebhookEndpoint`: WebhookEndpointResponse
	fmt.Fprintf(os.Stdout, "Response from `WebhooksAPI.UpdateWebhookEndpoint`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**endpointId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateWebhookEndpointRequest struct via the builder pattern


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

