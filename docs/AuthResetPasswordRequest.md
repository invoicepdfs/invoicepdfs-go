# AuthResetPasswordRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**OobCode** | **string** | Code from the password reset email | 
**NewPassword** | **string** | New password | 

## Methods

### NewAuthResetPasswordRequest

`func NewAuthResetPasswordRequest(oobCode string, newPassword string, ) *AuthResetPasswordRequest`

NewAuthResetPasswordRequest instantiates a new AuthResetPasswordRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAuthResetPasswordRequestWithDefaults

`func NewAuthResetPasswordRequestWithDefaults() *AuthResetPasswordRequest`

NewAuthResetPasswordRequestWithDefaults instantiates a new AuthResetPasswordRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetOobCode

`func (o *AuthResetPasswordRequest) GetOobCode() string`

GetOobCode returns the OobCode field if non-nil, zero value otherwise.

### GetOobCodeOk

`func (o *AuthResetPasswordRequest) GetOobCodeOk() (*string, bool)`

GetOobCodeOk returns a tuple with the OobCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOobCode

`func (o *AuthResetPasswordRequest) SetOobCode(v string)`

SetOobCode sets OobCode field to given value.


### GetNewPassword

`func (o *AuthResetPasswordRequest) GetNewPassword() string`

GetNewPassword returns the NewPassword field if non-nil, zero value otherwise.

### GetNewPasswordOk

`func (o *AuthResetPasswordRequest) GetNewPasswordOk() (*string, bool)`

GetNewPasswordOk returns a tuple with the NewPassword field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNewPassword

`func (o *AuthResetPasswordRequest) SetNewPassword(v string)`

SetNewPassword sets NewPassword field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


