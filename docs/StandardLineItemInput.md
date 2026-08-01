# StandardLineItemInput

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** |  | 
**Description** | Pointer to **NullableString** |  | [optional] 
**Quantity** | **string** | Decimal string | 
**UnitPrice** | Pointer to **string** | Decimal string, major units | [optional] [default to "0.00"]
**Unit** | Pointer to **NullableString** |  | [optional] 
**Sku** | Pointer to **NullableString** |  | [optional] 
**Discount** | Pointer to [**NullableLineItemDiscountInput**](LineItemDiscountInput.md) |  | [optional] 
**Taxes** | Pointer to [**[]LineItemTaxInput**](LineItemTaxInput.md) |  | [optional] 

## Methods

### NewStandardLineItemInput

`func NewStandardLineItemInput(name string, quantity string, ) *StandardLineItemInput`

NewStandardLineItemInput instantiates a new StandardLineItemInput object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewStandardLineItemInputWithDefaults

`func NewStandardLineItemInputWithDefaults() *StandardLineItemInput`

NewStandardLineItemInputWithDefaults instantiates a new StandardLineItemInput object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *StandardLineItemInput) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *StandardLineItemInput) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *StandardLineItemInput) SetName(v string)`

SetName sets Name field to given value.


### GetDescription

`func (o *StandardLineItemInput) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *StandardLineItemInput) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *StandardLineItemInput) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *StandardLineItemInput) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *StandardLineItemInput) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *StandardLineItemInput) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetQuantity

`func (o *StandardLineItemInput) GetQuantity() string`

GetQuantity returns the Quantity field if non-nil, zero value otherwise.

### GetQuantityOk

`func (o *StandardLineItemInput) GetQuantityOk() (*string, bool)`

GetQuantityOk returns a tuple with the Quantity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuantity

`func (o *StandardLineItemInput) SetQuantity(v string)`

SetQuantity sets Quantity field to given value.


### GetUnitPrice

`func (o *StandardLineItemInput) GetUnitPrice() string`

GetUnitPrice returns the UnitPrice field if non-nil, zero value otherwise.

### GetUnitPriceOk

`func (o *StandardLineItemInput) GetUnitPriceOk() (*string, bool)`

GetUnitPriceOk returns a tuple with the UnitPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUnitPrice

`func (o *StandardLineItemInput) SetUnitPrice(v string)`

SetUnitPrice sets UnitPrice field to given value.

### HasUnitPrice

`func (o *StandardLineItemInput) HasUnitPrice() bool`

HasUnitPrice returns a boolean if a field has been set.

### GetUnit

`func (o *StandardLineItemInput) GetUnit() string`

GetUnit returns the Unit field if non-nil, zero value otherwise.

### GetUnitOk

`func (o *StandardLineItemInput) GetUnitOk() (*string, bool)`

GetUnitOk returns a tuple with the Unit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUnit

`func (o *StandardLineItemInput) SetUnit(v string)`

SetUnit sets Unit field to given value.

### HasUnit

`func (o *StandardLineItemInput) HasUnit() bool`

HasUnit returns a boolean if a field has been set.

### SetUnitNil

`func (o *StandardLineItemInput) SetUnitNil(b bool)`

 SetUnitNil sets the value for Unit to be an explicit nil

### UnsetUnit
`func (o *StandardLineItemInput) UnsetUnit()`

UnsetUnit ensures that no value is present for Unit, not even an explicit nil
### GetSku

`func (o *StandardLineItemInput) GetSku() string`

GetSku returns the Sku field if non-nil, zero value otherwise.

### GetSkuOk

`func (o *StandardLineItemInput) GetSkuOk() (*string, bool)`

GetSkuOk returns a tuple with the Sku field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSku

`func (o *StandardLineItemInput) SetSku(v string)`

SetSku sets Sku field to given value.

### HasSku

`func (o *StandardLineItemInput) HasSku() bool`

HasSku returns a boolean if a field has been set.

### SetSkuNil

`func (o *StandardLineItemInput) SetSkuNil(b bool)`

 SetSkuNil sets the value for Sku to be an explicit nil

### UnsetSku
`func (o *StandardLineItemInput) UnsetSku()`

UnsetSku ensures that no value is present for Sku, not even an explicit nil
### GetDiscount

`func (o *StandardLineItemInput) GetDiscount() LineItemDiscountInput`

GetDiscount returns the Discount field if non-nil, zero value otherwise.

### GetDiscountOk

`func (o *StandardLineItemInput) GetDiscountOk() (*LineItemDiscountInput, bool)`

GetDiscountOk returns a tuple with the Discount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDiscount

`func (o *StandardLineItemInput) SetDiscount(v LineItemDiscountInput)`

SetDiscount sets Discount field to given value.

### HasDiscount

`func (o *StandardLineItemInput) HasDiscount() bool`

HasDiscount returns a boolean if a field has been set.

### SetDiscountNil

`func (o *StandardLineItemInput) SetDiscountNil(b bool)`

 SetDiscountNil sets the value for Discount to be an explicit nil

### UnsetDiscount
`func (o *StandardLineItemInput) UnsetDiscount()`

UnsetDiscount ensures that no value is present for Discount, not even an explicit nil
### GetTaxes

`func (o *StandardLineItemInput) GetTaxes() []LineItemTaxInput`

GetTaxes returns the Taxes field if non-nil, zero value otherwise.

### GetTaxesOk

`func (o *StandardLineItemInput) GetTaxesOk() (*[]LineItemTaxInput, bool)`

GetTaxesOk returns a tuple with the Taxes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTaxes

`func (o *StandardLineItemInput) SetTaxes(v []LineItemTaxInput)`

SetTaxes sets Taxes field to given value.

### HasTaxes

`func (o *StandardLineItemInput) HasTaxes() bool`

HasTaxes returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


