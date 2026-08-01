# DocumentLineItemInput

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** |  | 
**Description** | Pointer to **NullableString** |  | [optional] 
**Quantity** | **string** |  | 
**UnitPrice** | **string** | Decimal string in major units | 
**Unit** | Pointer to **NullableString** |  | [optional] 
**Sku** | Pointer to **NullableString** |  | [optional] 
**Discount** | Pointer to [**NullableDocumentDiscountInput**](DocumentDiscountInput.md) |  | [optional] 
**Taxes** | Pointer to [**[]DocumentLineItemTaxInput**](DocumentLineItemTaxInput.md) |  | [optional] 

## Methods

### NewDocumentLineItemInput

`func NewDocumentLineItemInput(name string, quantity string, unitPrice string, ) *DocumentLineItemInput`

NewDocumentLineItemInput instantiates a new DocumentLineItemInput object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDocumentLineItemInputWithDefaults

`func NewDocumentLineItemInputWithDefaults() *DocumentLineItemInput`

NewDocumentLineItemInputWithDefaults instantiates a new DocumentLineItemInput object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *DocumentLineItemInput) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *DocumentLineItemInput) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *DocumentLineItemInput) SetName(v string)`

SetName sets Name field to given value.


### GetDescription

`func (o *DocumentLineItemInput) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *DocumentLineItemInput) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *DocumentLineItemInput) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *DocumentLineItemInput) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *DocumentLineItemInput) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *DocumentLineItemInput) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetQuantity

`func (o *DocumentLineItemInput) GetQuantity() string`

GetQuantity returns the Quantity field if non-nil, zero value otherwise.

### GetQuantityOk

`func (o *DocumentLineItemInput) GetQuantityOk() (*string, bool)`

GetQuantityOk returns a tuple with the Quantity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuantity

`func (o *DocumentLineItemInput) SetQuantity(v string)`

SetQuantity sets Quantity field to given value.


### GetUnitPrice

`func (o *DocumentLineItemInput) GetUnitPrice() string`

GetUnitPrice returns the UnitPrice field if non-nil, zero value otherwise.

### GetUnitPriceOk

`func (o *DocumentLineItemInput) GetUnitPriceOk() (*string, bool)`

GetUnitPriceOk returns a tuple with the UnitPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUnitPrice

`func (o *DocumentLineItemInput) SetUnitPrice(v string)`

SetUnitPrice sets UnitPrice field to given value.


### GetUnit

`func (o *DocumentLineItemInput) GetUnit() string`

GetUnit returns the Unit field if non-nil, zero value otherwise.

### GetUnitOk

`func (o *DocumentLineItemInput) GetUnitOk() (*string, bool)`

GetUnitOk returns a tuple with the Unit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUnit

`func (o *DocumentLineItemInput) SetUnit(v string)`

SetUnit sets Unit field to given value.

### HasUnit

`func (o *DocumentLineItemInput) HasUnit() bool`

HasUnit returns a boolean if a field has been set.

### SetUnitNil

`func (o *DocumentLineItemInput) SetUnitNil(b bool)`

 SetUnitNil sets the value for Unit to be an explicit nil

### UnsetUnit
`func (o *DocumentLineItemInput) UnsetUnit()`

UnsetUnit ensures that no value is present for Unit, not even an explicit nil
### GetSku

`func (o *DocumentLineItemInput) GetSku() string`

GetSku returns the Sku field if non-nil, zero value otherwise.

### GetSkuOk

`func (o *DocumentLineItemInput) GetSkuOk() (*string, bool)`

GetSkuOk returns a tuple with the Sku field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSku

`func (o *DocumentLineItemInput) SetSku(v string)`

SetSku sets Sku field to given value.

### HasSku

`func (o *DocumentLineItemInput) HasSku() bool`

HasSku returns a boolean if a field has been set.

### SetSkuNil

`func (o *DocumentLineItemInput) SetSkuNil(b bool)`

 SetSkuNil sets the value for Sku to be an explicit nil

### UnsetSku
`func (o *DocumentLineItemInput) UnsetSku()`

UnsetSku ensures that no value is present for Sku, not even an explicit nil
### GetDiscount

`func (o *DocumentLineItemInput) GetDiscount() DocumentDiscountInput`

GetDiscount returns the Discount field if non-nil, zero value otherwise.

### GetDiscountOk

`func (o *DocumentLineItemInput) GetDiscountOk() (*DocumentDiscountInput, bool)`

GetDiscountOk returns a tuple with the Discount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDiscount

`func (o *DocumentLineItemInput) SetDiscount(v DocumentDiscountInput)`

SetDiscount sets Discount field to given value.

### HasDiscount

`func (o *DocumentLineItemInput) HasDiscount() bool`

HasDiscount returns a boolean if a field has been set.

### SetDiscountNil

`func (o *DocumentLineItemInput) SetDiscountNil(b bool)`

 SetDiscountNil sets the value for Discount to be an explicit nil

### UnsetDiscount
`func (o *DocumentLineItemInput) UnsetDiscount()`

UnsetDiscount ensures that no value is present for Discount, not even an explicit nil
### GetTaxes

`func (o *DocumentLineItemInput) GetTaxes() []DocumentLineItemTaxInput`

GetTaxes returns the Taxes field if non-nil, zero value otherwise.

### GetTaxesOk

`func (o *DocumentLineItemInput) GetTaxesOk() (*[]DocumentLineItemTaxInput, bool)`

GetTaxesOk returns a tuple with the Taxes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTaxes

`func (o *DocumentLineItemInput) SetTaxes(v []DocumentLineItemTaxInput)`

SetTaxes sets Taxes field to given value.

### HasTaxes

`func (o *DocumentLineItemInput) HasTaxes() bool`

HasTaxes returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


