# \ReferenceAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ListCountriesApiV1ReferenceCountriesGet**](ReferenceAPI.md#ListCountriesApiV1ReferenceCountriesGet) | **Get** /api/v1/reference/countries | List Countries
[**ListCurrenciesApiV1ReferenceCurrenciesGet**](ReferenceAPI.md#ListCurrenciesApiV1ReferenceCurrenciesGet) | **Get** /api/v1/reference/currencies | List Currencies
[**ListDocumentTypesApiV1ReferenceDocumentTypesGet**](ReferenceAPI.md#ListDocumentTypesApiV1ReferenceDocumentTypesGet) | **Get** /api/v1/reference/document-types | List Document Types
[**ListLocalesApiV1ReferenceLocalesGet**](ReferenceAPI.md#ListLocalesApiV1ReferenceLocalesGet) | **Get** /api/v1/reference/locales | List Locales
[**ListPageSizesApiV1ReferencePageSizesGet**](ReferenceAPI.md#ListPageSizesApiV1ReferencePageSizesGet) | **Get** /api/v1/reference/page-sizes | List Page Sizes
[**ListTimezonesApiV1ReferenceTimezonesGet**](ReferenceAPI.md#ListTimezonesApiV1ReferenceTimezonesGet) | **Get** /api/v1/reference/timezones | List Timezones



## ListCountriesApiV1ReferenceCountriesGet

> map[string]interface{} ListCountriesApiV1ReferenceCountriesGet(ctx).Execute()

List Countries

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
	resp, r, err := apiClient.ReferenceAPI.ListCountriesApiV1ReferenceCountriesGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ReferenceAPI.ListCountriesApiV1ReferenceCountriesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListCountriesApiV1ReferenceCountriesGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `ReferenceAPI.ListCountriesApiV1ReferenceCountriesGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListCountriesApiV1ReferenceCountriesGetRequest struct via the builder pattern


### Return type

**map[string]interface{}**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListCurrenciesApiV1ReferenceCurrenciesGet

> map[string]interface{} ListCurrenciesApiV1ReferenceCurrenciesGet(ctx).Execute()

List Currencies

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
	resp, r, err := apiClient.ReferenceAPI.ListCurrenciesApiV1ReferenceCurrenciesGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ReferenceAPI.ListCurrenciesApiV1ReferenceCurrenciesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListCurrenciesApiV1ReferenceCurrenciesGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `ReferenceAPI.ListCurrenciesApiV1ReferenceCurrenciesGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListCurrenciesApiV1ReferenceCurrenciesGetRequest struct via the builder pattern


### Return type

**map[string]interface{}**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListDocumentTypesApiV1ReferenceDocumentTypesGet

> map[string]interface{} ListDocumentTypesApiV1ReferenceDocumentTypesGet(ctx).Execute()

List Document Types

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
	resp, r, err := apiClient.ReferenceAPI.ListDocumentTypesApiV1ReferenceDocumentTypesGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ReferenceAPI.ListDocumentTypesApiV1ReferenceDocumentTypesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListDocumentTypesApiV1ReferenceDocumentTypesGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `ReferenceAPI.ListDocumentTypesApiV1ReferenceDocumentTypesGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListDocumentTypesApiV1ReferenceDocumentTypesGetRequest struct via the builder pattern


### Return type

**map[string]interface{}**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListLocalesApiV1ReferenceLocalesGet

> map[string]interface{} ListLocalesApiV1ReferenceLocalesGet(ctx).Execute()

List Locales

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
	resp, r, err := apiClient.ReferenceAPI.ListLocalesApiV1ReferenceLocalesGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ReferenceAPI.ListLocalesApiV1ReferenceLocalesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListLocalesApiV1ReferenceLocalesGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `ReferenceAPI.ListLocalesApiV1ReferenceLocalesGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListLocalesApiV1ReferenceLocalesGetRequest struct via the builder pattern


### Return type

**map[string]interface{}**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListPageSizesApiV1ReferencePageSizesGet

> map[string]interface{} ListPageSizesApiV1ReferencePageSizesGet(ctx).Execute()

List Page Sizes

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
	resp, r, err := apiClient.ReferenceAPI.ListPageSizesApiV1ReferencePageSizesGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ReferenceAPI.ListPageSizesApiV1ReferencePageSizesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListPageSizesApiV1ReferencePageSizesGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `ReferenceAPI.ListPageSizesApiV1ReferencePageSizesGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListPageSizesApiV1ReferencePageSizesGetRequest struct via the builder pattern


### Return type

**map[string]interface{}**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListTimezonesApiV1ReferenceTimezonesGet

> map[string]interface{} ListTimezonesApiV1ReferenceTimezonesGet(ctx).Execute()

List Timezones

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
	resp, r, err := apiClient.ReferenceAPI.ListTimezonesApiV1ReferenceTimezonesGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ReferenceAPI.ListTimezonesApiV1ReferenceTimezonesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListTimezonesApiV1ReferenceTimezonesGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `ReferenceAPI.ListTimezonesApiV1ReferenceTimezonesGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListTimezonesApiV1ReferenceTimezonesGetRequest struct via the builder pattern


### Return type

**map[string]interface{}**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

