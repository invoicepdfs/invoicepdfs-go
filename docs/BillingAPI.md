# \BillingAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateCheckoutApiV1BillingCheckoutSessionPost**](BillingAPI.md#CreateCheckoutApiV1BillingCheckoutSessionPost) | **Post** /api/v1/billing/checkout-session | Create Checkout
[**CreatePortalApiV1BillingPortalSessionPost**](BillingAPI.md#CreatePortalApiV1BillingPortalSessionPost) | **Post** /api/v1/billing/portal-session | Create Portal
[**GetSubscriptionApiV1BillingSubscriptionGet**](BillingAPI.md#GetSubscriptionApiV1BillingSubscriptionGet) | **Get** /api/v1/billing/subscription | Get Subscription
[**ListPlansApiV1BillingPlansGet**](BillingAPI.md#ListPlansApiV1BillingPlansGet) | **Get** /api/v1/billing/plans | List Plans



## CreateCheckoutApiV1BillingCheckoutSessionPost

> BillingCheckoutResponse CreateCheckoutApiV1BillingCheckoutSessionPost(ctx).BillingCheckoutRequest(billingCheckoutRequest).Execute()

Create Checkout



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
	billingCheckoutRequest := *openapiclient.NewBillingCheckoutRequest("PriceId_example") // BillingCheckoutRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BillingAPI.CreateCheckoutApiV1BillingCheckoutSessionPost(context.Background()).BillingCheckoutRequest(billingCheckoutRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BillingAPI.CreateCheckoutApiV1BillingCheckoutSessionPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateCheckoutApiV1BillingCheckoutSessionPost`: BillingCheckoutResponse
	fmt.Fprintf(os.Stdout, "Response from `BillingAPI.CreateCheckoutApiV1BillingCheckoutSessionPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateCheckoutApiV1BillingCheckoutSessionPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **billingCheckoutRequest** | [**BillingCheckoutRequest**](BillingCheckoutRequest.md) |  | 

### Return type

[**BillingCheckoutResponse**](BillingCheckoutResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreatePortalApiV1BillingPortalSessionPost

> BillingPortalResponse CreatePortalApiV1BillingPortalSessionPost(ctx).Execute()

Create Portal



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BillingAPI.CreatePortalApiV1BillingPortalSessionPost(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BillingAPI.CreatePortalApiV1BillingPortalSessionPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreatePortalApiV1BillingPortalSessionPost`: BillingPortalResponse
	fmt.Fprintf(os.Stdout, "Response from `BillingAPI.CreatePortalApiV1BillingPortalSessionPost`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiCreatePortalApiV1BillingPortalSessionPostRequest struct via the builder pattern


### Return type

[**BillingPortalResponse**](BillingPortalResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetSubscriptionApiV1BillingSubscriptionGet

> BillingSubscriptionResponse GetSubscriptionApiV1BillingSubscriptionGet(ctx).Execute()

Get Subscription



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BillingAPI.GetSubscriptionApiV1BillingSubscriptionGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BillingAPI.GetSubscriptionApiV1BillingSubscriptionGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetSubscriptionApiV1BillingSubscriptionGet`: BillingSubscriptionResponse
	fmt.Fprintf(os.Stdout, "Response from `BillingAPI.GetSubscriptionApiV1BillingSubscriptionGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetSubscriptionApiV1BillingSubscriptionGetRequest struct via the builder pattern


### Return type

[**BillingSubscriptionResponse**](BillingSubscriptionResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListPlansApiV1BillingPlansGet

> BillingPlansListResponse ListPlansApiV1BillingPlansGet(ctx).Execute()

List Plans



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BillingAPI.ListPlansApiV1BillingPlansGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BillingAPI.ListPlansApiV1BillingPlansGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListPlansApiV1BillingPlansGet`: BillingPlansListResponse
	fmt.Fprintf(os.Stdout, "Response from `BillingAPI.ListPlansApiV1BillingPlansGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListPlansApiV1BillingPlansGetRequest struct via the builder pattern


### Return type

[**BillingPlansListResponse**](BillingPlansListResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

