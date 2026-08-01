# DocumentCalculateRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**DocumentType** | Pointer to **string** |  | [optional] [default to "invoice"]
**Data** | [**DocumentInvoiceDataInput**](DocumentInvoiceDataInput.md) |  | 

## Methods

### NewDocumentCalculateRequest

`func NewDocumentCalculateRequest(data DocumentInvoiceDataInput, ) *DocumentCalculateRequest`

NewDocumentCalculateRequest instantiates a new DocumentCalculateRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDocumentCalculateRequestWithDefaults

`func NewDocumentCalculateRequestWithDefaults() *DocumentCalculateRequest`

NewDocumentCalculateRequestWithDefaults instantiates a new DocumentCalculateRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDocumentType

`func (o *DocumentCalculateRequest) GetDocumentType() string`

GetDocumentType returns the DocumentType field if non-nil, zero value otherwise.

### GetDocumentTypeOk

`func (o *DocumentCalculateRequest) GetDocumentTypeOk() (*string, bool)`

GetDocumentTypeOk returns a tuple with the DocumentType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDocumentType

`func (o *DocumentCalculateRequest) SetDocumentType(v string)`

SetDocumentType sets DocumentType field to given value.

### HasDocumentType

`func (o *DocumentCalculateRequest) HasDocumentType() bool`

HasDocumentType returns a boolean if a field has been set.

### GetData

`func (o *DocumentCalculateRequest) GetData() DocumentInvoiceDataInput`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *DocumentCalculateRequest) GetDataOk() (*DocumentInvoiceDataInput, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *DocumentCalculateRequest) SetData(v DocumentInvoiceDataInput)`

SetData sets Data field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


