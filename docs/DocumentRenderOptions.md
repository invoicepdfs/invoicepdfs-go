# DocumentRenderOptions

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TemplateId** | Pointer to **string** |  | [optional] [default to "tpl_modern"]
**PageSize** | Pointer to **string** |  | [optional] [default to "LETTER"]
**ExpiresIn** | Pointer to **int32** |  | [optional] [default to 3600]

## Methods

### NewDocumentRenderOptions

`func NewDocumentRenderOptions() *DocumentRenderOptions`

NewDocumentRenderOptions instantiates a new DocumentRenderOptions object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDocumentRenderOptionsWithDefaults

`func NewDocumentRenderOptionsWithDefaults() *DocumentRenderOptions`

NewDocumentRenderOptionsWithDefaults instantiates a new DocumentRenderOptions object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTemplateId

`func (o *DocumentRenderOptions) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *DocumentRenderOptions) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *DocumentRenderOptions) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.

### HasTemplateId

`func (o *DocumentRenderOptions) HasTemplateId() bool`

HasTemplateId returns a boolean if a field has been set.

### GetPageSize

`func (o *DocumentRenderOptions) GetPageSize() string`

GetPageSize returns the PageSize field if non-nil, zero value otherwise.

### GetPageSizeOk

`func (o *DocumentRenderOptions) GetPageSizeOk() (*string, bool)`

GetPageSizeOk returns a tuple with the PageSize field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPageSize

`func (o *DocumentRenderOptions) SetPageSize(v string)`

SetPageSize sets PageSize field to given value.

### HasPageSize

`func (o *DocumentRenderOptions) HasPageSize() bool`

HasPageSize returns a boolean if a field has been set.

### GetExpiresIn

`func (o *DocumentRenderOptions) GetExpiresIn() int32`

GetExpiresIn returns the ExpiresIn field if non-nil, zero value otherwise.

### GetExpiresInOk

`func (o *DocumentRenderOptions) GetExpiresInOk() (*int32, bool)`

GetExpiresInOk returns a tuple with the ExpiresIn field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresIn

`func (o *DocumentRenderOptions) SetExpiresIn(v int32)`

SetExpiresIn sets ExpiresIn field to given value.

### HasExpiresIn

`func (o *DocumentRenderOptions) HasExpiresIn() bool`

HasExpiresIn returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


