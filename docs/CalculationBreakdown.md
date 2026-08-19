# CalculationBreakdown

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Subtotal** | [**Money**](Money.md) |  | 
**DiscountTotal** | [**Money**](Money.md) |  | 
**DocumentDiscountTotal** | Pointer to [**Money**](Money.md) |  | [optional] 
**TaxTotal** | [**Money**](Money.md) |  | 
**ShippingTotal** | [**Money**](Money.md) |  | 
**Total** | [**Money**](Money.md) |  | 

## Methods

### NewCalculationBreakdown

`func NewCalculationBreakdown(subtotal Money, discountTotal Money, taxTotal Money, shippingTotal Money, total Money, ) *CalculationBreakdown`

NewCalculationBreakdown instantiates a new CalculationBreakdown object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCalculationBreakdownWithDefaults

`func NewCalculationBreakdownWithDefaults() *CalculationBreakdown`

NewCalculationBreakdownWithDefaults instantiates a new CalculationBreakdown object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSubtotal

`func (o *CalculationBreakdown) GetSubtotal() Money`

GetSubtotal returns the Subtotal field if non-nil, zero value otherwise.

### GetSubtotalOk

`func (o *CalculationBreakdown) GetSubtotalOk() (*Money, bool)`

GetSubtotalOk returns a tuple with the Subtotal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubtotal

`func (o *CalculationBreakdown) SetSubtotal(v Money)`

SetSubtotal sets Subtotal field to given value.


### GetDiscountTotal

`func (o *CalculationBreakdown) GetDiscountTotal() Money`

GetDiscountTotal returns the DiscountTotal field if non-nil, zero value otherwise.

### GetDiscountTotalOk

`func (o *CalculationBreakdown) GetDiscountTotalOk() (*Money, bool)`

GetDiscountTotalOk returns a tuple with the DiscountTotal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDiscountTotal

`func (o *CalculationBreakdown) SetDiscountTotal(v Money)`

SetDiscountTotal sets DiscountTotal field to given value.


### GetDocumentDiscountTotal

`func (o *CalculationBreakdown) GetDocumentDiscountTotal() Money`

GetDocumentDiscountTotal returns the DocumentDiscountTotal field if non-nil, zero value otherwise.

### GetDocumentDiscountTotalOk

`func (o *CalculationBreakdown) GetDocumentDiscountTotalOk() (*Money, bool)`

GetDocumentDiscountTotalOk returns a tuple with the DocumentDiscountTotal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDocumentDiscountTotal

`func (o *CalculationBreakdown) SetDocumentDiscountTotal(v Money)`

SetDocumentDiscountTotal sets DocumentDiscountTotal field to given value.

### HasDocumentDiscountTotal

`func (o *CalculationBreakdown) HasDocumentDiscountTotal() bool`

HasDocumentDiscountTotal returns a boolean if a field has been set.

### GetTaxTotal

`func (o *CalculationBreakdown) GetTaxTotal() Money`

GetTaxTotal returns the TaxTotal field if non-nil, zero value otherwise.

### GetTaxTotalOk

`func (o *CalculationBreakdown) GetTaxTotalOk() (*Money, bool)`

GetTaxTotalOk returns a tuple with the TaxTotal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTaxTotal

`func (o *CalculationBreakdown) SetTaxTotal(v Money)`

SetTaxTotal sets TaxTotal field to given value.


### GetShippingTotal

`func (o *CalculationBreakdown) GetShippingTotal() Money`

GetShippingTotal returns the ShippingTotal field if non-nil, zero value otherwise.

### GetShippingTotalOk

`func (o *CalculationBreakdown) GetShippingTotalOk() (*Money, bool)`

GetShippingTotalOk returns a tuple with the ShippingTotal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippingTotal

`func (o *CalculationBreakdown) SetShippingTotal(v Money)`

SetShippingTotal sets ShippingTotal field to given value.


### GetTotal

`func (o *CalculationBreakdown) GetTotal() Money`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *CalculationBreakdown) GetTotalOk() (*Money, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *CalculationBreakdown) SetTotal(v Money)`

SetTotal sets Total field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


