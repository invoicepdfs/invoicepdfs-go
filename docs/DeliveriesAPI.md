# \DeliveriesAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetDelivery**](DeliveriesAPI.md#GetDelivery) | **Get** /api/v1/deliveries/{delivery_id} | Get Delivery
[**RetryDelivery**](DeliveriesAPI.md#RetryDelivery) | **Post** /api/v1/deliveries/{delivery_id}/retry | Retry Delivery



## GetDelivery

> DeliveryResponse GetDelivery(ctx, deliveryId).Execute()

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
	resp, r, err := apiClient.DeliveriesAPI.GetDelivery(context.Background(), deliveryId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DeliveriesAPI.GetDelivery``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetDelivery`: DeliveryResponse
	fmt.Fprintf(os.Stdout, "Response from `DeliveriesAPI.GetDelivery`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**deliveryId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetDeliveryRequest struct via the builder pattern


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


## RetryDelivery

> DeliveryResponse RetryDelivery(ctx, deliveryId).Execute()

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
	resp, r, err := apiClient.DeliveriesAPI.RetryDelivery(context.Background(), deliveryId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DeliveriesAPI.RetryDelivery``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetryDelivery`: DeliveryResponse
	fmt.Fprintf(os.Stdout, "Response from `DeliveriesAPI.RetryDelivery`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**deliveryId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetryDeliveryRequest struct via the builder pattern


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

