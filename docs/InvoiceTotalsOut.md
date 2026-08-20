# InvoiceTotalsOut

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**GrossSubtotal** | Pointer to [**MoneyOut**](MoneyOut.md) |  | [optional] 
**Subtotal** | [**MoneyOut**](MoneyOut.md) |  | 
**DiscountTotal** | [**MoneyOut**](MoneyOut.md) |  | 
**DocumentDiscountTotal** | Pointer to [**MoneyOut**](MoneyOut.md) |  | [optional] 
**TaxTotal** | [**MoneyOut**](MoneyOut.md) |  | 
**ShippingTotal** | [**MoneyOut**](MoneyOut.md) |  | 
**Total** | [**MoneyOut**](MoneyOut.md) |  | 
**RecomputedTotal** | Pointer to [**NullableMoneyOut**](MoneyOut.md) |  | [optional] 
**TotalsDrift** | Pointer to [**NullableMoneyOut**](MoneyOut.md) |  | [optional] 

## Methods

### NewInvoiceTotalsOut

`func NewInvoiceTotalsOut(subtotal MoneyOut, discountTotal MoneyOut, taxTotal MoneyOut, shippingTotal MoneyOut, total MoneyOut, ) *InvoiceTotalsOut`

NewInvoiceTotalsOut instantiates a new InvoiceTotalsOut object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewInvoiceTotalsOutWithDefaults

`func NewInvoiceTotalsOutWithDefaults() *InvoiceTotalsOut`

NewInvoiceTotalsOutWithDefaults instantiates a new InvoiceTotalsOut object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetGrossSubtotal

`func (o *InvoiceTotalsOut) GetGrossSubtotal() MoneyOut`

GetGrossSubtotal returns the GrossSubtotal field if non-nil, zero value otherwise.

### GetGrossSubtotalOk

`func (o *InvoiceTotalsOut) GetGrossSubtotalOk() (*MoneyOut, bool)`

GetGrossSubtotalOk returns a tuple with the GrossSubtotal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGrossSubtotal

`func (o *InvoiceTotalsOut) SetGrossSubtotal(v MoneyOut)`

SetGrossSubtotal sets GrossSubtotal field to given value.

### HasGrossSubtotal

`func (o *InvoiceTotalsOut) HasGrossSubtotal() bool`

HasGrossSubtotal returns a boolean if a field has been set.

### GetSubtotal

`func (o *InvoiceTotalsOut) GetSubtotal() MoneyOut`

GetSubtotal returns the Subtotal field if non-nil, zero value otherwise.

### GetSubtotalOk

`func (o *InvoiceTotalsOut) GetSubtotalOk() (*MoneyOut, bool)`

GetSubtotalOk returns a tuple with the Subtotal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubtotal

`func (o *InvoiceTotalsOut) SetSubtotal(v MoneyOut)`

SetSubtotal sets Subtotal field to given value.


### GetDiscountTotal

`func (o *InvoiceTotalsOut) GetDiscountTotal() MoneyOut`

GetDiscountTotal returns the DiscountTotal field if non-nil, zero value otherwise.

### GetDiscountTotalOk

`func (o *InvoiceTotalsOut) GetDiscountTotalOk() (*MoneyOut, bool)`

GetDiscountTotalOk returns a tuple with the DiscountTotal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDiscountTotal

`func (o *InvoiceTotalsOut) SetDiscountTotal(v MoneyOut)`

SetDiscountTotal sets DiscountTotal field to given value.


### GetDocumentDiscountTotal

`func (o *InvoiceTotalsOut) GetDocumentDiscountTotal() MoneyOut`

GetDocumentDiscountTotal returns the DocumentDiscountTotal field if non-nil, zero value otherwise.

### GetDocumentDiscountTotalOk

`func (o *InvoiceTotalsOut) GetDocumentDiscountTotalOk() (*MoneyOut, bool)`

GetDocumentDiscountTotalOk returns a tuple with the DocumentDiscountTotal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDocumentDiscountTotal

`func (o *InvoiceTotalsOut) SetDocumentDiscountTotal(v MoneyOut)`

