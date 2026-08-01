# AppSchemasV1DocumentRenderRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**DocumentType** | Pointer to **string** |  | [optional] [default to "invoice"]
**Data** | [**DocumentInvoiceDataInput**](DocumentInvoiceDataInput.md) |  | 
**Template** | [**DocumentTemplateRef**](DocumentTemplateRef.md) |  | 
**Output** | Pointer to [**DocumentOutputOptions**](DocumentOutputOptions.md) |  | [optional] 

## Methods

### NewAppSchemasV1DocumentRenderRequest

`func NewAppSchemasV1DocumentRenderRequest(data DocumentInvoiceDataInput, template DocumentTemplateRef, ) *AppSchemasV1DocumentRenderRequest`

NewAppSchemasV1DocumentRenderRequest instantiates a new AppSchemasV1DocumentRenderRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAppSchemasV1DocumentRenderRequestWithDefaults

`func NewAppSchemasV1DocumentRenderRequestWithDefaults() *AppSchemasV1DocumentRenderRequest`

NewAppSchemasV1DocumentRenderRequestWithDefaults instantiates a new AppSchemasV1DocumentRenderRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDocumentType

`func (o *AppSchemasV1DocumentRenderRequest) GetDocumentType() string`

GetDocumentType returns the DocumentType field if non-nil, zero value otherwise.

### GetDocumentTypeOk

`func (o *AppSchemasV1DocumentRenderRequest) GetDocumentTypeOk() (*string, bool)`

GetDocumentTypeOk returns a tuple with the DocumentType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDocumentType

`func (o *AppSchemasV1DocumentRenderRequest) SetDocumentType(v string)`

SetDocumentType sets DocumentType field to given value.

### HasDocumentType

`func (o *AppSchemasV1DocumentRenderRequest) HasDocumentType() bool`

HasDocumentType returns a boolean if a field has been set.

### GetData

`func (o *AppSchemasV1DocumentRenderRequest) GetData() DocumentInvoiceDataInput`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *AppSchemasV1DocumentRenderRequest) GetDataOk() (*DocumentInvoiceDataInput, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *AppSchemasV1DocumentRenderRequest) SetData(v DocumentInvoiceDataInput)`

SetData sets Data field to given value.


### GetTemplate

`func (o *AppSchemasV1DocumentRenderRequest) GetTemplate() DocumentTemplateRef`

GetTemplate returns the Template field if non-nil, zero value otherwise.

### GetTemplateOk

`func (o *AppSchemasV1DocumentRenderRequest) GetTemplateOk() (*DocumentTemplateRef, bool)`

GetTemplateOk returns a tuple with the Template field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplate

`func (o *AppSchemasV1DocumentRenderRequest) SetTemplate(v DocumentTemplateRef)`

SetTemplate sets Template field to given value.


### GetOutput

`func (o *AppSchemasV1DocumentRenderRequest) GetOutput() DocumentOutputOptions`

GetOutput returns the Output field if non-nil, zero value otherwise.

### GetOutputOk

`func (o *AppSchemasV1DocumentRenderRequest) GetOutputOk() (*DocumentOutputOptions, bool)`

GetOutputOk returns a tuple with the Output field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOutput

`func (o *AppSchemasV1DocumentRenderRequest) SetOutput(v DocumentOutputOptions)`

SetOutput sets Output field to given value.

### HasOutput

`func (o *AppSchemasV1DocumentRenderRequest) HasOutput() bool`

HasOutput returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


