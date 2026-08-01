# NumberingSequencePatchRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **NullableString** |  | [optional] 
**Prefix** | Pointer to **NullableString** |  | [optional] 
**DatePattern** | Pointer to **NullableString** |  | [optional] 
**Padding** | Pointer to **NullableInt32** |  | [optional] 
**NextNumber** | Pointer to **NullableInt32** |  | [optional] 
**Reset** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewNumberingSequencePatchRequest

`func NewNumberingSequencePatchRequest() *NumberingSequencePatchRequest`

NewNumberingSequencePatchRequest instantiates a new NumberingSequencePatchRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewNumberingSequencePatchRequestWithDefaults

`func NewNumberingSequencePatchRequestWithDefaults() *NumberingSequencePatchRequest`

NewNumberingSequencePatchRequestWithDefaults instantiates a new NumberingSequencePatchRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *NumberingSequencePatchRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *NumberingSequencePatchRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *NumberingSequencePatchRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *NumberingSequencePatchRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### SetNameNil

`func (o *NumberingSequencePatchRequest) SetNameNil(b bool)`

 SetNameNil sets the value for Name to be an explicit nil

### UnsetName
`func (o *NumberingSequencePatchRequest) UnsetName()`

UnsetName ensures that no value is present for Name, not even an explicit nil
### GetPrefix

`func (o *NumberingSequencePatchRequest) GetPrefix() string`

GetPrefix returns the Prefix field if non-nil, zero value otherwise.

### GetPrefixOk

`func (o *NumberingSequencePatchRequest) GetPrefixOk() (*string, bool)`

GetPrefixOk returns a tuple with the Prefix field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrefix

`func (o *NumberingSequencePatchRequest) SetPrefix(v string)`

SetPrefix sets Prefix field to given value.

### HasPrefix

`func (o *NumberingSequencePatchRequest) HasPrefix() bool`

HasPrefix returns a boolean if a field has been set.

### SetPrefixNil

`func (o *NumberingSequencePatchRequest) SetPrefixNil(b bool)`

 SetPrefixNil sets the value for Prefix to be an explicit nil

### UnsetPrefix
`func (o *NumberingSequencePatchRequest) UnsetPrefix()`

UnsetPrefix ensures that no value is present for Prefix, not even an explicit nil
### GetDatePattern

`func (o *NumberingSequencePatchRequest) GetDatePattern() string`

GetDatePattern returns the DatePattern field if non-nil, zero value otherwise.

### GetDatePatternOk

`func (o *NumberingSequencePatchRequest) GetDatePatternOk() (*string, bool)`

GetDatePatternOk returns a tuple with the DatePattern field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDatePattern

`func (o *NumberingSequencePatchRequest) SetDatePattern(v string)`

SetDatePattern sets DatePattern field to given value.

### HasDatePattern

`func (o *NumberingSequencePatchRequest) HasDatePattern() bool`

HasDatePattern returns a boolean if a field has been set.

### SetDatePatternNil

`func (o *NumberingSequencePatchRequest) SetDatePatternNil(b bool)`

 SetDatePatternNil sets the value for DatePattern to be an explicit nil

### UnsetDatePattern
`func (o *NumberingSequencePatchRequest) UnsetDatePattern()`

UnsetDatePattern ensures that no value is present for DatePattern, not even an explicit nil
### GetPadding

`func (o *NumberingSequencePatchRequest) GetPadding() int32`

GetPadding returns the Padding field if non-nil, zero value otherwise.

### GetPaddingOk

`func (o *NumberingSequencePatchRequest) GetPaddingOk() (*int32, bool)`

GetPaddingOk returns a tuple with the Padding field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPadding

`func (o *NumberingSequencePatchRequest) SetPadding(v int32)`

SetPadding sets Padding field to given value.

### HasPadding

`func (o *NumberingSequencePatchRequest) HasPadding() bool`

HasPadding returns a boolean if a field has been set.

### SetPaddingNil

`func (o *NumberingSequencePatchRequest) SetPaddingNil(b bool)`

 SetPaddingNil sets the value for Padding to be an explicit nil

### UnsetPadding
`func (o *NumberingSequencePatchRequest) UnsetPadding()`

UnsetPadding ensures that no value is present for Padding, not even an explicit nil
### GetNextNumber

`func (o *NumberingSequencePatchRequest) GetNextNumber() int32`

GetNextNumber returns the NextNumber field if non-nil, zero value otherwise.

### GetNextNumberOk

`func (o *NumberingSequencePatchRequest) GetNextNumberOk() (*int32, bool)`

GetNextNumberOk returns a tuple with the NextNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextNumber

`func (o *NumberingSequencePatchRequest) SetNextNumber(v int32)`

SetNextNumber sets NextNumber field to given value.

### HasNextNumber

`func (o *NumberingSequencePatchRequest) HasNextNumber() bool`

HasNextNumber returns a boolean if a field has been set.

### SetNextNumberNil

`func (o *NumberingSequencePatchRequest) SetNextNumberNil(b bool)`

 SetNextNumberNil sets the value for NextNumber to be an explicit nil

### UnsetNextNumber
`func (o *NumberingSequencePatchRequest) UnsetNextNumber()`

UnsetNextNumber ensures that no value is present for NextNumber, not even an explicit nil
### GetReset

`func (o *NumberingSequencePatchRequest) GetReset() string`

GetReset returns the Reset field if non-nil, zero value otherwise.

### GetResetOk

`func (o *NumberingSequencePatchRequest) GetResetOk() (*string, bool)`

GetResetOk returns a tuple with the Reset field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReset

`func (o *NumberingSequencePatchRequest) SetReset(v string)`

SetReset sets Reset field to given value.

### HasReset

`func (o *NumberingSequencePatchRequest) HasReset() bool`

HasReset returns a boolean if a field has been set.

### SetResetNil

`func (o *NumberingSequencePatchRequest) SetResetNil(b bool)`

 SetResetNil sets the value for Reset to be an explicit nil

### UnsetReset
`func (o *NumberingSequencePatchRequest) UnsetReset()`

UnsetReset ensures that no value is present for Reset, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


