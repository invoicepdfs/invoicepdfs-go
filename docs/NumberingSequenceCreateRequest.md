# NumberingSequenceCreateRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** |  | 
**DocumentType** | Pointer to **string** |  | [optional] [default to "invoice"]
**Prefix** | Pointer to **string** |  | [optional] [default to "INV-"]
**DatePattern** | Pointer to **string** |  | [optional] [default to "{YYYY}-"]
**Padding** | Pointer to **int32** |  | [optional] [default to 5]
**NextNumber** | Pointer to **int32** |  | [optional] [default to 1]
**Reset** | Pointer to **string** |  | [optional] [default to "yearly"]

## Methods

### NewNumberingSequenceCreateRequest

`func NewNumberingSequenceCreateRequest(name string, ) *NumberingSequenceCreateRequest`

NewNumberingSequenceCreateRequest instantiates a new NumberingSequenceCreateRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewNumberingSequenceCreateRequestWithDefaults

`func NewNumberingSequenceCreateRequestWithDefaults() *NumberingSequenceCreateRequest`

NewNumberingSequenceCreateRequestWithDefaults instantiates a new NumberingSequenceCreateRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *NumberingSequenceCreateRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *NumberingSequenceCreateRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *NumberingSequenceCreateRequest) SetName(v string)`

SetName sets Name field to given value.


### GetDocumentType

`func (o *NumberingSequenceCreateRequest) GetDocumentType() string`

GetDocumentType returns the DocumentType field if non-nil, zero value otherwise.

### GetDocumentTypeOk

`func (o *NumberingSequenceCreateRequest) GetDocumentTypeOk() (*string, bool)`

GetDocumentTypeOk returns a tuple with the DocumentType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDocumentType

`func (o *NumberingSequenceCreateRequest) SetDocumentType(v string)`

SetDocumentType sets DocumentType field to given value.

### HasDocumentType

`func (o *NumberingSequenceCreateRequest) HasDocumentType() bool`

HasDocumentType returns a boolean if a field has been set.

### GetPrefix

`func (o *NumberingSequenceCreateRequest) GetPrefix() string`

GetPrefix returns the Prefix field if non-nil, zero value otherwise.

### GetPrefixOk

`func (o *NumberingSequenceCreateRequest) GetPrefixOk() (*string, bool)`

GetPrefixOk returns a tuple with the Prefix field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrefix

`func (o *NumberingSequenceCreateRequest) SetPrefix(v string)`

SetPrefix sets Prefix field to given value.

### HasPrefix

`func (o *NumberingSequenceCreateRequest) HasPrefix() bool`

HasPrefix returns a boolean if a field has been set.

### GetDatePattern

`func (o *NumberingSequenceCreateRequest) GetDatePattern() string`

GetDatePattern returns the DatePattern field if non-nil, zero value otherwise.

### GetDatePatternOk

`func (o *NumberingSequenceCreateRequest) GetDatePatternOk() (*string, bool)`

GetDatePatternOk returns a tuple with the DatePattern field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDatePattern

`func (o *NumberingSequenceCreateRequest) SetDatePattern(v string)`

SetDatePattern sets DatePattern field to given value.

### HasDatePattern

`func (o *NumberingSequenceCreateRequest) HasDatePattern() bool`

HasDatePattern returns a boolean if a field has been set.

### GetPadding

`func (o *NumberingSequenceCreateRequest) GetPadding() int32`

GetPadding returns the Padding field if non-nil, zero value otherwise.

### GetPaddingOk

`func (o *NumberingSequenceCreateRequest) GetPaddingOk() (*int32, bool)`

GetPaddingOk returns a tuple with the Padding field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPadding

`func (o *NumberingSequenceCreateRequest) SetPadding(v int32)`

SetPadding sets Padding field to given value.

### HasPadding

`func (o *NumberingSequenceCreateRequest) HasPadding() bool`

HasPadding returns a boolean if a field has been set.

### GetNextNumber

`func (o *NumberingSequenceCreateRequest) GetNextNumber() int32`

GetNextNumber returns the NextNumber field if non-nil, zero value otherwise.

### GetNextNumberOk

`func (o *NumberingSequenceCreateRequest) GetNextNumberOk() (*int32, bool)`

GetNextNumberOk returns a tuple with the NextNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextNumber

`func (o *NumberingSequenceCreateRequest) SetNextNumber(v int32)`

SetNextNumber sets NextNumber field to given value.

### HasNextNumber

`func (o *NumberingSequenceCreateRequest) HasNextNumber() bool`

HasNextNumber returns a boolean if a field has been set.

### GetReset

`func (o *NumberingSequenceCreateRequest) GetReset() string`

GetReset returns the Reset field if non-nil, zero value otherwise.

### GetResetOk

`func (o *NumberingSequenceCreateRequest) GetResetOk() (*string, bool)`

GetResetOk returns a tuple with the Reset field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReset

`func (o *NumberingSequenceCreateRequest) SetReset(v string)`

SetReset sets Reset field to given value.

### HasReset

`func (o *NumberingSequenceCreateRequest) HasReset() bool`

HasReset returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


