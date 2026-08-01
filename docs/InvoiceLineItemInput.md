# InvoiceLineItemInput

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** |  | 
**Description** | Pointer to **NullableString** |  | [optional] 
**Quantity** | **string** | Decimal string | 
**UnitPrice** | **string** | Decimal string in major units | 
**Unit** | Pointer to **NullableString** |  | [optional] 
**Sku** | Pointer to **NullableString** |  | [optional] 
**Discount** | Pointer to [**NullableInvoiceDiscountInput**](InvoiceDiscountInput.md) |  | [optional] 
**Taxes** | Pointer to [**[]InvoiceLineItemTaxInput**](InvoiceLineItemTaxInput.md) |  | [optional] 

## Methods

### NewInvoiceLineItemInput

`func NewInvoiceLineItemInput(name string, quantity string, unitPrice string, ) *InvoiceLineItemInput`

NewInvoiceLineItemInput instantiates a new InvoiceLineItemInput object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewInvoiceLineItemInputWithDefaults

`func NewInvoiceLineItemInputWithDefaults() *InvoiceLineItemInput`

NewInvoiceLineItemInputWithDefaults instantiates a new InvoiceLineItemInput object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *InvoiceLineItemInput) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *InvoiceLineItemInput) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *InvoiceLineItemInput) SetName(v string)`

SetName sets Name field to given value.


### GetDescription

`func (o *InvoiceLineItemInput) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *InvoiceLineItemInput) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *InvoiceLineItemInput) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *InvoiceLineItemInput) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *InvoiceLineItemInput) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *InvoiceLineItemInput) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetQuantity

`func (o *InvoiceLineItemInput) GetQuantity() string`

GetQuantity returns the Quantity field if non-nil, zero value otherwise.

### GetQuantityOk

`func (o *InvoiceLineItemInput) GetQuantityOk() (*string, bool)`

GetQuantityOk returns a tuple with the Quantity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuantity

`func (o *InvoiceLineItemInput) SetQuantity(v string)`

SetQuantity sets Quantity field to given value.


### GetUnitPrice

`func (o *InvoiceLineItemInput) GetUnitPrice() string`

GetUnitPrice returns the UnitPrice field if non-nil, zero value otherwise.

### GetUnitPriceOk

`func (o *InvoiceLineItemInput) GetUnitPriceOk() (*string, bool)`

GetUnitPriceOk returns a tuple with the UnitPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUnitPrice

`func (o *InvoiceLineItemInput) SetUnitPrice(v string)`

SetUnitPrice sets UnitPrice field to given value.


### GetUnit

`func (o *InvoiceLineItemInput) GetUnit() string`

GetUnit returns the Unit field if non-nil, zero value otherwise.

### GetUnitOk

`func (o *InvoiceLineItemInput) GetUnitOk() (*string, bool)`

GetUnitOk returns a tuple with the Unit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUnit

`func (o *InvoiceLineItemInput) SetUnit(v string)`

SetUnit sets Unit field to given value.

### HasUnit

`func (o *InvoiceLineItemInput) HasUnit() bool`

HasUnit returns a boolean if a field has been set.

### SetUnitNil

`func (o *InvoiceLineItemInput) SetUnitNil(b bool)`

 SetUnitNil sets the value for Unit to be an explicit nil

### UnsetUnit
`func (o *InvoiceLineItemInput) UnsetUnit()`

UnsetUnit ensures that no value is present for Unit, not even an explicit nil
### GetSku

`func (o *InvoiceLineItemInput) GetSku() string`

GetSku returns the Sku field if non-nil, zero value otherwise.

### GetSkuOk

`func (o *InvoiceLineItemInput) GetSkuOk() (*string, bool)`

GetSkuOk returns a tuple with the Sku field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSku

`func (o *InvoiceLineItemInput) SetSku(v string)`

SetSku sets Sku field to given value.

### HasSku

`func (o *InvoiceLineItemInput) HasSku() bool`

HasSku returns a boolean if a field has been set.

### SetSkuNil

`func (o *InvoiceLineItemInput) SetSkuNil(b bool)`

 SetSkuNil sets the value for Sku to be an explicit nil

### UnsetSku
`func (o *InvoiceLineItemInput) UnsetSku()`

UnsetSku ensures that no value is present for Sku, not even an explicit nil
### GetDiscount

`func (o *InvoiceLineItemInput) GetDiscount() InvoiceDiscountInput`

GetDiscount returns the Discount field if non-nil, zero value otherwise.

### GetDiscountOk

`func (o *InvoiceLineItemInput) GetDiscountOk() (*InvoiceDiscountInput, bool)`

GetDiscountOk returns a tuple with the Discount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDiscount

`func (o *InvoiceLineItemInput) SetDiscount(v InvoiceDiscountInput)`

SetDiscount sets Discount field to given value.

### HasDiscount

`func (o *InvoiceLineItemInput) HasDiscount() bool`

HasDiscount returns a boolean if a field has been set.

### SetDiscountNil

`func (o *InvoiceLineItemInput) SetDiscountNil(b bool)`

 SetDiscountNil sets the value for Discount to be an explicit nil

### UnsetDiscount
`func (o *InvoiceLineItemInput) UnsetDiscount()`

UnsetDiscount ensures that no value is present for Discount, not even an explicit nil
### GetTaxes

`func (o *InvoiceLineItemInput) GetTaxes() []InvoiceLineItemTaxInput`

GetTaxes returns the Taxes field if non-nil, zero value otherwise.

### GetTaxesOk

`func (o *InvoiceLineItemInput) GetTaxesOk() (*[]InvoiceLineItemTaxInput, bool)`

GetTaxesOk returns a tuple with the Taxes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTaxes

`func (o *InvoiceLineItemInput) SetTaxes(v []InvoiceLineItemTaxInput)`

SetTaxes sets Taxes field to given value.

### HasTaxes

`func (o *InvoiceLineItemInput) HasTaxes() bool`

HasTaxes returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


