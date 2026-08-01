# ImportCreateRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**SourceFormat** | **string** |  | 
**Data** | **[]map[string]interface{}** |  | 

## Methods

### NewImportCreateRequest

`func NewImportCreateRequest(sourceFormat string, data []map[string]interface{}, ) *ImportCreateRequest`

NewImportCreateRequest instantiates a new ImportCreateRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewImportCreateRequestWithDefaults

`func NewImportCreateRequestWithDefaults() *ImportCreateRequest`

NewImportCreateRequestWithDefaults instantiates a new ImportCreateRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSourceFormat

`func (o *ImportCreateRequest) GetSourceFormat() string`

GetSourceFormat returns the SourceFormat field if non-nil, zero value otherwise.

### GetSourceFormatOk

`func (o *ImportCreateRequest) GetSourceFormatOk() (*string, bool)`

GetSourceFormatOk returns a tuple with the SourceFormat field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceFormat

`func (o *ImportCreateRequest) SetSourceFormat(v string)`

SetSourceFormat sets SourceFormat field to given value.


### GetData

`func (o *ImportCreateRequest) GetData() []map[string]interface{}`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *ImportCreateRequest) GetDataOk() (*[]map[string]interface{}, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *ImportCreateRequest) SetData(v []map[string]interface{})`

SetData sets Data field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


