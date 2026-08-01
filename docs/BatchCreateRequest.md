# BatchCreateRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Operation** | Pointer to **string** |  | [optional] [default to "render"]
**Items** | [**[]BatchItemInput**](BatchItemInput.md) |  | 
**TemplateId** | Pointer to **string** |  | [optional] [default to "tpl_modern"]
**Output** | Pointer to [**BatchOutputOptions**](BatchOutputOptions.md) |  | [optional] 

## Methods

### NewBatchCreateRequest

`func NewBatchCreateRequest(items []BatchItemInput, ) *BatchCreateRequest`

NewBatchCreateRequest instantiates a new BatchCreateRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBatchCreateRequestWithDefaults

`func NewBatchCreateRequestWithDefaults() *BatchCreateRequest`

NewBatchCreateRequestWithDefaults instantiates a new BatchCreateRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetOperation

`func (o *BatchCreateRequest) GetOperation() string`

GetOperation returns the Operation field if non-nil, zero value otherwise.

### GetOperationOk

`func (o *BatchCreateRequest) GetOperationOk() (*string, bool)`

GetOperationOk returns a tuple with the Operation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOperation

`func (o *BatchCreateRequest) SetOperation(v string)`

SetOperation sets Operation field to given value.

### HasOperation

`func (o *BatchCreateRequest) HasOperation() bool`

HasOperation returns a boolean if a field has been set.

### GetItems

`func (o *BatchCreateRequest) GetItems() []BatchItemInput`

GetItems returns the Items field if non-nil, zero value otherwise.

### GetItemsOk

`func (o *BatchCreateRequest) GetItemsOk() (*[]BatchItemInput, bool)`

GetItemsOk returns a tuple with the Items field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItems

`func (o *BatchCreateRequest) SetItems(v []BatchItemInput)`

SetItems sets Items field to given value.


### GetTemplateId

`func (o *BatchCreateRequest) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *BatchCreateRequest) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *BatchCreateRequest) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.

### HasTemplateId

`func (o *BatchCreateRequest) HasTemplateId() bool`

HasTemplateId returns a boolean if a field has been set.

### GetOutput

`func (o *BatchCreateRequest) GetOutput() BatchOutputOptions`

GetOutput returns the Output field if non-nil, zero value otherwise.

### GetOutputOk

`func (o *BatchCreateRequest) GetOutputOk() (*BatchOutputOptions, bool)`

GetOutputOk returns a tuple with the Output field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOutput

`func (o *BatchCreateRequest) SetOutput(v BatchOutputOptions)`

SetOutput sets Output field to given value.

### HasOutput

`func (o *BatchCreateRequest) HasOutput() bool`

HasOutput returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


