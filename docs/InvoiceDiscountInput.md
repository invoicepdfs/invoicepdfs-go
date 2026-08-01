# InvoiceDiscountInput

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | Pointer to **string** |  | [optional] [default to "percentage"]
**Value** | **string** |  | 
**Reason** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewInvoiceDiscountInput

`func NewInvoiceDiscountInput(value string, ) *InvoiceDiscountInput`

NewInvoiceDiscountInput instantiates a new InvoiceDiscountInput object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewInvoiceDiscountInputWithDefaults

`func NewInvoiceDiscountInputWithDefaults() *InvoiceDiscountInput`

NewInvoiceDiscountInputWithDefaults instantiates a new InvoiceDiscountInput object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *InvoiceDiscountInput) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *InvoiceDiscountInput) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *InvoiceDiscountInput) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *InvoiceDiscountInput) HasType() bool`

HasType returns a boolean if a field has been set.

### GetValue

`func (o *InvoiceDiscountInput) GetValue() string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *InvoiceDiscountInput) GetValueOk() (*string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *InvoiceDiscountInput) SetValue(v string)`

SetValue sets Value field to given value.


### GetReason

`func (o *InvoiceDiscountInput) GetReason() string`

GetReason returns the Reason field if non-nil, zero value otherwise.

### GetReasonOk

`func (o *InvoiceDiscountInput) GetReasonOk() (*string, bool)`

GetReasonOk returns a tuple with the Reason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReason

`func (o *InvoiceDiscountInput) SetReason(v string)`

SetReason sets Reason field to given value.

### HasReason

`func (o *InvoiceDiscountInput) HasReason() bool`

HasReason returns a boolean if a field has been set.

### SetReasonNil

`func (o *InvoiceDiscountInput) SetReasonNil(b bool)`

 SetReasonNil sets the value for Reason to be an explicit nil

### UnsetReason
`func (o *InvoiceDiscountInput) UnsetReason()`

UnsetReason ensures that no value is present for Reason, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


