# CustomTemplateOut

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Name** | **string** |  | 
**Description** | Pointer to **NullableString** |  | [optional] 
**BaseTemplateId** | **string** |  | 
**Config** | Pointer to **map[string]interface{}** |  | [optional] 
**Status** | **string** |  | 
**IsDefault** | Pointer to **bool** |  | [optional] [default to false]
**CreatedAt** | **string** |  | 
**UpdatedAt** | **string** |  | 
**PublishedAt** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewCustomTemplateOut

`func NewCustomTemplateOut(id string, name string, baseTemplateId string, status string, createdAt string, updatedAt string, ) *CustomTemplateOut`

NewCustomTemplateOut instantiates a new CustomTemplateOut object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCustomTemplateOutWithDefaults

`func NewCustomTemplateOutWithDefaults() *CustomTemplateOut`

NewCustomTemplateOutWithDefaults instantiates a new CustomTemplateOut object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *CustomTemplateOut) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *CustomTemplateOut) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *CustomTemplateOut) SetId(v string)`

SetId sets Id field to given value.


### GetName

`func (o *CustomTemplateOut) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CustomTemplateOut) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CustomTemplateOut) SetName(v string)`

SetName sets Name field to given value.


### GetDescription

`func (o *CustomTemplateOut) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *CustomTemplateOut) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *CustomTemplateOut) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *CustomTemplateOut) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *CustomTemplateOut) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *CustomTemplateOut) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetBaseTemplateId

`func (o *CustomTemplateOut) GetBaseTemplateId() string`

GetBaseTemplateId returns the BaseTemplateId field if non-nil, zero value otherwise.

### GetBaseTemplateIdOk

`func (o *CustomTemplateOut) GetBaseTemplateIdOk() (*string, bool)`

GetBaseTemplateIdOk returns a tuple with the BaseTemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBaseTemplateId

`func (o *CustomTemplateOut) SetBaseTemplateId(v string)`

SetBaseTemplateId sets BaseTemplateId field to given value.


### GetConfig

`func (o *CustomTemplateOut) GetConfig() map[string]interface{}`

GetConfig returns the Config field if non-nil, zero value otherwise.

### GetConfigOk

`func (o *CustomTemplateOut) GetConfigOk() (*map[string]interface{}, bool)`

GetConfigOk returns a tuple with the Config field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConfig

`func (o *CustomTemplateOut) SetConfig(v map[string]interface{})`

SetConfig sets Config field to given value.

### HasConfig

`func (o *CustomTemplateOut) HasConfig() bool`

HasConfig returns a boolean if a field has been set.

### GetStatus

`func (o *CustomTemplateOut) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *CustomTemplateOut) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *CustomTemplateOut) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetIsDefault

`func (o *CustomTemplateOut) GetIsDefault() bool`

GetIsDefault returns the IsDefault field if non-nil, zero value otherwise.

### GetIsDefaultOk

`func (o *CustomTemplateOut) GetIsDefaultOk() (*bool, bool)`

GetIsDefaultOk returns a tuple with the IsDefault field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsDefault

`func (o *CustomTemplateOut) SetIsDefault(v bool)`

SetIsDefault sets IsDefault field to given value.

### HasIsDefault

`func (o *CustomTemplateOut) HasIsDefault() bool`

HasIsDefault returns a boolean if a field has been set.

### GetCreatedAt

`func (o *CustomTemplateOut) GetCreatedAt() string`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *CustomTemplateOut) GetCreatedAtOk() (*string, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *CustomTemplateOut) SetCreatedAt(v string)`

SetCreatedAt sets CreatedAt field to given value.


### GetUpdatedAt

`func (o *CustomTemplateOut) GetUpdatedAt() string`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *CustomTemplateOut) GetUpdatedAtOk() (*string, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *CustomTemplateOut) SetUpdatedAt(v string)`

SetUpdatedAt sets UpdatedAt field to given value.


### GetPublishedAt

`func (o *CustomTemplateOut) GetPublishedAt() string`

GetPublishedAt returns the PublishedAt field if non-nil, zero value otherwise.

### GetPublishedAtOk

`func (o *CustomTemplateOut) GetPublishedAtOk() (*string, bool)`

GetPublishedAtOk returns a tuple with the PublishedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPublishedAt

`func (o *CustomTemplateOut) SetPublishedAt(v string)`

SetPublishedAt sets PublishedAt field to given value.

### HasPublishedAt

`func (o *CustomTemplateOut) HasPublishedAt() bool`

HasPublishedAt returns a boolean if a field has been set.

### SetPublishedAtNil

`func (o *CustomTemplateOut) SetPublishedAtNil(b bool)`

 SetPublishedAtNil sets the value for PublishedAt to be an explicit nil

### UnsetPublishedAt
`func (o *CustomTemplateOut) UnsetPublishedAt()`

UnsetPublishedAt ensures that no value is present for PublishedAt, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


