# TemplateCreateRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** |  | 
**Description** | Pointer to **NullableString** |  | [optional] 
**BaseTemplateId** | Pointer to **string** |  | [optional] [default to "tpl_modern"]
**Config** | Pointer to **map[string]interface{}** |  | [optional] 

## Methods

### NewTemplateCreateRequest

`func NewTemplateCreateRequest(name string, ) *TemplateCreateRequest`

NewTemplateCreateRequest instantiates a new TemplateCreateRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTemplateCreateRequestWithDefaults

`func NewTemplateCreateRequestWithDefaults() *TemplateCreateRequest`

NewTemplateCreateRequestWithDefaults instantiates a new TemplateCreateRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *TemplateCreateRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *TemplateCreateRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *TemplateCreateRequest) SetName(v string)`

SetName sets Name field to given value.


### GetDescription

`func (o *TemplateCreateRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *TemplateCreateRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *TemplateCreateRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *TemplateCreateRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *TemplateCreateRequest) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *TemplateCreateRequest) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetBaseTemplateId

`func (o *TemplateCreateRequest) GetBaseTemplateId() string`

GetBaseTemplateId returns the BaseTemplateId field if non-nil, zero value otherwise.

### GetBaseTemplateIdOk

`func (o *TemplateCreateRequest) GetBaseTemplateIdOk() (*string, bool)`

GetBaseTemplateIdOk returns a tuple with the BaseTemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBaseTemplateId

`func (o *TemplateCreateRequest) SetBaseTemplateId(v string)`

SetBaseTemplateId sets BaseTemplateId field to given value.

### HasBaseTemplateId

`func (o *TemplateCreateRequest) HasBaseTemplateId() bool`

HasBaseTemplateId returns a boolean if a field has been set.

### GetConfig

`func (o *TemplateCreateRequest) GetConfig() map[string]interface{}`

GetConfig returns the Config field if non-nil, zero value otherwise.

### GetConfigOk

`func (o *TemplateCreateRequest) GetConfigOk() (*map[string]interface{}, bool)`

GetConfigOk returns a tuple with the Config field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConfig

`func (o *TemplateCreateRequest) SetConfig(v map[string]interface{})`

SetConfig sets Config field to given value.

### HasConfig

`func (o *TemplateCreateRequest) HasConfig() bool`

HasConfig returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


