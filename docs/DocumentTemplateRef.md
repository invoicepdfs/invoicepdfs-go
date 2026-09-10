# DocumentTemplateRef

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Version** | Pointer to **NullableInt32** |  | [optional] 

## Methods

### NewDocumentTemplateRef

`func NewDocumentTemplateRef(id string, ) *DocumentTemplateRef`

NewDocumentTemplateRef instantiates a new DocumentTemplateRef object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDocumentTemplateRefWithDefaults

`func NewDocumentTemplateRefWithDefaults() *DocumentTemplateRef`

NewDocumentTemplateRefWithDefaults instantiates a new DocumentTemplateRef object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *DocumentTemplateRef) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *DocumentTemplateRef) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *DocumentTemplateRef) SetId(v string)`

SetId sets Id field to given value.


### GetVersion

`func (o *DocumentTemplateRef) GetVersion() int32`

GetVersion returns the Version field if non-nil, zero value otherwise.

### GetVersionOk

`func (o *DocumentTemplateRef) GetVersionOk() (*int32, bool)`

GetVersionOk returns a tuple with the Version field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersion

`func (o *DocumentTemplateRef) SetVersion(v int32)`

SetVersion sets Version field to given value.

### HasVersion

`func (o *DocumentTemplateRef) HasVersion() bool`

HasVersion returns a boolean if a field has been set.

### SetVersionNil

`func (o *DocumentTemplateRef) SetVersionNil(b bool)`

 SetVersionNil sets the value for Version to be an explicit nil

### UnsetVersion
`func (o *DocumentTemplateRef) UnsetVersion()`

UnsetVersion ensures that no value is present for Version, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


