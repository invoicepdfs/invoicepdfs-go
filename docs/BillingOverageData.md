# BillingOverageData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**OverageEnabled** | **bool** |  | 
**OverageAvailable** | **bool** |  | 
**OveragePriceMillicents** | Pointer to **NullableInt32** |  | [optional] 

## Methods

### NewBillingOverageData

`func NewBillingOverageData(overageEnabled bool, overageAvailable bool, ) *BillingOverageData`

NewBillingOverageData instantiates a new BillingOverageData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBillingOverageDataWithDefaults

`func NewBillingOverageDataWithDefaults() *BillingOverageData`

NewBillingOverageDataWithDefaults instantiates a new BillingOverageData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetOverageEnabled

`func (o *BillingOverageData) GetOverageEnabled() bool`

GetOverageEnabled returns the OverageEnabled field if non-nil, zero value otherwise.

### GetOverageEnabledOk

`func (o *BillingOverageData) GetOverageEnabledOk() (*bool, bool)`

GetOverageEnabledOk returns a tuple with the OverageEnabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOverageEnabled

`func (o *BillingOverageData) SetOverageEnabled(v bool)`

SetOverageEnabled sets OverageEnabled field to given value.


### GetOverageAvailable

`func (o *BillingOverageData) GetOverageAvailable() bool`

GetOverageAvailable returns the OverageAvailable field if non-nil, zero value otherwise.

### GetOverageAvailableOk

`func (o *BillingOverageData) GetOverageAvailableOk() (*bool, bool)`

GetOverageAvailableOk returns a tuple with the OverageAvailable field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOverageAvailable

`func (o *BillingOverageData) SetOverageAvailable(v bool)`

SetOverageAvailable sets OverageAvailable field to given value.


### GetOveragePriceMillicents

`func (o *BillingOverageData) GetOveragePriceMillicents() int32`

GetOveragePriceMillicents returns the OveragePriceMillicents field if non-nil, zero value otherwise.

### GetOveragePriceMillicentsOk

`func (o *BillingOverageData) GetOveragePriceMillicentsOk() (*int32, bool)`

GetOveragePriceMillicentsOk returns a tuple with the OveragePriceMillicents field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOveragePriceMillicents

`func (o *BillingOverageData) SetOveragePriceMillicents(v int32)`

SetOveragePriceMillicents sets OveragePriceMillicents field to given value.

### HasOveragePriceMillicents

`func (o *BillingOverageData) HasOveragePriceMillicents() bool`

HasOveragePriceMillicents returns a boolean if a field has been set.

### SetOveragePriceMillicentsNil

`func (o *BillingOverageData) SetOveragePriceMillicentsNil(b bool)`

 SetOveragePriceMillicentsNil sets the value for OveragePriceMillicents to be an explicit nil

### UnsetOveragePriceMillicents
`func (o *BillingOverageData) UnsetOveragePriceMillicents()`

UnsetOveragePriceMillicents ensures that no value is present for OveragePriceMillicents, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


