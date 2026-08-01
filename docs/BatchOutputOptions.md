# BatchOutputOptions

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Format** | Pointer to **string** |  | [optional] [default to "pdf"]
**Combine** | Pointer to **bool** |  | [optional] [default to false]
**ArchiveFormat** | Pointer to **string** |  | [optional] [default to "zip"]

## Methods

### NewBatchOutputOptions

`func NewBatchOutputOptions() *BatchOutputOptions`

NewBatchOutputOptions instantiates a new BatchOutputOptions object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBatchOutputOptionsWithDefaults

`func NewBatchOutputOptionsWithDefaults() *BatchOutputOptions`

NewBatchOutputOptionsWithDefaults instantiates a new BatchOutputOptions object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetFormat

`func (o *BatchOutputOptions) GetFormat() string`

GetFormat returns the Format field if non-nil, zero value otherwise.

### GetFormatOk

`func (o *BatchOutputOptions) GetFormatOk() (*string, bool)`

GetFormatOk returns a tuple with the Format field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFormat

`func (o *BatchOutputOptions) SetFormat(v string)`

SetFormat sets Format field to given value.

### HasFormat

`func (o *BatchOutputOptions) HasFormat() bool`

HasFormat returns a boolean if a field has been set.

### GetCombine

`func (o *BatchOutputOptions) GetCombine() bool`

GetCombine returns the Combine field if non-nil, zero value otherwise.

### GetCombineOk

`func (o *BatchOutputOptions) GetCombineOk() (*bool, bool)`

GetCombineOk returns a tuple with the Combine field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCombine

`func (o *BatchOutputOptions) SetCombine(v bool)`

SetCombine sets Combine field to given value.

### HasCombine

`func (o *BatchOutputOptions) HasCombine() bool`

HasCombine returns a boolean if a field has been set.

### GetArchiveFormat

`func (o *BatchOutputOptions) GetArchiveFormat() string`

GetArchiveFormat returns the ArchiveFormat field if non-nil, zero value otherwise.

### GetArchiveFormatOk

`func (o *BatchOutputOptions) GetArchiveFormatOk() (*string, bool)`

GetArchiveFormatOk returns a tuple with the ArchiveFormat field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArchiveFormat

`func (o *BatchOutputOptions) SetArchiveFormat(v string)`

SetArchiveFormat sets ArchiveFormat field to given value.

### HasArchiveFormat

`func (o *BatchOutputOptions) HasArchiveFormat() bool`

HasArchiveFormat returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


