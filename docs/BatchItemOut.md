# BatchItemOut

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**ExternalId** | Pointer to **NullableString** |  | [optional] 
**DocumentType** | **string** |  | 
**Status** | **string** |  | 
**RenderId** | Pointer to **NullableString** |  | [optional] 
**ErrorMessage** | Pointer to **NullableString** |  | [optional] 
**CreatedAt** | **string** |  | 

## Methods

### NewBatchItemOut

`func NewBatchItemOut(id string, documentType string, status string, createdAt string, ) *BatchItemOut`

NewBatchItemOut instantiates a new BatchItemOut object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBatchItemOutWithDefaults

`func NewBatchItemOutWithDefaults() *BatchItemOut`

NewBatchItemOutWithDefaults instantiates a new BatchItemOut object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *BatchItemOut) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *BatchItemOut) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *BatchItemOut) SetId(v string)`

SetId sets Id field to given value.


### GetExternalId

`func (o *BatchItemOut) GetExternalId() string`

GetExternalId returns the ExternalId field if non-nil, zero value otherwise.

### GetExternalIdOk

`func (o *BatchItemOut) GetExternalIdOk() (*string, bool)`

GetExternalIdOk returns a tuple with the ExternalId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExternalId

`func (o *BatchItemOut) SetExternalId(v string)`

SetExternalId sets ExternalId field to given value.

### HasExternalId

`func (o *BatchItemOut) HasExternalId() bool`

HasExternalId returns a boolean if a field has been set.

### SetExternalIdNil

`func (o *BatchItemOut) SetExternalIdNil(b bool)`

 SetExternalIdNil sets the value for ExternalId to be an explicit nil

### UnsetExternalId
`func (o *BatchItemOut) UnsetExternalId()`

UnsetExternalId ensures that no value is present for ExternalId, not even an explicit nil
### GetDocumentType

`func (o *BatchItemOut) GetDocumentType() string`

GetDocumentType returns the DocumentType field if non-nil, zero value otherwise.

### GetDocumentTypeOk

`func (o *BatchItemOut) GetDocumentTypeOk() (*string, bool)`

GetDocumentTypeOk returns a tuple with the DocumentType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDocumentType

`func (o *BatchItemOut) SetDocumentType(v string)`

SetDocumentType sets DocumentType field to given value.


### GetStatus

`func (o *BatchItemOut) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *BatchItemOut) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *BatchItemOut) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetRenderId

`func (o *BatchItemOut) GetRenderId() string`

GetRenderId returns the RenderId field if non-nil, zero value otherwise.

### GetRenderIdOk

`func (o *BatchItemOut) GetRenderIdOk() (*string, bool)`

GetRenderIdOk returns a tuple with the RenderId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRenderId

`func (o *BatchItemOut) SetRenderId(v string)`

SetRenderId sets RenderId field to given value.

### HasRenderId

`func (o *BatchItemOut) HasRenderId() bool`

HasRenderId returns a boolean if a field has been set.

### SetRenderIdNil

`func (o *BatchItemOut) SetRenderIdNil(b bool)`

 SetRenderIdNil sets the value for RenderId to be an explicit nil

### UnsetRenderId
`func (o *BatchItemOut) UnsetRenderId()`

UnsetRenderId ensures that no value is present for RenderId, not even an explicit nil
### GetErrorMessage

`func (o *BatchItemOut) GetErrorMessage() string`

GetErrorMessage returns the ErrorMessage field if non-nil, zero value otherwise.

### GetErrorMessageOk

`func (o *BatchItemOut) GetErrorMessageOk() (*string, bool)`

GetErrorMessageOk returns a tuple with the ErrorMessage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrorMessage

`func (o *BatchItemOut) SetErrorMessage(v string)`

SetErrorMessage sets ErrorMessage field to given value.

### HasErrorMessage

`func (o *BatchItemOut) HasErrorMessage() bool`

HasErrorMessage returns a boolean if a field has been set.

### SetErrorMessageNil

`func (o *BatchItemOut) SetErrorMessageNil(b bool)`

 SetErrorMessageNil sets the value for ErrorMessage to be an explicit nil

### UnsetErrorMessage
`func (o *BatchItemOut) UnsetErrorMessage()`

UnsetErrorMessage ensures that no value is present for ErrorMessage, not even an explicit nil
### GetCreatedAt

`func (o *BatchItemOut) GetCreatedAt() string`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *BatchItemOut) GetCreatedAtOk() (*string, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *BatchItemOut) SetCreatedAt(v string)`

SetCreatedAt sets CreatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


