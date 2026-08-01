# InvoiceAttachmentOut

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**InvoiceId** | **string** |  | 
**FileId** | **string** |  | 
**Label** | Pointer to **NullableString** |  | [optional] 
**CreatedAt** | **string** |  | 

## Methods

### NewInvoiceAttachmentOut

`func NewInvoiceAttachmentOut(id string, invoiceId string, fileId string, createdAt string, ) *InvoiceAttachmentOut`

NewInvoiceAttachmentOut instantiates a new InvoiceAttachmentOut object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewInvoiceAttachmentOutWithDefaults

`func NewInvoiceAttachmentOutWithDefaults() *InvoiceAttachmentOut`

NewInvoiceAttachmentOutWithDefaults instantiates a new InvoiceAttachmentOut object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *InvoiceAttachmentOut) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *InvoiceAttachmentOut) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *InvoiceAttachmentOut) SetId(v string)`

SetId sets Id field to given value.


### GetInvoiceId

`func (o *InvoiceAttachmentOut) GetInvoiceId() string`

GetInvoiceId returns the InvoiceId field if non-nil, zero value otherwise.

### GetInvoiceIdOk

`func (o *InvoiceAttachmentOut) GetInvoiceIdOk() (*string, bool)`

GetInvoiceIdOk returns a tuple with the InvoiceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInvoiceId

`func (o *InvoiceAttachmentOut) SetInvoiceId(v string)`

SetInvoiceId sets InvoiceId field to given value.


### GetFileId

`func (o *InvoiceAttachmentOut) GetFileId() string`

GetFileId returns the FileId field if non-nil, zero value otherwise.

### GetFileIdOk

`func (o *InvoiceAttachmentOut) GetFileIdOk() (*string, bool)`

GetFileIdOk returns a tuple with the FileId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileId

`func (o *InvoiceAttachmentOut) SetFileId(v string)`

SetFileId sets FileId field to given value.


### GetLabel

`func (o *InvoiceAttachmentOut) GetLabel() string`

GetLabel returns the Label field if non-nil, zero value otherwise.

### GetLabelOk

`func (o *InvoiceAttachmentOut) GetLabelOk() (*string, bool)`

GetLabelOk returns a tuple with the Label field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabel

`func (o *InvoiceAttachmentOut) SetLabel(v string)`

SetLabel sets Label field to given value.

### HasLabel

`func (o *InvoiceAttachmentOut) HasLabel() bool`

HasLabel returns a boolean if a field has been set.

### SetLabelNil

`func (o *InvoiceAttachmentOut) SetLabelNil(b bool)`

 SetLabelNil sets the value for Label to be an explicit nil

### UnsetLabel
`func (o *InvoiceAttachmentOut) UnsetLabel()`

UnsetLabel ensures that no value is present for Label, not even an explicit nil
### GetCreatedAt

`func (o *InvoiceAttachmentOut) GetCreatedAt() string`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *InvoiceAttachmentOut) GetCreatedAtOk() (*string, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *InvoiceAttachmentOut) SetCreatedAt(v string)`

SetCreatedAt sets CreatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


