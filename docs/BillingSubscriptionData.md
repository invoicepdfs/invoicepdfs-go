# BillingSubscriptionData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**SubscriptionId** | Pointer to **NullableString** |  | [optional] 
**Status** | Pointer to **NullableString** |  | [optional] 
**PlanId** | **string** |  | 
**PlanName** | **string** |  | 
**StripeConfigured** | Pointer to **bool** |  | [optional] [default to false]
**HasBillingAccount** | Pointer to **bool** |  | [optional] [default to false]
**OverageEnabled** | Pointer to **bool** |  | [optional] [default to false]
**OverageAvailable** | Pointer to **bool** |  | [optional] [default to false]
**OveragePriceMillicents** | Pointer to **NullableInt32** |  | [optional] 

## Methods

### NewBillingSubscriptionData

`func NewBillingSubscriptionData(planId string, planName string, ) *BillingSubscriptionData`

NewBillingSubscriptionData instantiates a new BillingSubscriptionData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBillingSubscriptionDataWithDefaults

`func NewBillingSubscriptionDataWithDefaults() *BillingSubscriptionData`

NewBillingSubscriptionDataWithDefaults instantiates a new BillingSubscriptionData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSubscriptionId

`func (o *BillingSubscriptionData) GetSubscriptionId() string`

GetSubscriptionId returns the SubscriptionId field if non-nil, zero value otherwise.

### GetSubscriptionIdOk

`func (o *BillingSubscriptionData) GetSubscriptionIdOk() (*string, bool)`

GetSubscriptionIdOk returns a tuple with the SubscriptionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubscriptionId

`func (o *BillingSubscriptionData) SetSubscriptionId(v string)`

SetSubscriptionId sets SubscriptionId field to given value.

### HasSubscriptionId

`func (o *BillingSubscriptionData) HasSubscriptionId() bool`

HasSubscriptionId returns a boolean if a field has been set.

### SetSubscriptionIdNil

`func (o *BillingSubscriptionData) SetSubscriptionIdNil(b bool)`

 SetSubscriptionIdNil sets the value for SubscriptionId to be an explicit nil

### UnsetSubscriptionId
`func (o *BillingSubscriptionData) UnsetSubscriptionId()`

UnsetSubscriptionId ensures that no value is present for SubscriptionId, not even an explicit nil
### GetStatus

