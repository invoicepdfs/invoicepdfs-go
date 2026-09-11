# CodeListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Data** | [**[]CodeOut**](CodeOut.md) |  | 
**Standard** | **string** | The code list these values come from. | 
**Exhaustive** | **bool** | Whether &#x60;data&#x60; is the complete list. When false it is a shortlist and other codes remain valid. | 

## Methods

### NewCodeListResponse

`func NewCodeListResponse(data []CodeOut, standard string, exhaustive bool, ) *CodeListResponse`

NewCodeListResponse instantiates a new CodeListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCodeListResponseWithDefaults

`func NewCodeListResponseWithDefaults() *CodeListResponse`

NewCodeListResponseWithDefaults instantiates a new CodeListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetData

`func (o *CodeListResponse) GetData() []CodeOut`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *CodeListResponse) GetDataOk() (*[]CodeOut, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *CodeListResponse) SetData(v []CodeOut)`

SetData sets Data field to given value.


### GetStandard

`func (o *CodeListResponse) GetStandard() string`

GetStandard returns the Standard field if non-nil, zero value otherwise.

### GetStandardOk

`func (o *CodeListResponse) GetStandardOk() (*string, bool)`

GetStandardOk returns a tuple with the Standard field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStandard

`func (o *CodeListResponse) SetStandard(v string)`

SetStandard sets Standard field to given value.


### GetExhaustive

`func (o *CodeListResponse) GetExhaustive() bool`

GetExhaustive returns the Exhaustive field if non-nil, zero value otherwise.

### GetExhaustiveOk

`func (o *CodeListResponse) GetExhaustiveOk() (*bool, bool)`

GetExhaustiveOk returns a tuple with the Exhaustive field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExhaustive

`func (o *CodeListResponse) SetExhaustive(v bool)`

SetExhaustive sets Exhaustive field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


