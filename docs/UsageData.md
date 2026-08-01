# UsageData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Period** | [**UsagePeriod**](UsagePeriod.md) |  | 
**Renders** | [**UsageRenders**](UsageRenders.md) |  | 

## Methods

### NewUsageData

`func NewUsageData(period UsagePeriod, renders UsageRenders, ) *UsageData`

NewUsageData instantiates a new UsageData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUsageDataWithDefaults

`func NewUsageDataWithDefaults() *UsageData`

NewUsageDataWithDefaults instantiates a new UsageData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPeriod

`func (o *UsageData) GetPeriod() UsagePeriod`

GetPeriod returns the Period field if non-nil, zero value otherwise.

### GetPeriodOk

`func (o *UsageData) GetPeriodOk() (*UsagePeriod, bool)`

GetPeriodOk returns a tuple with the Period field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPeriod

`func (o *UsageData) SetPeriod(v UsagePeriod)`

SetPeriod sets Period field to given value.


### GetRenders

`func (o *UsageData) GetRenders() UsageRenders`

GetRenders returns the Renders field if non-nil, zero value otherwise.

### GetRendersOk

`func (o *UsageData) GetRendersOk() (*UsageRenders, bool)`

GetRendersOk returns a tuple with the Renders field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRenders

`func (o *UsageData) SetRenders(v UsageRenders)`

SetRenders sets Renders field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


