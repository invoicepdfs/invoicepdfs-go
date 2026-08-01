# AppDocumentsSchemasDocumentRenderRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TemplateId** | Pointer to **string** |  | [optional] [default to "tpl_modern"]
**PageSize** | Pointer to **string** |  | [optional] [default to "LETTER"]
**ExpiresIn** | Pointer to **int32** |  | [optional] [default to 3600]

## Methods

### NewAppDocumentsSchemasDocumentRenderRequest

`func NewAppDocumentsSchemasDocumentRenderRequest() *AppDocumentsSchemasDocumentRenderRequest`

NewAppDocumentsSchemasDocumentRenderRequest instantiates a new AppDocumentsSchemasDocumentRenderRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAppDocumentsSchemasDocumentRenderRequestWithDefaults

`func NewAppDocumentsSchemasDocumentRenderRequestWithDefaults() *AppDocumentsSchemasDocumentRenderRequest`

NewAppDocumentsSchemasDocumentRenderRequestWithDefaults instantiates a new AppDocumentsSchemasDocumentRenderRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTemplateId

`func (o *AppDocumentsSchemasDocumentRenderRequest) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *AppDocumentsSchemasDocumentRenderRequest) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *AppDocumentsSchemasDocumentRenderRequest) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.

### HasTemplateId

`func (o *AppDocumentsSchemasDocumentRenderRequest) HasTemplateId() bool`

HasTemplateId returns a boolean if a field has been set.

### GetPageSize

`func (o *AppDocumentsSchemasDocumentRenderRequest) GetPageSize() string`

GetPageSize returns the PageSize field if non-nil, zero value otherwise.

### GetPageSizeOk

`func (o *AppDocumentsSchemasDocumentRenderRequest) GetPageSizeOk() (*string, bool)`

GetPageSizeOk returns a tuple with the PageSize field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPageSize

`func (o *AppDocumentsSchemasDocumentRenderRequest) SetPageSize(v string)`

SetPageSize sets PageSize field to given value.

### HasPageSize

`func (o *AppDocumentsSchemasDocumentRenderRequest) HasPageSize() bool`

HasPageSize returns a boolean if a field has been set.

### GetExpiresIn

`func (o *AppDocumentsSchemasDocumentRenderRequest) GetExpiresIn() int32`

GetExpiresIn returns the ExpiresIn field if non-nil, zero value otherwise.

### GetExpiresInOk

`func (o *AppDocumentsSchemasDocumentRenderRequest) GetExpiresInOk() (*int32, bool)`

GetExpiresInOk returns a tuple with the ExpiresIn field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresIn

`func (o *AppDocumentsSchemasDocumentRenderRequest) SetExpiresIn(v int32)`

SetExpiresIn sets ExpiresIn field to given value.

### HasExpiresIn

`func (o *AppDocumentsSchemasDocumentRenderRequest) HasExpiresIn() bool`

HasExpiresIn returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


