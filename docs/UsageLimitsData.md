# UsageLimitsData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Renders** | [**UsageRenderLimits**](UsageRenderLimits.md) |  | 
**RateLimit** | [**UsageRateLimit**](UsageRateLimit.md) |  | 

## Methods

### NewUsageLimitsData

`func NewUsageLimitsData(renders UsageRenderLimits, rateLimit UsageRateLimit, ) *UsageLimitsData`

NewUsageLimitsData instantiates a new UsageLimitsData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUsageLimitsDataWithDefaults

`func NewUsageLimitsDataWithDefaults() *UsageLimitsData`

NewUsageLimitsDataWithDefaults instantiates a new UsageLimitsData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRenders

`func (o *UsageLimitsData) GetRenders() UsageRenderLimits`

GetRenders returns the Renders field if non-nil, zero value otherwise.

### GetRendersOk

`func (o *UsageLimitsData) GetRendersOk() (*UsageRenderLimits, bool)`

GetRendersOk returns a tuple with the Renders field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRenders

`func (o *UsageLimitsData) SetRenders(v UsageRenderLimits)`

SetRenders sets Renders field to given value.


### GetRateLimit

`func (o *UsageLimitsData) GetRateLimit() UsageRateLimit`

GetRateLimit returns the RateLimit field if non-nil, zero value otherwise.

### GetRateLimitOk

`func (o *UsageLimitsData) GetRateLimitOk() (*UsageRateLimit, bool)`

GetRateLimitOk returns a tuple with the RateLimit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRateLimit

`func (o *UsageLimitsData) SetRateLimit(v UsageRateLimit)`

SetRateLimit sets RateLimit field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


