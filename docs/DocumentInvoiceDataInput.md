# DocumentInvoiceDataInput

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**InvoiceNumber** | **string** |  | 
**IssueDate** | **string** |  | 
**DueDate** | Pointer to **NullableString** |  | [optional] 
**Currency** | **string** |  | 
**Seller** | [**DocumentPartyInput**](DocumentPartyInput.md) |  | 
**Buyer** | [**DocumentPartyInput**](DocumentPartyInput.md) |  | 
**ShipTo** | Pointer to [**NullableDocumentPartyInput**](DocumentPartyInput.md) |  | [optional] 
**LineItems** | [**[]DocumentLineItemInput**](DocumentLineItemInput.md) |  | 
**Discounts** | Pointer to [**[]DocumentDiscountInput**](DocumentDiscountInput.md) |  | [optional] 
**Shipping** | Pointer to [**NullableDocumentShippingInput**](DocumentShippingInput.md) |  | [optional] 
**CustomFields** | Pointer to [**[]DocumentCustomFieldInput**](DocumentCustomFieldInput.md) |  | [optional] 
**Payment** | Pointer to [**NullableDocumentPaymentInput**](DocumentPaymentInput.md) |  | [optional] 
**Branding** | Pointer to [**NullableDocumentBrandingInput**](DocumentBrandingInput.md) |  | [optional] 

## Methods

### NewDocumentInvoiceDataInput

`func NewDocumentInvoiceDataInput(invoiceNumber string, issueDate string, currency string, seller DocumentPartyInput, buyer DocumentPartyInput, lineItems []DocumentLineItemInput, ) *DocumentInvoiceDataInput`

NewDocumentInvoiceDataInput instantiates a new DocumentInvoiceDataInput object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDocumentInvoiceDataInputWithDefaults

`func NewDocumentInvoiceDataInputWithDefaults() *DocumentInvoiceDataInput`

NewDocumentInvoiceDataInputWithDefaults instantiates a new DocumentInvoiceDataInput object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetInvoiceNumber

`func (o *DocumentInvoiceDataInput) GetInvoiceNumber() string`

GetInvoiceNumber returns the InvoiceNumber field if non-nil, zero value otherwise.

### GetInvoiceNumberOk

`func (o *DocumentInvoiceDataInput) GetInvoiceNumberOk() (*string, bool)`

GetInvoiceNumberOk returns a tuple with the InvoiceNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInvoiceNumber

`func (o *DocumentInvoiceDataInput) SetInvoiceNumber(v string)`

SetInvoiceNumber sets InvoiceNumber field to given value.


### GetIssueDate

`func (o *DocumentInvoiceDataInput) GetIssueDate() string`

GetIssueDate returns the IssueDate field if non-nil, zero value otherwise.

### GetIssueDateOk

`func (o *DocumentInvoiceDataInput) GetIssueDateOk() (*string, bool)`

GetIssueDateOk returns a tuple with the IssueDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIssueDate

`func (o *DocumentInvoiceDataInput) SetIssueDate(v string)`

SetIssueDate sets IssueDate field to given value.


### GetDueDate

`func (o *DocumentInvoiceDataInput) GetDueDate() string`

GetDueDate returns the DueDate field if non-nil, zero value otherwise.

### GetDueDateOk

`func (o *DocumentInvoiceDataInput) GetDueDateOk() (*string, bool)`

GetDueDateOk returns a tuple with the DueDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDueDate

`func (o *DocumentInvoiceDataInput) SetDueDate(v string)`

SetDueDate sets DueDate field to given value.

### HasDueDate

`func (o *DocumentInvoiceDataInput) HasDueDate() bool`

HasDueDate returns a boolean if a field has been set.

### SetDueDateNil

`func (o *DocumentInvoiceDataInput) SetDueDateNil(b bool)`

 SetDueDateNil sets the value for DueDate to be an explicit nil

### UnsetDueDate
`func (o *DocumentInvoiceDataInput) UnsetDueDate()`

UnsetDueDate ensures that no value is present for DueDate, not even an explicit nil
### GetCurrency

