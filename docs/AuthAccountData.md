# AuthAccountData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AccountId** | **string** |  | 
**Name** | **string** |  | 
**Email** | Pointer to **NullableString** |  | [optional] 
**PlanId** | **string** |  | 
**PlanName** | **string** |  | 

## Methods

### NewAuthAccountData

`func NewAuthAccountData(accountId string, name string, planId string, planName string, ) *AuthAccountData`

NewAuthAccountData instantiates a new AuthAccountData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAuthAccountDataWithDefaults

`func NewAuthAccountDataWithDefaults() *AuthAccountData`

NewAuthAccountDataWithDefaults instantiates a new AuthAccountData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAccountId

`func (o *AuthAccountData) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *AuthAccountData) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *AuthAccountData) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.


### GetName

`func (o *AuthAccountData) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *AuthAccountData) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *AuthAccountData) SetName(v string)`

SetName sets Name field to given value.


### GetEmail

`func (o *AuthAccountData) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *AuthAccountData) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *AuthAccountData) SetEmail(v string)`

SetEmail sets Email field to given value.

### HasEmail

`func (o *AuthAccountData) HasEmail() bool`

HasEmail returns a boolean if a field has been set.

### SetEmailNil

`func (o *AuthAccountData) SetEmailNil(b bool)`

 SetEmailNil sets the value for Email to be an explicit nil

### UnsetEmail
`func (o *AuthAccountData) UnsetEmail()`

UnsetEmail ensures that no value is present for Email, not even an explicit nil
### GetPlanId

`func (o *AuthAccountData) GetPlanId() string`

GetPlanId returns the PlanId field if non-nil, zero value otherwise.

### GetPlanIdOk

`func (o *AuthAccountData) GetPlanIdOk() (*string, bool)`

GetPlanIdOk returns a tuple with the PlanId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPlanId

`func (o *AuthAccountData) SetPlanId(v string)`

SetPlanId sets PlanId field to given value.


### GetPlanName

`func (o *AuthAccountData) GetPlanName() string`

GetPlanName returns the PlanName field if non-nil, zero value otherwise.

### GetPlanNameOk

`func (o *AuthAccountData) GetPlanNameOk() (*string, bool)`

GetPlanNameOk returns a tuple with the PlanName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPlanName

`func (o *AuthAccountData) SetPlanName(v string)`

SetPlanName sets PlanName field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


