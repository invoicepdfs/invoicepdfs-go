# InvoiceTotalsOut

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Subtotal** | [**MoneyOut**](MoneyOut.md) |  | 
**DiscountTotal** | [**MoneyOut**](MoneyOut.md) |  | 
**TaxTotal** | [**MoneyOut**](MoneyOut.md) |  | 
**ShippingTotal** | [**MoneyOut**](MoneyOut.md) |  | 
**Total** | [**MoneyOut**](MoneyOut.md) |  | 

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



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


