# InvoiceShippingInput

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Description** | Pointer to **string** |  | [optional] [default to "Shipping"]
**Amount** | **string** |  | 

## Methods

### NewInvoiceShippingInput

`func NewInvoiceShippingInput(amount string, ) *InvoiceShippingInput`

NewInvoiceShippingInput instantiates a new InvoiceShippingInput object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewInvoiceShippingInputWithDefaults

`func NewInvoiceShippingInputWithDefaults() *InvoiceShippingInput`

NewInvoiceShippingInputWithDefaults instantiates a new InvoiceShippingInput object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDescription

`func (o *InvoiceShippingInput) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *InvoiceShippingInput) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *InvoiceShippingInput) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *InvoiceShippingInput) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetAmount

`func (o *InvoiceShippingInput) GetAmount() string`

GetAmount returns the Amount field if non-nil, zero value otherwise.

### GetAmountOk

`func (o *InvoiceShippingInput) GetAmountOk() (*string, bool)`

GetAmountOk returns a tuple with the Amount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAmount

`func (o *InvoiceShippingInput) SetAmount(v string)`

SetAmount sets Amount field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


