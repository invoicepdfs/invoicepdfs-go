# \AuthAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ExchangeAuthToken**](AuthAPI.md#ExchangeAuthToken) | **Post** /api/v1/auth/token | Exchange Auth Token
[**GetCurrentUser**](AuthAPI.md#GetCurrentUser) | **Get** /api/v1/auth/me | Get Current User
[**Logout**](AuthAPI.md#Logout) | **Post** /api/v1/auth/logout | Logout
[**RefreshAccessToken**](AuthAPI.md#RefreshAccessToken) | **Post** /api/v1/auth/refresh | Refresh Access Token
[**Register**](AuthAPI.md#Register) | **Post** /api/v1/auth/register | Register
[**RequestPasswordReset**](AuthAPI.md#RequestPasswordReset) | **Post** /api/v1/auth/forgot-password | Request Password Reset
[**ResetPassword**](AuthAPI.md#ResetPassword) | **Post** /api/v1/auth/reset-password | Reset Password
[**UpdateCurrentUser**](AuthAPI.md#UpdateCurrentUser) | **Patch** /api/v1/auth/me | Update Current User



## ExchangeAuthToken

> AuthTokenResponse ExchangeAuthToken(ctx).AuthTokenRequest(authTokenRequest).Execute()

Exchange Auth Token



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
	authTokenRequest := *openapiclient.NewAuthTokenRequest("IdToken_example") // AuthTokenRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.ExchangeAuthToken(context.Background()).AuthTokenRequest(authTokenRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.ExchangeAuthToken``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ExchangeAuthToken`: AuthTokenResponse
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.ExchangeAuthToken`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiExchangeAuthTokenRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authTokenRequest** | [**AuthTokenRequest**](AuthTokenRequest.md) |  | 

### Return type

[**AuthTokenResponse**](AuthTokenResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetCurrentUser

> AuthMeResponse GetCurrentUser(ctx).Execute()

Get Current User

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
	resp, r, err := apiClient.AuthAPI.GetCurrentUser(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.GetCurrentUser``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetCurrentUser`: AuthMeResponse
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.GetCurrentUser`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetCurrentUserRequest struct via the builder pattern


### Return type

[**AuthMeResponse**](AuthMeResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## Logout

> AuthMessageResponse Logout(ctx).Execute()

Logout



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
	resp, r, err := apiClient.AuthAPI.Logout(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.Logout``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `Logout`: AuthMessageResponse
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.Logout`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiLogoutRequest struct via the builder pattern


### Return type

[**AuthMessageResponse**](AuthMessageResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RefreshAccessToken

> AuthRefreshResponse RefreshAccessToken(ctx).AuthRefreshRequest(authRefreshRequest).Execute()

Refresh Access Token



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
	authRefreshRequest := *openapiclient.NewAuthRefreshRequest("RefreshToken_example") // AuthRefreshRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.RefreshAccessToken(context.Background()).AuthRefreshRequest(authRefreshRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.RefreshAccessToken``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RefreshAccessToken`: AuthRefreshResponse
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.RefreshAccessToken`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRefreshAccessTokenRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authRefreshRequest** | [**AuthRefreshRequest**](AuthRefreshRequest.md) |  | 

### Return type

[**AuthRefreshResponse**](AuthRefreshResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## Register

> AuthRegisterResponse Register(ctx).AuthRegisterRequest(authRegisterRequest).Execute()

Register



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
	authRegisterRequest := *openapiclient.NewAuthRegisterRequest("IdToken_example") // AuthRegisterRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.Register(context.Background()).AuthRegisterRequest(authRegisterRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.Register``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `Register`: AuthRegisterResponse
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.Register`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRegisterRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authRegisterRequest** | [**AuthRegisterRequest**](AuthRegisterRequest.md) |  | 

### Return type

[**AuthRegisterResponse**](AuthRegisterResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RequestPasswordReset

> AuthMessageResponse RequestPasswordReset(ctx).AuthForgotPasswordRequest(authForgotPasswordRequest).Execute()

Request Password Reset



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
	authForgotPasswordRequest := *openapiclient.NewAuthForgotPasswordRequest("Email_example") // AuthForgotPasswordRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.RequestPasswordReset(context.Background()).AuthForgotPasswordRequest(authForgotPasswordRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.RequestPasswordReset``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RequestPasswordReset`: AuthMessageResponse
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.RequestPasswordReset`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRequestPasswordResetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authForgotPasswordRequest** | [**AuthForgotPasswordRequest**](AuthForgotPasswordRequest.md) |  | 

### Return type

[**AuthMessageResponse**](AuthMessageResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ResetPassword

> AuthMessageResponse ResetPassword(ctx).AuthResetPasswordRequest(authResetPasswordRequest).Execute()

Reset Password



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
	authResetPasswordRequest := *openapiclient.NewAuthResetPasswordRequest("OobCode_example", "NewPassword_example") // AuthResetPasswordRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.ResetPassword(context.Background()).AuthResetPasswordRequest(authResetPasswordRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.ResetPassword``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ResetPassword`: AuthMessageResponse
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.ResetPassword`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiResetPasswordRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authResetPasswordRequest** | [**AuthResetPasswordRequest**](AuthResetPasswordRequest.md) |  | 

### Return type

[**AuthMessageResponse**](AuthMessageResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateCurrentUser

> AuthMeResponse UpdateCurrentUser(ctx).AuthMePatchRequest(authMePatchRequest).Execute()

Update Current User



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
	authMePatchRequest := *openapiclient.NewAuthMePatchRequest() // AuthMePatchRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.UpdateCurrentUser(context.Background()).AuthMePatchRequest(authMePatchRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.UpdateCurrentUser``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateCurrentUser`: AuthMeResponse
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.UpdateCurrentUser`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiUpdateCurrentUserRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authMePatchRequest** | [**AuthMePatchRequest**](AuthMePatchRequest.md) |  | 

### Return type

[**AuthMeResponse**](AuthMeResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

