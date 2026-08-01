# \AuthAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ForgotPasswordApiV1AuthForgotPasswordPost**](AuthAPI.md#ForgotPasswordApiV1AuthForgotPasswordPost) | **Post** /api/v1/auth/forgot-password | Forgot Password
[**LogoutApiV1AuthLogoutPost**](AuthAPI.md#LogoutApiV1AuthLogoutPost) | **Post** /api/v1/auth/logout | Logout
[**MeApiV1AuthMeGet**](AuthAPI.md#MeApiV1AuthMeGet) | **Get** /api/v1/auth/me | Me
[**PatchMeApiV1AuthMePatch**](AuthAPI.md#PatchMeApiV1AuthMePatch) | **Patch** /api/v1/auth/me | Patch Me
[**RefreshApiV1AuthRefreshPost**](AuthAPI.md#RefreshApiV1AuthRefreshPost) | **Post** /api/v1/auth/refresh | Refresh
[**RegisterApiV1AuthRegisterPost**](AuthAPI.md#RegisterApiV1AuthRegisterPost) | **Post** /api/v1/auth/register | Register
[**ResetPasswordApiV1AuthResetPasswordPost**](AuthAPI.md#ResetPasswordApiV1AuthResetPasswordPost) | **Post** /api/v1/auth/reset-password | Reset Password
[**TokenExchangeApiV1AuthTokenPost**](AuthAPI.md#TokenExchangeApiV1AuthTokenPost) | **Post** /api/v1/auth/token | Token Exchange



## ForgotPasswordApiV1AuthForgotPasswordPost

> AuthMessageResponse ForgotPasswordApiV1AuthForgotPasswordPost(ctx).AuthForgotPasswordRequest(authForgotPasswordRequest).Execute()

Forgot Password



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/invoicepdfs"
)

func main() {
	authForgotPasswordRequest := *openapiclient.NewAuthForgotPasswordRequest("Email_example") // AuthForgotPasswordRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.ForgotPasswordApiV1AuthForgotPasswordPost(context.Background()).AuthForgotPasswordRequest(authForgotPasswordRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.ForgotPasswordApiV1AuthForgotPasswordPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ForgotPasswordApiV1AuthForgotPasswordPost`: AuthMessageResponse
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.ForgotPasswordApiV1AuthForgotPasswordPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiForgotPasswordApiV1AuthForgotPasswordPostRequest struct via the builder pattern


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


## LogoutApiV1AuthLogoutPost

> AuthMessageResponse LogoutApiV1AuthLogoutPost(ctx).Execute()

Logout



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/invoicepdfs"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.LogoutApiV1AuthLogoutPost(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.LogoutApiV1AuthLogoutPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LogoutApiV1AuthLogoutPost`: AuthMessageResponse
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.LogoutApiV1AuthLogoutPost`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiLogoutApiV1AuthLogoutPostRequest struct via the builder pattern


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


## MeApiV1AuthMeGet

> AuthMeResponse MeApiV1AuthMeGet(ctx).Execute()

Me

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/invoicepdfs"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.MeApiV1AuthMeGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.MeApiV1AuthMeGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MeApiV1AuthMeGet`: AuthMeResponse
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.MeApiV1AuthMeGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiMeApiV1AuthMeGetRequest struct via the builder pattern


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


## PatchMeApiV1AuthMePatch

> AuthMeResponse PatchMeApiV1AuthMePatch(ctx).AuthMePatchRequest(authMePatchRequest).Execute()

Patch Me



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/invoicepdfs"
)

func main() {
	authMePatchRequest := *openapiclient.NewAuthMePatchRequest() // AuthMePatchRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.PatchMeApiV1AuthMePatch(context.Background()).AuthMePatchRequest(authMePatchRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.PatchMeApiV1AuthMePatch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PatchMeApiV1AuthMePatch`: AuthMeResponse
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.PatchMeApiV1AuthMePatch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiPatchMeApiV1AuthMePatchRequest struct via the builder pattern


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


## RefreshApiV1AuthRefreshPost

> AuthRefreshResponse RefreshApiV1AuthRefreshPost(ctx).AuthRefreshRequest(authRefreshRequest).Execute()

Refresh



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/invoicepdfs"
)

func main() {
	authRefreshRequest := *openapiclient.NewAuthRefreshRequest("RefreshToken_example") // AuthRefreshRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.RefreshApiV1AuthRefreshPost(context.Background()).AuthRefreshRequest(authRefreshRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.RefreshApiV1AuthRefreshPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RefreshApiV1AuthRefreshPost`: AuthRefreshResponse
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.RefreshApiV1AuthRefreshPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRefreshApiV1AuthRefreshPostRequest struct via the builder pattern


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


## RegisterApiV1AuthRegisterPost

> AuthRegisterResponse RegisterApiV1AuthRegisterPost(ctx).AuthRegisterRequest(authRegisterRequest).Execute()

Register



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/invoicepdfs"
)

func main() {
	authRegisterRequest := *openapiclient.NewAuthRegisterRequest("IdToken_example") // AuthRegisterRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.RegisterApiV1AuthRegisterPost(context.Background()).AuthRegisterRequest(authRegisterRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.RegisterApiV1AuthRegisterPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RegisterApiV1AuthRegisterPost`: AuthRegisterResponse
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.RegisterApiV1AuthRegisterPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRegisterApiV1AuthRegisterPostRequest struct via the builder pattern


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


## ResetPasswordApiV1AuthResetPasswordPost

> AuthMessageResponse ResetPasswordApiV1AuthResetPasswordPost(ctx).AuthResetPasswordRequest(authResetPasswordRequest).Execute()

Reset Password



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/invoicepdfs"
)

func main() {
	authResetPasswordRequest := *openapiclient.NewAuthResetPasswordRequest("OobCode_example", "NewPassword_example") // AuthResetPasswordRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.ResetPasswordApiV1AuthResetPasswordPost(context.Background()).AuthResetPasswordRequest(authResetPasswordRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.ResetPasswordApiV1AuthResetPasswordPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ResetPasswordApiV1AuthResetPasswordPost`: AuthMessageResponse
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.ResetPasswordApiV1AuthResetPasswordPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiResetPasswordApiV1AuthResetPasswordPostRequest struct via the builder pattern


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


## TokenExchangeApiV1AuthTokenPost

> AuthTokenResponse TokenExchangeApiV1AuthTokenPost(ctx).AuthTokenRequest(authTokenRequest).Execute()

Token Exchange



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/invoicepdfs"
)

func main() {
	authTokenRequest := *openapiclient.NewAuthTokenRequest("IdToken_example") // AuthTokenRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.TokenExchangeApiV1AuthTokenPost(context.Background()).AuthTokenRequest(authTokenRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.TokenExchangeApiV1AuthTokenPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TokenExchangeApiV1AuthTokenPost`: AuthTokenResponse
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.TokenExchangeApiV1AuthTokenPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTokenExchangeApiV1AuthTokenPostRequest struct via the builder pattern


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

