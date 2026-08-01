# BatchOut

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Status** | **string** |  | 
**Operation** | **string** |  | 
**TemplateId** | **string** |  | 
**TotalItems** | **int32** |  | 
**CompletedItems** | **int32** |  | 
**FailedItems** | **int32** |  | 
**CreatedAt** | **string** |  | 
**UpdatedAt** | **string** |  | 
**CompletedAt** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewBatchOut

`func NewBatchOut(id string, status string, operation string, templateId string, totalItems int32, completedItems int32, failedItems int32, createdAt string, updatedAt string, ) *BatchOut`

NewBatchOut instantiates a new BatchOut object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBatchOutWithDefaults

`func NewBatchOutWithDefaults() *BatchOut`

NewBatchOutWithDefaults instantiates a new BatchOut object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *BatchOut) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *BatchOut) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *BatchOut) SetId(v string)`

SetId sets Id field to given value.


### GetStatus

`func (o *BatchOut) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *BatchOut) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *BatchOut) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetOperation

`func (o *BatchOut) GetOperation() string`

GetOperation returns the Operation field if non-nil, zero value otherwise.

### GetOperationOk

`func (o *BatchOut) GetOperationOk() (*string, bool)`

GetOperationOk returns a tuple with the Operation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOperation

`func (o *BatchOut) SetOperation(v string)`

SetOperation sets Operation field to given value.


### GetTemplateId

`func (o *BatchOut) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *BatchOut) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *BatchOut) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.


### GetTotalItems

`func (o *BatchOut) GetTotalItems() int32`

GetTotalItems returns the TotalItems field if non-nil, zero value otherwise.

### GetTotalItemsOk

`func (o *BatchOut) GetTotalItemsOk() (*int32, bool)`

GetTotalItemsOk returns a tuple with the TotalItems field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalItems

`func (o *BatchOut) SetTotalItems(v int32)`

SetTotalItems sets TotalItems field to given value.


### GetCompletedItems

`func (o *BatchOut) GetCompletedItems() int32`

GetCompletedItems returns the CompletedItems field if non-nil, zero value otherwise.

### GetCompletedItemsOk

`func (o *BatchOut) GetCompletedItemsOk() (*int32, bool)`

GetCompletedItemsOk returns a tuple with the CompletedItems field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCompletedItems

`func (o *BatchOut) SetCompletedItems(v int32)`

SetCompletedItems sets CompletedItems field to given value.


### GetFailedItems

`func (o *BatchOut) GetFailedItems() int32`

GetFailedItems returns the FailedItems field if non-nil, zero value otherwise.

### GetFailedItemsOk

`func (o *BatchOut) GetFailedItemsOk() (*int32, bool)`

GetFailedItemsOk returns a tuple with the FailedItems field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFailedItems

`func (o *BatchOut) SetFailedItems(v int32)`

SetFailedItems sets FailedItems field to given value.


### GetCreatedAt

`func (o *BatchOut) GetCreatedAt() string`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *BatchOut) GetCreatedAtOk() (*string, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *BatchOut) SetCreatedAt(v string)`

SetCreatedAt sets CreatedAt field to given value.


### GetUpdatedAt

`func (o *BatchOut) GetUpdatedAt() string`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *BatchOut) GetUpdatedAtOk() (*string, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *BatchOut) SetUpdatedAt(v string)`

SetUpdatedAt sets UpdatedAt field to given value.


### GetCompletedAt

`func (o *BatchOut) GetCompletedAt() string`

GetCompletedAt returns the CompletedAt field if non-nil, zero value otherwise.

### GetCompletedAtOk

`func (o *BatchOut) GetCompletedAtOk() (*string, bool)`

GetCompletedAtOk returns a tuple with the CompletedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCompletedAt

`func (o *BatchOut) SetCompletedAt(v string)`

SetCompletedAt sets CompletedAt field to given value.

### HasCompletedAt

`func (o *BatchOut) HasCompletedAt() bool`

HasCompletedAt returns a boolean if a field has been set.

### SetCompletedAtNil

`func (o *BatchOut) SetCompletedAtNil(b bool)`

 SetCompletedAtNil sets the value for CompletedAt to be an explicit nil

### UnsetCompletedAt
`func (o *BatchOut) UnsetCompletedAt()`

UnsetCompletedAt ensures that no value is present for CompletedAt, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


