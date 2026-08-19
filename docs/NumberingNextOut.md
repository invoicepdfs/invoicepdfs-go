# NumberingNextOut

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Number** | **string** |  | 
**SequenceId** | **string** |  | 
**NextNumber** | **int32** | The counter after this allocation | 

## Methods

### NewNumberingNextOut

`func NewNumberingNextOut(number string, sequenceId string, nextNumber int32, ) *NumberingNextOut`

NewNumberingNextOut instantiates a new NumberingNextOut object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewNumberingNextOutWithDefaults

`func NewNumberingNextOutWithDefaults() *NumberingNextOut`

NewNumberingNextOutWithDefaults instantiates a new NumberingNextOut object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetNumber

`func (o *NumberingNextOut) GetNumber() string`

GetNumber returns the Number field if non-nil, zero value otherwise.

### GetNumberOk

`func (o *NumberingNextOut) GetNumberOk() (*string, bool)`

GetNumberOk returns a tuple with the Number field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNumber

`func (o *NumberingNextOut) SetNumber(v string)`

SetNumber sets Number field to given value.


### GetSequenceId

`func (o *NumberingNextOut) GetSequenceId() string`

GetSequenceId returns the SequenceId field if non-nil, zero value otherwise.

### GetSequenceIdOk

`func (o *NumberingNextOut) GetSequenceIdOk() (*string, bool)`

GetSequenceIdOk returns a tuple with the SequenceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSequenceId

`func (o *NumberingNextOut) SetSequenceId(v string)`

SetSequenceId sets SequenceId field to given value.


### GetNextNumber

`func (o *NumberingNextOut) GetNextNumber() int32`

GetNextNumber returns the NextNumber field if non-nil, zero value otherwise.

### GetNextNumberOk

`func (o *NumberingNextOut) GetNextNumberOk() (*int32, bool)`

GetNextNumberOk returns a tuple with the NextNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextNumber

`func (o *NumberingNextOut) SetNextNumber(v int32)`

SetNextNumber sets NextNumber field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