SetDocumentDiscountTotal sets DocumentDiscountTotal field to given value.

### HasDocumentDiscountTotal

`func (o *InvoiceTotalsOut) HasDocumentDiscountTotal() bool`

HasDocumentDiscountTotal returns a boolean if a field has been set.

### GetTaxTotal

`func (o *InvoiceTotalsOut) GetTaxTotal() MoneyOut`

GetTaxTotal returns the TaxTotal field if non-nil, zero value otherwise.

### GetTaxTotalOk

`func (o *InvoiceTotalsOut) GetTaxTotalOk() (*MoneyOut, bool)`

GetTaxTotalOk returns a tuple with the TaxTotal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTaxTotal

`func (o *InvoiceTotalsOut) SetTaxTotal(v MoneyOut)`

SetTaxTotal sets TaxTotal field to given value.


### GetShippingTotal

`func (o *InvoiceTotalsOut) GetShippingTotal() MoneyOut`

GetShippingTotal returns the ShippingTotal field if non-nil, zero value otherwise.

### GetShippingTotalOk

`func (o *InvoiceTotalsOut) GetShippingTotalOk() (*MoneyOut, bool)`

GetShippingTotalOk returns a tuple with the ShippingTotal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippingTotal

`func (o *InvoiceTotalsOut) SetShippingTotal(v MoneyOut)`

SetShippingTotal sets ShippingTotal field to given value.


### GetTotal

`func (o *InvoiceTotalsOut) GetTotal() MoneyOut`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *InvoiceTotalsOut) GetTotalOk() (*MoneyOut, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *InvoiceTotalsOut) SetTotal(v MoneyOut)`

SetTotal sets Total field to given value.


### GetRecomputedTotal

`func (o *InvoiceTotalsOut) GetRecomputedTotal() MoneyOut`

GetRecomputedTotal returns the RecomputedTotal field if non-nil, zero value otherwise.

### GetRecomputedTotalOk

`func (o *InvoiceTotalsOut) GetRecomputedTotalOk() (*MoneyOut, bool)`

GetRecomputedTotalOk returns a tuple with the RecomputedTotal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRecomputedTotal

`func (o *InvoiceTotalsOut) SetRecomputedTotal(v MoneyOut)`

SetRecomputedTotal sets RecomputedTotal field to given value.

### HasRecomputedTotal

`func (o *InvoiceTotalsOut) HasRecomputedTotal() bool`

HasRecomputedTotal returns a boolean if a field has been set.

### SetRecomputedTotalNil

`func (o *InvoiceTotalsOut) SetRecomputedTotalNil(b bool)`

 SetRecomputedTotalNil sets the value for RecomputedTotal to be an explicit nil

### UnsetRecomputedTotal
`func (o *InvoiceTotalsOut) UnsetRecomputedTotal()`

UnsetRecomputedTotal ensures that no value is present for RecomputedTotal, not even an explicit nil
### GetTotalsDrift

`func (o *InvoiceTotalsOut) GetTotalsDrift() MoneyOut`

GetTotalsDrift returns the TotalsDrift field if non-nil, zero value otherwise.

### GetTotalsDriftOk

`func (o *InvoiceTotalsOut) GetTotalsDriftOk() (*MoneyOut, bool)`

GetTotalsDriftOk returns a tuple with the TotalsDrift field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalsDrift

`func (o *InvoiceTotalsOut) SetTotalsDrift(v MoneyOut)`

SetTotalsDrift sets TotalsDrift field to given value.

### HasTotalsDrift

`func (o *InvoiceTotalsOut) HasTotalsDrift() bool`

HasTotalsDrift returns a boolean if a field has been set.

### SetTotalsDriftNil

`func (o *InvoiceTotalsOut) SetTotalsDriftNil(b bool)`

 SetTotalsDriftNil sets the value for TotalsDrift to be an explicit nil

### UnsetTotalsDrift
`func (o *InvoiceTotalsOut) UnsetTotalsDrift()`

UnsetTotalsDrift ensures that no value is present for TotalsDrift, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


