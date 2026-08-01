# \DeliveriesAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetDeliveryApiV1DeliveriesDeliveryIdGet**](DeliveriesAPI.md#GetDeliveryApiV1DeliveriesDeliveryIdGet) | **Get** /api/v1/deliveries/{delivery_id} | Get Delivery
[**RetryDeliveryApiV1DeliveriesDeliveryIdRetryPost**](DeliveriesAPI.md#RetryDeliveryApiV1DeliveriesDeliveryIdRetryPost) | **Post** /api/v1/deliveries/{delivery_id}/retry | Retry Delivery



## GetDeliveryApiV1DeliveriesDeliveryIdGet

> DeliveryResponse GetDeliveryApiV1DeliveriesDeliveryIdGet(ctx, deliveryId).Execute()

Get Delivery

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
	resp, r, err := apiClient.DeliveriesAPI.GetDeliveryApiV1DeliveriesDeliveryIdGet(context.Background(), deliveryId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DeliveriesAPI.GetDeliveryApiV1DeliveriesDeliveryIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetDeliveryApiV1DeliveriesDeliveryIdGet`: DeliveryResponse
	fmt.Fprintf(os.Stdout, "Response from `DeliveriesAPI.GetDeliveryApiV1DeliveriesDeliveryIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**deliveryId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetDeliveryApiV1DeliveriesDeliveryIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**DeliveryResponse**](DeliveryResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetryDeliveryApiV1DeliveriesDeliveryIdRetryPost

> DeliveryResponse RetryDeliveryApiV1DeliveriesDeliveryIdRetryPost(ctx, deliveryId).Execute()

Retry Delivery

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
	resp, r, err := apiClient.DeliveriesAPI.RetryDeliveryApiV1DeliveriesDeliveryIdRetryPost(context.Background(), deliveryId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DeliveriesAPI.RetryDeliveryApiV1DeliveriesDeliveryIdRetryPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetryDeliveryApiV1DeliveriesDeliveryIdRetryPost`: DeliveryResponse
	fmt.Fprintf(os.Stdout, "Response from `DeliveriesAPI.RetryDeliveryApiV1DeliveriesDeliveryIdRetryPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**deliveryId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetryDeliveryApiV1DeliveriesDeliveryIdRetryPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**DeliveryResponse**](DeliveryResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

