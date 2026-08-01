# DeliverySendRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**To** | **[]string** |  | 
**Cc** | Pointer to **[]string** |  | [optional] 
**Bcc** | Pointer to **[]string** |  | [optional] 
**Subject** | Pointer to **NullableString** |  | [optional] 
**Message** | Pointer to **NullableString** |  | [optional] 
**AttachPdf** | Pointer to **bool** |  | [optional] [default to true]

## Methods

### NewDeliverySendRequest

`func NewDeliverySendRequest(to []string, ) *DeliverySendRequest`

NewDeliverySendRequest instantiates a new DeliverySendRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDeliverySendRequestWithDefaults

`func NewDeliverySendRequestWithDefaults() *DeliverySendRequest`

NewDeliverySendRequestWithDefaults instantiates a new DeliverySendRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTo

`func (o *DeliverySendRequest) GetTo() []string`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *DeliverySendRequest) GetToOk() (*[]string, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *DeliverySendRequest) SetTo(v []string)`

SetTo sets To field to given value.


### GetCc

`func (o *DeliverySendRequest) GetCc() []string`

GetCc returns the Cc field if non-nil, zero value otherwise.

### GetCcOk

`func (o *DeliverySendRequest) GetCcOk() (*[]string, bool)`

GetCcOk returns a tuple with the Cc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCc

`func (o *DeliverySendRequest) SetCc(v []string)`

SetCc sets Cc field to given value.

### HasCc

`func (o *DeliverySendRequest) HasCc() bool`

HasCc returns a boolean if a field has been set.

### GetBcc

`func (o *DeliverySendRequest) GetBcc() []string`

GetBcc returns the Bcc field if non-nil, zero value otherwise.

### GetBccOk

`func (o *DeliverySendRequest) GetBccOk() (*[]string, bool)`

GetBccOk returns a tuple with the Bcc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBcc

`func (o *DeliverySendRequest) SetBcc(v []string)`

SetBcc sets Bcc field to given value.

### HasBcc

`func (o *DeliverySendRequest) HasBcc() bool`

HasBcc returns a boolean if a field has been set.

### GetSubject

`func (o *DeliverySendRequest) GetSubject() string`

GetSubject returns the Subject field if non-nil, zero value otherwise.

### GetSubjectOk

`func (o *DeliverySendRequest) GetSubjectOk() (*string, bool)`

GetSubjectOk returns a tuple with the Subject field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubject

`func (o *DeliverySendRequest) SetSubject(v string)`

SetSubject sets Subject field to given value.

### HasSubject

`func (o *DeliverySendRequest) HasSubject() bool`

HasSubject returns a boolean if a field has been set.

### SetSubjectNil

`func (o *DeliverySendRequest) SetSubjectNil(b bool)`

 SetSubjectNil sets the value for Subject to be an explicit nil

### UnsetSubject
`func (o *DeliverySendRequest) UnsetSubject()`

UnsetSubject ensures that no value is present for Subject, not even an explicit nil
### GetMessage

`func (o *DeliverySendRequest) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *DeliverySendRequest) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *DeliverySendRequest) SetMessage(v string)`

SetMessage sets Message field to given value.

### HasMessage

`func (o *DeliverySendRequest) HasMessage() bool`

HasMessage returns a boolean if a field has been set.

### SetMessageNil

`func (o *DeliverySendRequest) SetMessageNil(b bool)`

 SetMessageNil sets the value for Message to be an explicit nil

### UnsetMessage
`func (o *DeliverySendRequest) UnsetMessage()`

UnsetMessage ensures that no value is present for Message, not even an explicit nil
### GetAttachPdf

`func (o *DeliverySendRequest) GetAttachPdf() bool`

GetAttachPdf returns the AttachPdf field if non-nil, zero value otherwise.

### GetAttachPdfOk

`func (o *DeliverySendRequest) GetAttachPdfOk() (*bool, bool)`

GetAttachPdfOk returns a tuple with the AttachPdf field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttachPdf

`func (o *DeliverySendRequest) SetAttachPdf(v bool)`

SetAttachPdf sets AttachPdf field to given value.

### HasAttachPdf

`func (o *DeliverySendRequest) HasAttachPdf() bool`

HasAttachPdf returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


