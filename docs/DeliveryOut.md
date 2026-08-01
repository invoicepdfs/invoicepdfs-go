# DeliveryOut

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**InvoiceId** | **string** |  | 
**To** | **[]string** |  | 
**Cc** | **[]string** |  | 
**Bcc** | **[]string** |  | 
**Subject** | **string** |  | 
**Message** | Pointer to **NullableString** |  | [optional] 
**AttachPdf** | **bool** |  | 
**Status** | **string** |  | 
**CreatedAt** | **string** |  | 
**SentAt** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewDeliveryOut

`func NewDeliveryOut(id string, invoiceId string, to []string, cc []string, bcc []string, subject string, attachPdf bool, status string, createdAt string, ) *DeliveryOut`

NewDeliveryOut instantiates a new DeliveryOut object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDeliveryOutWithDefaults

`func NewDeliveryOutWithDefaults() *DeliveryOut`

NewDeliveryOutWithDefaults instantiates a new DeliveryOut object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *DeliveryOut) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *DeliveryOut) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *DeliveryOut) SetId(v string)`

SetId sets Id field to given value.


### GetInvoiceId

`func (o *DeliveryOut) GetInvoiceId() string`

GetInvoiceId returns the InvoiceId field if non-nil, zero value otherwise.

### GetInvoiceIdOk

`func (o *DeliveryOut) GetInvoiceIdOk() (*string, bool)`

GetInvoiceIdOk returns a tuple with the InvoiceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInvoiceId

`func (o *DeliveryOut) SetInvoiceId(v string)`

SetInvoiceId sets InvoiceId field to given value.


### GetTo

`func (o *DeliveryOut) GetTo() []string`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *DeliveryOut) GetToOk() (*[]string, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *DeliveryOut) SetTo(v []string)`

SetTo sets To field to given value.


### GetCc

`func (o *DeliveryOut) GetCc() []string`

GetCc returns the Cc field if non-nil, zero value otherwise.

### GetCcOk

`func (o *DeliveryOut) GetCcOk() (*[]string, bool)`

GetCcOk returns a tuple with the Cc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCc

`func (o *DeliveryOut) SetCc(v []string)`

SetCc sets Cc field to given value.


### GetBcc

`func (o *DeliveryOut) GetBcc() []string`

GetBcc returns the Bcc field if non-nil, zero value otherwise.

### GetBccOk

`func (o *DeliveryOut) GetBccOk() (*[]string, bool)`

GetBccOk returns a tuple with the Bcc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBcc

`func (o *DeliveryOut) SetBcc(v []string)`

SetBcc sets Bcc field to given value.


### GetSubject

`func (o *DeliveryOut) GetSubject() string`

GetSubject returns the Subject field if non-nil, zero value otherwise.

### GetSubjectOk

`func (o *DeliveryOut) GetSubjectOk() (*string, bool)`

GetSubjectOk returns a tuple with the Subject field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubject

`func (o *DeliveryOut) SetSubject(v string)`

SetSubject sets Subject field to given value.


### GetMessage

`func (o *DeliveryOut) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *DeliveryOut) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *DeliveryOut) SetMessage(v string)`

SetMessage sets Message field to given value.

### HasMessage

`func (o *DeliveryOut) HasMessage() bool`

HasMessage returns a boolean if a field has been set.

### SetMessageNil

`func (o *DeliveryOut) SetMessageNil(b bool)`

 SetMessageNil sets the value for Message to be an explicit nil

### UnsetMessage
`func (o *DeliveryOut) UnsetMessage()`

UnsetMessage ensures that no value is present for Message, not even an explicit nil
### GetAttachPdf

`func (o *DeliveryOut) GetAttachPdf() bool`

GetAttachPdf returns the AttachPdf field if non-nil, zero value otherwise.

### GetAttachPdfOk

`func (o *DeliveryOut) GetAttachPdfOk() (*bool, bool)`

GetAttachPdfOk returns a tuple with the AttachPdf field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttachPdf

`func (o *DeliveryOut) SetAttachPdf(v bool)`

SetAttachPdf sets AttachPdf field to given value.


### GetStatus

`func (o *DeliveryOut) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *DeliveryOut) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *DeliveryOut) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetCreatedAt

`func (o *DeliveryOut) GetCreatedAt() string`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *DeliveryOut) GetCreatedAtOk() (*string, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *DeliveryOut) SetCreatedAt(v string)`

SetCreatedAt sets CreatedAt field to given value.


### GetSentAt

`func (o *DeliveryOut) GetSentAt() string`

GetSentAt returns the SentAt field if non-nil, zero value otherwise.

### GetSentAtOk

`func (o *DeliveryOut) GetSentAtOk() (*string, bool)`

GetSentAtOk returns a tuple with the SentAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSentAt

`func (o *DeliveryOut) SetSentAt(v string)`

SetSentAt sets SentAt field to given value.

### HasSentAt

`func (o *DeliveryOut) HasSentAt() bool`

HasSentAt returns a boolean if a field has been set.

### SetSentAtNil

`func (o *DeliveryOut) SetSentAtNil(b bool)`

 SetSentAtNil sets the value for SentAt to be an explicit nil

### UnsetSentAt
`func (o *DeliveryOut) UnsetSentAt()`

UnsetSentAt ensures that no value is present for SentAt, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


