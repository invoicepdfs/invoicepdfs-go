# CreditNoteLineItemInput

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** |  | 
**Description** | Pointer to **NullableString** |  | [optional] 
**Quantity** | **string** |  | 
**UnitPrice** | **string** |  | 
**Taxes** | Pointer to [**[]InvoiceLineItemTaxInput**](InvoiceLineItemTaxInput.md) |  | [optional] 

## Methods

### NewCreditNoteLineItemInput

`func NewCreditNoteLineItemInput(name string, quantity string, unitPrice string, ) *CreditNoteLineItemInput`

NewCreditNoteLineItemInput instantiates a new CreditNoteLineItemInput object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreditNoteLineItemInputWithDefaults

`func NewCreditNoteLineItemInputWithDefaults() *CreditNoteLineItemInput`

NewCreditNoteLineItemInputWithDefaults instantiates a new CreditNoteLineItemInput object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *CreditNoteLineItemInput) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CreditNoteLineItemInput) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CreditNoteLineItemInput) SetName(v string)`

SetName sets Name field to given value.


### GetDescription

`func (o *CreditNoteLineItemInput) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *CreditNoteLineItemInput) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *CreditNoteLineItemInput) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *CreditNoteLineItemInput) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *CreditNoteLineItemInput) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *CreditNoteLineItemInput) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetQuantity

`func (o *CreditNoteLineItemInput) GetQuantity() string`

GetQuantity returns the Quantity field if non-nil, zero value otherwise.

### GetQuantityOk

`func (o *CreditNoteLineItemInput) GetQuantityOk() (*string, bool)`

GetQuantityOk returns a tuple with the Quantity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuantity

`func (o *CreditNoteLineItemInput) SetQuantity(v string)`

SetQuantity sets Quantity field to given value.


### GetUnitPrice

`func (o *CreditNoteLineItemInput) GetUnitPrice() string`

GetUnitPrice returns the UnitPrice field if non-nil, zero value otherwise.

### GetUnitPriceOk

`func (o *CreditNoteLineItemInput) GetUnitPriceOk() (*string, bool)`

GetUnitPriceOk returns a tuple with the UnitPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUnitPrice

`func (o *CreditNoteLineItemInput) SetUnitPrice(v string)`

SetUnitPrice sets UnitPrice field to given value.


### GetTaxes

`func (o *CreditNoteLineItemInput) GetTaxes() []InvoiceLineItemTaxInput`

GetTaxes returns the Taxes field if non-nil, zero value otherwise.

### GetTaxesOk

`func (o *CreditNoteLineItemInput) GetTaxesOk() (*[]InvoiceLineItemTaxInput, bool)`

GetTaxesOk returns a tuple with the Taxes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTaxes

`func (o *CreditNoteLineItemInput) SetTaxes(v []InvoiceLineItemTaxInput)`

SetTaxes sets Taxes field to given value.

### HasTaxes

`func (o *CreditNoteLineItemInput) HasTaxes() bool`

HasTaxes returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


