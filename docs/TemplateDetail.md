# TemplateDetail

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TemplateId** | **string** |  | 
**Name** | **string** |  | 
**DocumentType** | Pointer to **string** |  | [optional] [default to "invoice"]
**Engine** | **string** |  | 

## Methods

### NewTemplateDetail

`func NewTemplateDetail(templateId string, name string, engine string, ) *TemplateDetail`

NewTemplateDetail instantiates a new TemplateDetail object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTemplateDetailWithDefaults

`func NewTemplateDetailWithDefaults() *TemplateDetail`

NewTemplateDetailWithDefaults instantiates a new TemplateDetail object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTemplateId

`func (o *TemplateDetail) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *TemplateDetail) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *TemplateDetail) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.


### GetName

`func (o *TemplateDetail) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *TemplateDetail) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *TemplateDetail) SetName(v string)`

SetName sets Name field to given value.


### GetDocumentType

`func (o *TemplateDetail) GetDocumentType() string`

GetDocumentType returns the DocumentType field if non-nil, zero value otherwise.

### GetDocumentTypeOk

`func (o *TemplateDetail) GetDocumentTypeOk() (*string, bool)`

GetDocumentTypeOk returns a tuple with the DocumentType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDocumentType

`func (o *TemplateDetail) SetDocumentType(v string)`

SetDocumentType sets DocumentType field to given value.

### HasDocumentType

`func (o *TemplateDetail) HasDocumentType() bool`

HasDocumentType returns a boolean if a field has been set.

### GetEngine

`func (o *TemplateDetail) GetEngine() string`

GetEngine returns the Engine field if non-nil, zero value otherwise.

### GetEngineOk

`func (o *TemplateDetail) GetEngineOk() (*string, bool)`

GetEngineOk returns a tuple with the Engine field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEngine

`func (o *TemplateDetail) SetEngine(v string)`

SetEngine sets Engine field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


