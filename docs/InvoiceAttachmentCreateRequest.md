# InvoiceAttachmentCreateRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**FileId** | **string** |  | 
**Label** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewInvoiceAttachmentCreateRequest

`func NewInvoiceAttachmentCreateRequest(fileId string, ) *InvoiceAttachmentCreateRequest`

NewInvoiceAttachmentCreateRequest instantiates a new InvoiceAttachmentCreateRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewInvoiceAttachmentCreateRequestWithDefaults

`func NewInvoiceAttachmentCreateRequestWithDefaults() *InvoiceAttachmentCreateRequest`

NewInvoiceAttachmentCreateRequestWithDefaults instantiates a new InvoiceAttachmentCreateRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetFileId

`func (o *InvoiceAttachmentCreateRequest) GetFileId() string`

GetFileId returns the FileId field if non-nil, zero value otherwise.

### GetFileIdOk

`func (o *InvoiceAttachmentCreateRequest) GetFileIdOk() (*string, bool)`

GetFileIdOk returns a tuple with the FileId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileId

`func (o *InvoiceAttachmentCreateRequest) SetFileId(v string)`

SetFileId sets FileId field to given value.


### GetLabel

`func (o *InvoiceAttachmentCreateRequest) GetLabel() string`

GetLabel returns the Label field if non-nil, zero value otherwise.

### GetLabelOk

`func (o *InvoiceAttachmentCreateRequest) GetLabelOk() (*string, bool)`

GetLabelOk returns a tuple with the Label field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabel

`func (o *InvoiceAttachmentCreateRequest) SetLabel(v string)`

SetLabel sets Label field to given value.

### HasLabel

`func (o *InvoiceAttachmentCreateRequest) HasLabel() bool`

HasLabel returns a boolean if a field has been set.

### SetLabelNil

`func (o *InvoiceAttachmentCreateRequest) SetLabelNil(b bool)`

 SetLabelNil sets the value for Label to be an explicit nil

### UnsetLabel
`func (o *InvoiceAttachmentCreateRequest) UnsetLabel()`

UnsetLabel ensures that no value is present for Label, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


