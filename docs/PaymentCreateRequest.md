# PaymentCreateRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Amount** | **string** |  | 
**PaidAt** | **time.Time** |  | 
**Method** | Pointer to **NullableString** |  | [optional] 
**Reference** | Pointer to **NullableString** |  | [optional] 
**Notes** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewPaymentCreateRequest

`func NewPaymentCreateRequest(amount string, paidAt time.Time, ) *PaymentCreateRequest`

NewPaymentCreateRequest instantiates a new PaymentCreateRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPaymentCreateRequestWithDefaults

`func NewPaymentCreateRequestWithDefaults() *PaymentCreateRequest`

NewPaymentCreateRequestWithDefaults instantiates a new PaymentCreateRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAmount

`func (o *PaymentCreateRequest) GetAmount() string`

GetAmount returns the Amount field if non-nil, zero value otherwise.

### GetAmountOk

`func (o *PaymentCreateRequest) GetAmountOk() (*string, bool)`

GetAmountOk returns a tuple with the Amount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAmount

`func (o *PaymentCreateRequest) SetAmount(v string)`

SetAmount sets Amount field to given value.


### GetPaidAt

`func (o *PaymentCreateRequest) GetPaidAt() time.Time`

GetPaidAt returns the PaidAt field if non-nil, zero value otherwise.

### GetPaidAtOk

`func (o *PaymentCreateRequest) GetPaidAtOk() (*time.Time, bool)`

GetPaidAtOk returns a tuple with the PaidAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaidAt

`func (o *PaymentCreateRequest) SetPaidAt(v time.Time)`

SetPaidAt sets PaidAt field to given value.


### GetMethod

`func (o *PaymentCreateRequest) GetMethod() string`

GetMethod returns the Method field if non-nil, zero value otherwise.

### GetMethodOk

`func (o *PaymentCreateRequest) GetMethodOk() (*string, bool)`

GetMethodOk returns a tuple with the Method field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMethod

`func (o *PaymentCreateRequest) SetMethod(v string)`

SetMethod sets Method field to given value.

### HasMethod

`func (o *PaymentCreateRequest) HasMethod() bool`

HasMethod returns a boolean if a field has been set.

### SetMethodNil

`func (o *PaymentCreateRequest) SetMethodNil(b bool)`

 SetMethodNil sets the value for Method to be an explicit nil

### UnsetMethod
`func (o *PaymentCreateRequest) UnsetMethod()`

UnsetMethod ensures that no value is present for Method, not even an explicit nil
### GetReference

`func (o *PaymentCreateRequest) GetReference() string`

GetReference returns the Reference field if non-nil, zero value otherwise.

### GetReferenceOk

`func (o *PaymentCreateRequest) GetReferenceOk() (*string, bool)`

GetReferenceOk returns a tuple with the Reference field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReference

`func (o *PaymentCreateRequest) SetReference(v string)`

SetReference sets Reference field to given value.

### HasReference

`func (o *PaymentCreateRequest) HasReference() bool`

HasReference returns a boolean if a field has been set.

### SetReferenceNil

`func (o *PaymentCreateRequest) SetReferenceNil(b bool)`

 SetReferenceNil sets the value for Reference to be an explicit nil

### UnsetReference
`func (o *PaymentCreateRequest) UnsetReference()`

UnsetReference ensures that no value is present for Reference, not even an explicit nil
### GetNotes

`func (o *PaymentCreateRequest) GetNotes() string`

GetNotes returns the Notes field if non-nil, zero value otherwise.

### GetNotesOk

`func (o *PaymentCreateRequest) GetNotesOk() (*string, bool)`

GetNotesOk returns a tuple with the Notes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNotes

`func (o *PaymentCreateRequest) SetNotes(v string)`

SetNotes sets Notes field to given value.

### HasNotes

`func (o *PaymentCreateRequest) HasNotes() bool`

HasNotes returns a boolean if a field has been set.

### SetNotesNil

`func (o *PaymentCreateRequest) SetNotesNil(b bool)`

 SetNotesNil sets the value for Notes to be an explicit nil

### UnsetNotes
`func (o *PaymentCreateRequest) UnsetNotes()`

UnsetNotes ensures that no value is present for Notes, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