`func (o *DocumentInvoiceDataInput) GetCurrency() string`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *DocumentInvoiceDataInput) GetCurrencyOk() (*string, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *DocumentInvoiceDataInput) SetCurrency(v string)`

SetCurrency sets Currency field to given value.


### GetSeller

`func (o *DocumentInvoiceDataInput) GetSeller() DocumentPartyInput`

GetSeller returns the Seller field if non-nil, zero value otherwise.

### GetSellerOk

`func (o *DocumentInvoiceDataInput) GetSellerOk() (*DocumentPartyInput, bool)`

GetSellerOk returns a tuple with the Seller field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSeller

`func (o *DocumentInvoiceDataInput) SetSeller(v DocumentPartyInput)`

SetSeller sets Seller field to given value.


### GetBuyer

`func (o *DocumentInvoiceDataInput) GetBuyer() DocumentPartyInput`

GetBuyer returns the Buyer field if non-nil, zero value otherwise.

### GetBuyerOk

`func (o *DocumentInvoiceDataInput) GetBuyerOk() (*DocumentPartyInput, bool)`

GetBuyerOk returns a tuple with the Buyer field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuyer

`func (o *DocumentInvoiceDataInput) SetBuyer(v DocumentPartyInput)`

SetBuyer sets Buyer field to given value.


### GetShipTo

`func (o *DocumentInvoiceDataInput) GetShipTo() DocumentPartyInput`

GetShipTo returns the ShipTo field if non-nil, zero value otherwise.

### GetShipToOk

`func (o *DocumentInvoiceDataInput) GetShipToOk() (*DocumentPartyInput, bool)`

GetShipToOk returns a tuple with the ShipTo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShipTo

`func (o *DocumentInvoiceDataInput) SetShipTo(v DocumentPartyInput)`

SetShipTo sets ShipTo field to given value.

### HasShipTo

`func (o *DocumentInvoiceDataInput) HasShipTo() bool`

HasShipTo returns a boolean if a field has been set.

### SetShipToNil

`func (o *DocumentInvoiceDataInput) SetShipToNil(b bool)`

 SetShipToNil sets the value for ShipTo to be an explicit nil

### UnsetShipTo
`func (o *DocumentInvoiceDataInput) UnsetShipTo()`

UnsetShipTo ensures that no value is present for ShipTo, not even an explicit nil
### GetLineItems

`func (o *DocumentInvoiceDataInput) GetLineItems() []DocumentLineItemInput`

GetLineItems returns the LineItems field if non-nil, zero value otherwise.

### GetLineItemsOk

`func (o *DocumentInvoiceDataInput) GetLineItemsOk() (*[]DocumentLineItemInput, bool)`

GetLineItemsOk returns a tuple with the LineItems field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLineItems

`func (o *DocumentInvoiceDataInput) SetLineItems(v []DocumentLineItemInput)`

SetLineItems sets LineItems field to given value.


### GetDiscounts

`func (o *DocumentInvoiceDataInput) GetDiscounts() []DocumentDiscountInput`

GetDiscounts returns the Discounts field if non-nil, zero value otherwise.

### GetDiscountsOk

`func (o *DocumentInvoiceDataInput) GetDiscountsOk() (*[]DocumentDiscountInput, bool)`

GetDiscountsOk returns a tuple with the Discounts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDiscounts

`func (o *DocumentInvoiceDataInput) SetDiscounts(v []DocumentDiscountInput)`

SetDiscounts sets Discounts field to given value.

### HasDiscounts

`func (o *DocumentInvoiceDataInput) HasDiscounts() bool`

HasDiscounts returns a boolean if a field has been set.

### GetShipping

`func (o *DocumentInvoiceDataInput) GetShipping() DocumentShippingInput`

GetShipping returns the Shipping field if non-nil, zero value otherwise.

### GetShippingOk

`func (o *DocumentInvoiceDataInput) GetShippingOk() (*DocumentShippingInput, bool)`

GetShippingOk returns a tuple with the Shipping field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShipping

`func (o *DocumentInvoiceDataInput) SetShipping(v DocumentShippingInput)`

SetShipping sets Shipping field to given value.

### HasShipping

`func (o *DocumentInvoiceDataInput) HasShipping() bool`

HasShipping returns a boolean if a field has been set.

### SetShippingNil

`func (o *DocumentInvoiceDataInput) SetShippingNil(b bool)`

 SetShippingNil sets the value for Shipping to be an explicit nil

### UnsetShipping
`func (o *DocumentInvoiceDataInput) UnsetShipping()`

UnsetShipping ensures that no value is present for Shipping, not even an explicit nil
### GetCustomFields

`func (o *DocumentInvoiceDataInput) GetCustomFields() []DocumentCustomFieldInput`

GetCustomFields returns the CustomFields field if non-nil, zero value otherwise.

### GetCustomFieldsOk

`func (o *DocumentInvoiceDataInput) GetCustomFieldsOk() (*[]DocumentCustomFieldInput, bool)`

GetCustomFieldsOk returns a tuple with the CustomFields field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomFields

`func (o *DocumentInvoiceDataInput) SetCustomFields(v []DocumentCustomFieldInput)`

SetCustomFields sets CustomFields field to given value.

### HasCustomFields

`func (o *DocumentInvoiceDataInput) HasCustomFields() bool`

HasCustomFields returns a boolean if a field has been set.

### GetPayment

`func (o *DocumentInvoiceDataInput) GetPayment() DocumentPaymentInput`

GetPayment returns the Payment field if non-nil, zero value otherwise.

### GetPaymentOk

`func (o *DocumentInvoiceDataInput) GetPaymentOk() (*DocumentPaymentInput, bool)`

GetPaymentOk returns a tuple with the Payment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPayment

`func (o *DocumentInvoiceDataInput) SetPayment(v DocumentPaymentInput)`

SetPayment sets Payment field to given value.

### HasPayment

`func (o *DocumentInvoiceDataInput) HasPayment() bool`

HasPayment returns a boolean if a field has been set.

### SetPaymentNil

`func (o *DocumentInvoiceDataInput) SetPaymentNil(b bool)`

 SetPaymentNil sets the value for Payment to be an explicit nil

### UnsetPayment
`func (o *DocumentInvoiceDataInput) UnsetPayment()`

UnsetPayment ensures that no value is present for Payment, not even an explicit nil
### GetBranding

`func (o *DocumentInvoiceDataInput) GetBranding() DocumentBrandingInput`

GetBranding returns the Branding field if non-nil, zero value otherwise.

### GetBrandingOk

`func (o *DocumentInvoiceDataInput) GetBrandingOk() (*DocumentBrandingInput, bool)`

GetBrandingOk returns a tuple with the Branding field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBranding

`func (o *DocumentInvoiceDataInput) SetBranding(v DocumentBrandingInput)`

SetBranding sets Branding field to given value.

### HasBranding

`func (o *DocumentInvoiceDataInput) HasBranding() bool`

HasBranding returns a boolean if a field has been set.

### SetBrandingNil

`func (o *DocumentInvoiceDataInput) SetBrandingNil(b bool)`

 SetBrandingNil sets the value for Branding to be an explicit nil

### UnsetBranding
`func (o *DocumentInvoiceDataInput) UnsetBranding()`

UnsetBranding ensures that no value is present for Branding, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


