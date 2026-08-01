# PaymentOut

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**InvoiceId** | **string** |  | 
**Amount** | [**MoneyOut**](MoneyOut.md) |  | 
**PaidAt** | **string** |  | 
**Method** | Pointer to **NullableString** |  | [optional] 
**Reference** | Pointer to **NullableString** |  | [optional] 
**Notes** | Pointer to **NullableString** |  | [optional] 
**CreatedAt** | **string** |  | 
**UpdatedAt** | **string** |  | 

## Methods

### NewPaymentOut

`func NewPaymentOut(id string, invoiceId string, amount MoneyOut, paidAt string, createdAt string, updatedAt string, ) *PaymentOut`

NewPaymentOut instantiates a new PaymentOut object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPaymentOutWithDefaults

`func NewPaymentOutWithDefaults() *PaymentOut`

NewPaymentOutWithDefaults instantiates a new PaymentOut object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *PaymentOut) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *PaymentOut) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *PaymentOut) SetId(v string)`

SetId sets Id field to given value.


### GetInvoiceId

`func (o *PaymentOut) GetInvoiceId() string`

GetInvoiceId returns the InvoiceId field if non-nil, zero value otherwise.

### GetInvoiceIdOk

`func (o *PaymentOut) GetInvoiceIdOk() (*string, bool)`

GetInvoiceIdOk returns a tuple with the InvoiceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInvoiceId

`func (o *PaymentOut) SetInvoiceId(v string)`

SetInvoiceId sets InvoiceId field to given value.


### GetAmount

`func (o *PaymentOut) GetAmount() MoneyOut`

GetAmount returns the Amount field if non-nil, zero value otherwise.

### GetAmountOk

`func (o *PaymentOut) GetAmountOk() (*MoneyOut, bool)`

GetAmountOk returns a tuple with the Amount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAmount

`func (o *PaymentOut) SetAmount(v MoneyOut)`

SetAmount sets Amount field to given value.


### GetPaidAt

`func (o *PaymentOut) GetPaidAt() string`

GetPaidAt returns the PaidAt field if non-nil, zero value otherwise.

### GetPaidAtOk

`func (o *PaymentOut) GetPaidAtOk() (*string, bool)`

GetPaidAtOk returns a tuple with the PaidAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaidAt

`func (o *PaymentOut) SetPaidAt(v string)`

SetPaidAt sets PaidAt field to given value.


### GetMethod

`func (o *PaymentOut) GetMethod() string`

GetMethod returns the Method field if non-nil, zero value otherwise.

### GetMethodOk

`func (o *PaymentOut) GetMethodOk() (*string, bool)`

GetMethodOk returns a tuple with the Method field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMethod

`func (o *PaymentOut) SetMethod(v string)`

SetMethod sets Method field to given value.

### HasMethod

`func (o *PaymentOut) HasMethod() bool`

HasMethod returns a boolean if a field has been set.

### SetMethodNil

`func (o *PaymentOut) SetMethodNil(b bool)`

 SetMethodNil sets the value for Method to be an explicit nil

### UnsetMethod
`func (o *PaymentOut) UnsetMethod()`

UnsetMethod ensures that no value is present for Method, not even an explicit nil
### GetReference

`func (o *PaymentOut) GetReference() string`

GetReference returns the Reference field if non-nil, zero value otherwise.

### GetReferenceOk

`func (o *PaymentOut) GetReferenceOk() (*string, bool)`

GetReferenceOk returns a tuple with the Reference field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReference

`func (o *PaymentOut) SetReference(v string)`

SetReference sets Reference field to given value.

### HasReference

`func (o *PaymentOut) HasReference() bool`

HasReference returns a boolean if a field has been set.

### SetReferenceNil

`func (o *PaymentOut) SetReferenceNil(b bool)`

 SetReferenceNil sets the value for Reference to be an explicit nil

### UnsetReference
`func (o *PaymentOut) UnsetReference()`

UnsetReference ensures that no value is present for Reference, not even an explicit nil
### GetNotes

`func (o *PaymentOut) GetNotes() string`

GetNotes returns the Notes field if non-nil, zero value otherwise.

### GetNotesOk

`func (o *PaymentOut) GetNotesOk() (*string, bool)`

GetNotesOk returns a tuple with the Notes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNotes

`func (o *PaymentOut) SetNotes(v string)`

SetNotes sets Notes field to given value.

### HasNotes

`func (o *PaymentOut) HasNotes() bool`

HasNotes returns a boolean if a field has been set.

### SetNotesNil

`func (o *PaymentOut) SetNotesNil(b bool)`

 SetNotesNil sets the value for Notes to be an explicit nil

### UnsetNotes
`func (o *PaymentOut) UnsetNotes()`

UnsetNotes ensures that no value is present for Notes, not even an explicit nil
### GetCreatedAt

`func (o *PaymentOut) GetCreatedAt() string`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *PaymentOut) GetCreatedAtOk() (*string, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *PaymentOut) SetCreatedAt(v string)`

SetCreatedAt sets CreatedAt field to given value.


### GetUpdatedAt

`func (o *PaymentOut) GetUpdatedAt() string`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *PaymentOut) GetUpdatedAtOk() (*string, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *PaymentOut) SetUpdatedAt(v string)`

SetUpdatedAt sets UpdatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


