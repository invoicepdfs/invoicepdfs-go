# AuthTokenRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**IdToken** | **string** | Firebase ID token from client-side auth | 

## Methods

### NewAuthTokenRequest

`func NewAuthTokenRequest(idToken string, ) *AuthTokenRequest`

NewAuthTokenRequest instantiates a new AuthTokenRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAuthTokenRequestWithDefaults

`func NewAuthTokenRequestWithDefaults() *AuthTokenRequest`

NewAuthTokenRequestWithDefaults instantiates a new AuthTokenRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetIdToken

`func (o *AuthTokenRequest) GetIdToken() string`

GetIdToken returns the IdToken field if non-nil, zero value otherwise.

### GetIdTokenOk

`func (o *AuthTokenRequest) GetIdTokenOk() (*string, bool)`

GetIdTokenOk returns a tuple with the IdToken field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIdToken

`func (o *AuthTokenRequest) SetIdToken(v string)`

SetIdToken sets IdToken field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


