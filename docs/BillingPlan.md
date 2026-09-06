# BillingPlan

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Name** | **string** |  | 
**PriceId** | **string** |  | 
**PriceIdAnnual** | Pointer to **NullableString** |  | [optional] 
**MonthlyRenderQuota** | **int32** |  | 
**AllowBrandingRemoval** | Pointer to **bool** |  | [optional] [default to false]
**OveragePriceMillicents** | Pointer to **NullableInt32** |  | [optional] 

## Methods

### NewBillingPlan

`func NewBillingPlan(id string, name string, priceId string, monthlyRenderQuota int32, ) *BillingPlan`

NewBillingPlan instantiates a new BillingPlan object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBillingPlanWithDefaults

`func NewBillingPlanWithDefaults() *BillingPlan`

NewBillingPlanWithDefaults instantiates a new BillingPlan object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *BillingPlan) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *BillingPlan) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *BillingPlan) SetId(v string)`

SetId sets Id field to given value.


### GetName

`func (o *BillingPlan) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *BillingPlan) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *BillingPlan) SetName(v string)`

SetName sets Name field to given value.


### GetPriceId

`func (o *BillingPlan) GetPriceId() string`

GetPriceId returns the PriceId field if non-nil, zero value otherwise.

### GetPriceIdOk

`func (o *BillingPlan) GetPriceIdOk() (*string, bool)`

GetPriceIdOk returns a tuple with the PriceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriceId

`func (o *BillingPlan) SetPriceId(v string)`

SetPriceId sets PriceId field to given value.


### GetPriceIdAnnual

`func (o *BillingPlan) GetPriceIdAnnual() string`

GetPriceIdAnnual returns the PriceIdAnnual field if non-nil, zero value otherwise.

### GetPriceIdAnnualOk

`func (o *BillingPlan) GetPriceIdAnnualOk() (*string, bool)`

GetPriceIdAnnualOk returns a tuple with the PriceIdAnnual field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriceIdAnnual

`func (o *BillingPlan) SetPriceIdAnnual(v string)`

SetPriceIdAnnual sets PriceIdAnnual field to given value.

### HasPriceIdAnnual

`func (o *BillingPlan) HasPriceIdAnnual() bool`

HasPriceIdAnnual returns a boolean if a field has been set.

### SetPriceIdAnnualNil

`func (o *BillingPlan) SetPriceIdAnnualNil(b bool)`

 SetPriceIdAnnualNil sets the value for PriceIdAnnual to be an explicit nil

### UnsetPriceIdAnnual
`func (o *BillingPlan) UnsetPriceIdAnnual()`

UnsetPriceIdAnnual ensures that no value is present for PriceIdAnnual, not even an explicit nil
### GetMonthlyRenderQuota

`func (o *BillingPlan) GetMonthlyRenderQuota() int32`

GetMonthlyRenderQuota returns the MonthlyRenderQuota field if non-nil, zero value otherwise.

### GetMonthlyRenderQuotaOk

`func (o *BillingPlan) GetMonthlyRenderQuotaOk() (*int32, bool)`

GetMonthlyRenderQuotaOk returns a tuple with the MonthlyRenderQuota field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMonthlyRenderQuota

`func (o *BillingPlan) SetMonthlyRenderQuota(v int32)`

SetMonthlyRenderQuota sets MonthlyRenderQuota field to given value.


### GetAllowBrandingRemoval

`func (o *BillingPlan) GetAllowBrandingRemoval() bool`

GetAllowBrandingRemoval returns the AllowBrandingRemoval field if non-nil, zero value otherwise.

### GetAllowBrandingRemovalOk

`func (o *BillingPlan) GetAllowBrandingRemovalOk() (*bool, bool)`

GetAllowBrandingRemovalOk returns a tuple with the AllowBrandingRemoval field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAllowBrandingRemoval

`func (o *BillingPlan) SetAllowBrandingRemoval(v bool)`

SetAllowBrandingRemoval sets AllowBrandingRemoval field to given value.

### HasAllowBrandingRemoval

`func (o *BillingPlan) HasAllowBrandingRemoval() bool`

HasAllowBrandingRemoval returns a boolean if a field has been set.

### GetOveragePriceMillicents

`func (o *BillingPlan) GetOveragePriceMillicents() int32`

GetOveragePriceMillicents returns the OveragePriceMillicents field if non-nil, zero value otherwise.

### GetOveragePriceMillicentsOk

`func (o *BillingPlan) GetOveragePriceMillicentsOk() (*int32, bool)`

GetOveragePriceMillicentsOk returns a tuple with the OveragePriceMillicents field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOveragePriceMillicents

`func (o *BillingPlan) SetOveragePriceMillicents(v int32)`

SetOveragePriceMillicents sets OveragePriceMillicents field to given value.

### HasOveragePriceMillicents

`func (o *BillingPlan) HasOveragePriceMillicents() bool`

HasOveragePriceMillicents returns a boolean if a field has been set.

### SetOveragePriceMillicentsNil

`func (o *BillingPlan) SetOveragePriceMillicentsNil(b bool)`

 SetOveragePriceMillicentsNil sets the value for OveragePriceMillicents to be an explicit nil

### UnsetOveragePriceMillicents
`func (o *BillingPlan) UnsetOveragePriceMillicents()`

UnsetOveragePriceMillicents ensures that no value is present for OveragePriceMillicents, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