`func (o *BillingSubscriptionData) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *BillingSubscriptionData) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *BillingSubscriptionData) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *BillingSubscriptionData) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### SetStatusNil

`func (o *BillingSubscriptionData) SetStatusNil(b bool)`

 SetStatusNil sets the value for Status to be an explicit nil

### UnsetStatus
`func (o *BillingSubscriptionData) UnsetStatus()`

UnsetStatus ensures that no value is present for Status, not even an explicit nil
### GetPlanId

`func (o *BillingSubscriptionData) GetPlanId() string`

GetPlanId returns the PlanId field if non-nil, zero value otherwise.

### GetPlanIdOk

`func (o *BillingSubscriptionData) GetPlanIdOk() (*string, bool)`

GetPlanIdOk returns a tuple with the PlanId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPlanId

`func (o *BillingSubscriptionData) SetPlanId(v string)`

SetPlanId sets PlanId field to given value.


### GetPlanName

`func (o *BillingSubscriptionData) GetPlanName() string`

GetPlanName returns the PlanName field if non-nil, zero value otherwise.

### GetPlanNameOk

`func (o *BillingSubscriptionData) GetPlanNameOk() (*string, bool)`

GetPlanNameOk returns a tuple with the PlanName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPlanName

`func (o *BillingSubscriptionData) SetPlanName(v string)`

SetPlanName sets PlanName field to given value.


### GetStripeConfigured

`func (o *BillingSubscriptionData) GetStripeConfigured() bool`

GetStripeConfigured returns the StripeConfigured field if non-nil, zero value otherwise.

### GetStripeConfiguredOk

`func (o *BillingSubscriptionData) GetStripeConfiguredOk() (*bool, bool)`

GetStripeConfiguredOk returns a tuple with the StripeConfigured field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStripeConfigured

`func (o *BillingSubscriptionData) SetStripeConfigured(v bool)`

SetStripeConfigured sets StripeConfigured field to given value.

### HasStripeConfigured

`func (o *BillingSubscriptionData) HasStripeConfigured() bool`

HasStripeConfigured returns a boolean if a field has been set.

### GetHasBillingAccount

`func (o *BillingSubscriptionData) GetHasBillingAccount() bool`

GetHasBillingAccount returns the HasBillingAccount field if non-nil, zero value otherwise.

### GetHasBillingAccountOk

`func (o *BillingSubscriptionData) GetHasBillingAccountOk() (*bool, bool)`

GetHasBillingAccountOk returns a tuple with the HasBillingAccount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasBillingAccount

`func (o *BillingSubscriptionData) SetHasBillingAccount(v bool)`

SetHasBillingAccount sets HasBillingAccount field to given value.

### HasHasBillingAccount

`func (o *BillingSubscriptionData) HasHasBillingAccount() bool`

HasHasBillingAccount returns a boolean if a field has been set.

### GetOverageEnabled

`func (o *BillingSubscriptionData) GetOverageEnabled() bool`

GetOverageEnabled returns the OverageEnabled field if non-nil, zero value otherwise.

### GetOverageEnabledOk

`func (o *BillingSubscriptionData) GetOverageEnabledOk() (*bool, bool)`

GetOverageEnabledOk returns a tuple with the OverageEnabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOverageEnabled

`func (o *BillingSubscriptionData) SetOverageEnabled(v bool)`

SetOverageEnabled sets OverageEnabled field to given value.

### HasOverageEnabled

`func (o *BillingSubscriptionData) HasOverageEnabled() bool`

HasOverageEnabled returns a boolean if a field has been set.

### GetOverageAvailable

`func (o *BillingSubscriptionData) GetOverageAvailable() bool`

GetOverageAvailable returns the OverageAvailable field if non-nil, zero value otherwise.

### GetOverageAvailableOk

`func (o *BillingSubscriptionData) GetOverageAvailableOk() (*bool, bool)`

GetOverageAvailableOk returns a tuple with the OverageAvailable field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOverageAvailable

`func (o *BillingSubscriptionData) SetOverageAvailable(v bool)`

SetOverageAvailable sets OverageAvailable field to given value.

### HasOverageAvailable

`func (o *BillingSubscriptionData) HasOverageAvailable() bool`

HasOverageAvailable returns a boolean if a field has been set.

### GetOveragePriceMillicents

`func (o *BillingSubscriptionData) GetOveragePriceMillicents() int32`

GetOveragePriceMillicents returns the OveragePriceMillicents field if non-nil, zero value otherwise.

### GetOveragePriceMillicentsOk

`func (o *BillingSubscriptionData) GetOveragePriceMillicentsOk() (*int32, bool)`

GetOveragePriceMillicentsOk returns a tuple with the OveragePriceMillicents field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOveragePriceMillicents

`func (o *BillingSubscriptionData) SetOveragePriceMillicents(v int32)`

SetOveragePriceMillicents sets OveragePriceMillicents field to given value.

### HasOveragePriceMillicents

`func (o *BillingSubscriptionData) HasOveragePriceMillicents() bool`

HasOveragePriceMillicents returns a boolean if a field has been set.

### SetOveragePriceMillicentsNil

`func (o *BillingSubscriptionData) SetOveragePriceMillicentsNil(b bool)`

 SetOveragePriceMillicentsNil sets the value for OveragePriceMillicents to be an explicit nil

### UnsetOveragePriceMillicents
`func (o *BillingSubscriptionData) UnsetOveragePriceMillicents()`

UnsetOveragePriceMillicents ensures that no value is present for OveragePriceMillicents, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


