# UsageOverage

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enabled** | Pointer to **bool** |  | [optional] [default to false]
**Available** | Pointer to **bool** |  | [optional] [default to false]
**Renders** | Pointer to **int32** |  | [optional] [default to 0]
**PriceMillicents** | Pointer to **NullableInt32** |  | [optional] 
**EstimatedCostCents** | Pointer to **int32** |  | [optional] [default to 0]

## Methods

### NewUsageOverage

`func NewUsageOverage() *UsageOverage`

NewUsageOverage instantiates a new UsageOverage object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUsageOverageWithDefaults

`func NewUsageOverageWithDefaults() *UsageOverage`

NewUsageOverageWithDefaults instantiates a new UsageOverage object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEnabled

`func (o *UsageOverage) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *UsageOverage) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *UsageOverage) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *UsageOverage) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.

### GetAvailable

`func (o *UsageOverage) GetAvailable() bool`

GetAvailable returns the Available field if non-nil, zero value otherwise.

### GetAvailableOk

`func (o *UsageOverage) GetAvailableOk() (*bool, bool)`

GetAvailableOk returns a tuple with the Available field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAvailable

`func (o *UsageOverage) SetAvailable(v bool)`

SetAvailable sets Available field to given value.

### HasAvailable

`func (o *UsageOverage) HasAvailable() bool`

HasAvailable returns a boolean if a field has been set.

### GetRenders

`func (o *UsageOverage) GetRenders() int32`

GetRenders returns the Renders field if non-nil, zero value otherwise.

### GetRendersOk

`func (o *UsageOverage) GetRendersOk() (*int32, bool)`

GetRendersOk returns a tuple with the Renders field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRenders

`func (o *UsageOverage) SetRenders(v int32)`

SetRenders sets Renders field to given value.

### HasRenders

`func (o *UsageOverage) HasRenders() bool`

HasRenders returns a boolean if a field has been set.

### GetPriceMillicents

`func (o *UsageOverage) GetPriceMillicents() int32`

GetPriceMillicents returns the PriceMillicents field if non-nil, zero value otherwise.

### GetPriceMillicentsOk

`func (o *UsageOverage) GetPriceMillicentsOk() (*int32, bool)`

GetPriceMillicentsOk returns a tuple with the PriceMillicents field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriceMillicents

`func (o *UsageOverage) SetPriceMillicents(v int32)`

SetPriceMillicents sets PriceMillicents field to given value.

### HasPriceMillicents

`func (o *UsageOverage) HasPriceMillicents() bool`

HasPriceMillicents returns a boolean if a field has been set.

### SetPriceMillicentsNil

`func (o *UsageOverage) SetPriceMillicentsNil(b bool)`

 SetPriceMillicentsNil sets the value for PriceMillicents to be an explicit nil

### UnsetPriceMillicents
`func (o *UsageOverage) UnsetPriceMillicents()`

UnsetPriceMillicents ensures that no value is present for PriceMillicents, not even an explicit nil
### GetEstimatedCostCents

`func (o *UsageOverage) GetEstimatedCostCents() int32`

GetEstimatedCostCents returns the EstimatedCostCents field if non-nil, zero value otherwise.

### GetEstimatedCostCentsOk

`func (o *UsageOverage) GetEstimatedCostCentsOk() (*int32, bool)`

GetEstimatedCostCentsOk returns a tuple with the EstimatedCostCents field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEstimatedCostCents

`func (o *UsageOverage) SetEstimatedCostCents(v int32)`

SetEstimatedCostCents sets EstimatedCostCents field to given value.

### HasEstimatedCostCents

`func (o *UsageOverage) HasEstimatedCostCents() bool`

HasEstimatedCostCents returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


