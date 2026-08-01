# ImportOut

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**SourceFormat** | **string** |  | 
**Status** | **string** |  | 
**TotalRows** | **int32** |  | 
**ImportedRows** | **int32** |  | 
**FailedRows** | **int32** |  | 
**Errors** | Pointer to **[]map[string]interface{}** |  | [optional] 
**CreatedAt** | **string** |  | 
**UpdatedAt** | **string** |  | 
**CompletedAt** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewImportOut

`func NewImportOut(id string, sourceFormat string, status string, totalRows int32, importedRows int32, failedRows int32, createdAt string, updatedAt string, ) *ImportOut`

NewImportOut instantiates a new ImportOut object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewImportOutWithDefaults

`func NewImportOutWithDefaults() *ImportOut`

NewImportOutWithDefaults instantiates a new ImportOut object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ImportOut) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ImportOut) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ImportOut) SetId(v string)`

SetId sets Id field to given value.


### GetSourceFormat

`func (o *ImportOut) GetSourceFormat() string`

GetSourceFormat returns the SourceFormat field if non-nil, zero value otherwise.

### GetSourceFormatOk

`func (o *ImportOut) GetSourceFormatOk() (*string, bool)`

GetSourceFormatOk returns a tuple with the SourceFormat field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceFormat

`func (o *ImportOut) SetSourceFormat(v string)`

SetSourceFormat sets SourceFormat field to given value.


### GetStatus

`func (o *ImportOut) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *ImportOut) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *ImportOut) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetTotalRows

`func (o *ImportOut) GetTotalRows() int32`

GetTotalRows returns the TotalRows field if non-nil, zero value otherwise.

### GetTotalRowsOk

`func (o *ImportOut) GetTotalRowsOk() (*int32, bool)`

GetTotalRowsOk returns a tuple with the TotalRows field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalRows

`func (o *ImportOut) SetTotalRows(v int32)`

SetTotalRows sets TotalRows field to given value.


### GetImportedRows

`func (o *ImportOut) GetImportedRows() int32`

GetImportedRows returns the ImportedRows field if non-nil, zero value otherwise.

### GetImportedRowsOk

`func (o *ImportOut) GetImportedRowsOk() (*int32, bool)`

GetImportedRowsOk returns a tuple with the ImportedRows field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetImportedRows

`func (o *ImportOut) SetImportedRows(v int32)`

SetImportedRows sets ImportedRows field to given value.


### GetFailedRows

`func (o *ImportOut) GetFailedRows() int32`

GetFailedRows returns the FailedRows field if non-nil, zero value otherwise.

### GetFailedRowsOk

`func (o *ImportOut) GetFailedRowsOk() (*int32, bool)`

GetFailedRowsOk returns a tuple with the FailedRows field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFailedRows

`func (o *ImportOut) SetFailedRows(v int32)`

SetFailedRows sets FailedRows field to given value.


### GetErrors

`func (o *ImportOut) GetErrors() []map[string]interface{}`

GetErrors returns the Errors field if non-nil, zero value otherwise.

### GetErrorsOk

`func (o *ImportOut) GetErrorsOk() (*[]map[string]interface{}, bool)`

GetErrorsOk returns a tuple with the Errors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrors

`func (o *ImportOut) SetErrors(v []map[string]interface{})`

SetErrors sets Errors field to given value.

### HasErrors

`func (o *ImportOut) HasErrors() bool`

HasErrors returns a boolean if a field has been set.

### SetErrorsNil

`func (o *ImportOut) SetErrorsNil(b bool)`

 SetErrorsNil sets the value for Errors to be an explicit nil

### UnsetErrors
`func (o *ImportOut) UnsetErrors()`

UnsetErrors ensures that no value is present for Errors, not even an explicit nil
### GetCreatedAt

`func (o *ImportOut) GetCreatedAt() string`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *ImportOut) GetCreatedAtOk() (*string, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *ImportOut) SetCreatedAt(v string)`

SetCreatedAt sets CreatedAt field to given value.


### GetUpdatedAt

`func (o *ImportOut) GetUpdatedAt() string`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *ImportOut) GetUpdatedAtOk() (*string, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *ImportOut) SetUpdatedAt(v string)`

SetUpdatedAt sets UpdatedAt field to given value.


### GetCompletedAt

`func (o *ImportOut) GetCompletedAt() string`

GetCompletedAt returns the CompletedAt field if non-nil, zero value otherwise.

### GetCompletedAtOk

`func (o *ImportOut) GetCompletedAtOk() (*string, bool)`

GetCompletedAtOk returns a tuple with the CompletedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCompletedAt

`func (o *ImportOut) SetCompletedAt(v string)`

SetCompletedAt sets CompletedAt field to given value.

### HasCompletedAt

`func (o *ImportOut) HasCompletedAt() bool`

HasCompletedAt returns a boolean if a field has been set.

### SetCompletedAtNil

`func (o *ImportOut) SetCompletedAtNil(b bool)`

 SetCompletedAtNil sets the value for CompletedAt to be an explicit nil

### UnsetCompletedAt
`func (o *ImportOut) UnsetCompletedAt()`

UnsetCompletedAt ensures that no value is present for CompletedAt, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


