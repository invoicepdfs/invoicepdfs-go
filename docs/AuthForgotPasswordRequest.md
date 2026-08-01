# AuthForgotPasswordRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Email** | **string** | Email address of the account | 

## Methods

### NewAuthForgotPasswordRequest

`func NewAuthForgotPasswordRequest(email string, ) *AuthForgotPasswordRequest`

NewAuthForgotPasswordRequest instantiates a new AuthForgotPasswordRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAuthForgotPasswordRequestWithDefaults

`func NewAuthForgotPasswordRequestWithDefaults() *AuthForgotPasswordRequest`

NewAuthForgotPasswordRequestWithDefaults instantiates a new AuthForgotPasswordRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEmail

`func (o *AuthForgotPasswordRequest) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *AuthForgotPasswordRequest) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *AuthForgotPasswordRequest) SetEmail(v string)`

SetEmail sets Email field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


