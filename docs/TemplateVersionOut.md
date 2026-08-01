# TemplateVersionOut

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**TemplateId** | **string** |  | 
**Version** | **int32** |  | 
**Label** | Pointer to **NullableString** |  | [optional] 
**Changelog** | Pointer to **NullableString** |  | [optional] 
**Config** | **map[string]interface{}** |  | 
**CreatedAt** | **string** |  | 

## Methods

### NewTemplateVersionOut

`func NewTemplateVersionOut(id string, templateId string, version int32, config map[string]interface{}, createdAt string, ) *TemplateVersionOut`

NewTemplateVersionOut instantiates a new TemplateVersionOut object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTemplateVersionOutWithDefaults

`func NewTemplateVersionOutWithDefaults() *TemplateVersionOut`

NewTemplateVersionOutWithDefaults instantiates a new TemplateVersionOut object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *TemplateVersionOut) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *TemplateVersionOut) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *TemplateVersionOut) SetId(v string)`

SetId sets Id field to given value.


### GetTemplateId

`func (o *TemplateVersionOut) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *TemplateVersionOut) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *TemplateVersionOut) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.


### GetVersion

`func (o *TemplateVersionOut) GetVersion() int32`

GetVersion returns the Version field if non-nil, zero value otherwise.

### GetVersionOk

`func (o *TemplateVersionOut) GetVersionOk() (*int32, bool)`

GetVersionOk returns a tuple with the Version field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersion

`func (o *TemplateVersionOut) SetVersion(v int32)`

SetVersion sets Version field to given value.


### GetLabel

`func (o *TemplateVersionOut) GetLabel() string`

GetLabel returns the Label field if non-nil, zero value otherwise.

### GetLabelOk

`func (o *TemplateVersionOut) GetLabelOk() (*string, bool)`

GetLabelOk returns a tuple with the Label field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabel

`func (o *TemplateVersionOut) SetLabel(v string)`

SetLabel sets Label field to given value.

### HasLabel

`func (o *TemplateVersionOut) HasLabel() bool`

HasLabel returns a boolean if a field has been set.

### SetLabelNil

`func (o *TemplateVersionOut) SetLabelNil(b bool)`

 SetLabelNil sets the value for Label to be an explicit nil

### UnsetLabel
`func (o *TemplateVersionOut) UnsetLabel()`

UnsetLabel ensures that no value is present for Label, not even an explicit nil
### GetChangelog

`func (o *TemplateVersionOut) GetChangelog() string`

GetChangelog returns the Changelog field if non-nil, zero value otherwise.

### GetChangelogOk

`func (o *TemplateVersionOut) GetChangelogOk() (*string, bool)`

GetChangelogOk returns a tuple with the Changelog field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChangelog

`func (o *TemplateVersionOut) SetChangelog(v string)`

SetChangelog sets Changelog field to given value.

### HasChangelog

`func (o *TemplateVersionOut) HasChangelog() bool`

HasChangelog returns a boolean if a field has been set.

### SetChangelogNil

`func (o *TemplateVersionOut) SetChangelogNil(b bool)`

 SetChangelogNil sets the value for Changelog to be an explicit nil

### UnsetChangelog
`func (o *TemplateVersionOut) UnsetChangelog()`

UnsetChangelog ensures that no value is present for Changelog, not even an explicit nil
### GetConfig

`func (o *TemplateVersionOut) GetConfig() map[string]interface{}`

GetConfig returns the Config field if non-nil, zero value otherwise.

### GetConfigOk

`func (o *TemplateVersionOut) GetConfigOk() (*map[string]interface{}, bool)`

GetConfigOk returns a tuple with the Config field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConfig

`func (o *TemplateVersionOut) SetConfig(v map[string]interface{})`

SetConfig sets Config field to given value.


### GetCreatedAt

`func (o *TemplateVersionOut) GetCreatedAt() string`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *TemplateVersionOut) GetCreatedAtOk() (*string, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *TemplateVersionOut) SetCreatedAt(v string)`

SetCreatedAt sets CreatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


