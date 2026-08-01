# AuthRegisterRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**IdToken** | **string** | Firebase ID token from client-side auth | 
**Name** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewAuthRegisterRequest

`func NewAuthRegisterRequest(idToken string, ) *AuthRegisterRequest`

NewAuthRegisterRequest instantiates a new AuthRegisterRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAuthRegisterRequestWithDefaults

`func NewAuthRegisterRequestWithDefaults() *AuthRegisterRequest`

NewAuthRegisterRequestWithDefaults instantiates a new AuthRegisterRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetIdToken

`func (o *AuthRegisterRequest) GetIdToken() string`

GetIdToken returns the IdToken field if non-nil, zero value otherwise.

### GetIdTokenOk

`func (o *AuthRegisterRequest) GetIdTokenOk() (*string, bool)`

GetIdTokenOk returns a tuple with the IdToken field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIdToken

`func (o *AuthRegisterRequest) SetIdToken(v string)`

SetIdToken sets IdToken field to given value.


### GetName

`func (o *AuthRegisterRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *AuthRegisterRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *AuthRegisterRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *AuthRegisterRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### SetNameNil

`func (o *AuthRegisterRequest) SetNameNil(b bool)`

 SetNameNil sets the value for Name to be an explicit nil

### UnsetName
`func (o *AuthRegisterRequest) UnsetName()`

UnsetName ensures that no value is present for Name, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


