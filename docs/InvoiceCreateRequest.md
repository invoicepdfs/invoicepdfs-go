# InvoiceCreateRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**InvoiceNumber** | **string** |  | 
**DocumentType** | Pointer to **string** |  | [optional] [default to "invoice"]
**IssueDate** | **string** |  | 
**DueDate** | Pointer to **NullableString** |  | [optional] 
**Currency** | **string** |  | 
**Locale** | Pointer to **NullableString** |  | [optional] 
**BusinessProfileId** | **string** |  | 
**CustomerId** | **string** |  | 
**ShipTo** | Pointer to [**NullablePostalAddress**](PostalAddress.md) |  | [optional] 
**LineItems** | [**[]InvoiceLineItemInput**](InvoiceLineItemInput.md) |  | 
**Discounts** | Pointer to [**[]InvoiceDiscountInput**](InvoiceDiscountInput.md) |  | [optional] 
**Shipping** | Pointer to [**NullableInvoiceShippingInput**](InvoiceShippingInput.md) |  | [optional] 
**Notes** | Pointer to [**[]InvoiceNoteInput**](InvoiceNoteInput.md) |  | [optional] 
**Terms** | Pointer to [**[]InvoiceTermInput**](InvoiceTermInput.md) |  | [optional] 
**CustomFields** | Pointer to [**[]InvoiceCustomFieldInput**](InvoiceCustomFieldInput.md) |  | [optional] 
**Payment** | Pointer to [**NullableInvoicePaymentInput**](InvoicePaymentInput.md) |  | [optional] 
**Branding** | Pointer to [**NullableInvoiceBrandingInput**](InvoiceBrandingInput.md) |  | [optional] 

## Methods

### NewInvoiceCreateRequest

`func NewInvoiceCreateRequest(invoiceNumber string, issueDate string, currency string, businessProfileId string, customerId string, lineItems []InvoiceLineItemInput, ) *InvoiceCreateRequest`

NewInvoiceCreateRequest instantiates a new InvoiceCreateRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewInvoiceCreateRequestWithDefaults

`func NewInvoiceCreateRequestWithDefaults() *InvoiceCreateRequest`

NewInvoiceCreateRequestWithDefaults instantiates a new InvoiceCreateRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetInvoiceNumber

`func (o *InvoiceCreateRequest) GetInvoiceNumber() string`

GetInvoiceNumber returns the InvoiceNumber field if non-nil, zero value otherwise.

### GetInvoiceNumberOk

`func (o *InvoiceCreateRequest) GetInvoiceNumberOk() (*string, bool)`

GetInvoiceNumberOk returns a tuple with the InvoiceNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInvoiceNumber

`func (o *InvoiceCreateRequest) SetInvoiceNumber(v string)`

SetInvoiceNumber sets InvoiceNumber field to given value.


### GetDocumentType

`func (o *InvoiceCreateRequest) GetDocumentType() string`

GetDocumentType returns the DocumentType field if non-nil, zero value otherwise.

### GetDocumentTypeOk

`func (o *InvoiceCreateRequest) GetDocumentTypeOk() (*string, bool)`

GetDocumentTypeOk returns a tuple with the DocumentType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDocumentType

`func (o *InvoiceCreateRequest) SetDocumentType(v string)`

SetDocumentType sets DocumentType field to given value.

### HasDocumentType

`func (o *InvoiceCreateRequest) HasDocumentType() bool`

HasDocumentType returns a boolean if a field has been set.

### GetIssueDate

`func (o *InvoiceCreateRequest) GetIssueDate() string`

GetIssueDate returns the IssueDate field if non-nil, zero value otherwise.

### GetIssueDateOk

`func (o *InvoiceCreateRequest) GetIssueDateOk() (*string, bool)`

GetIssueDateOk returns a tuple with the IssueDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIssueDate

`func (o *InvoiceCreateRequest) SetIssueDate(v string)`

SetIssueDate sets IssueDate field to given value.


### GetDueDate

`func (o *InvoiceCreateRequest) GetDueDate() string`

GetDueDate returns the DueDate field if non-nil, zero value otherwise.

### GetDueDateOk

`func (o *InvoiceCreateRequest) GetDueDateOk() (*string, bool)`

GetDueDateOk returns a tuple with the DueDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDueDate

`func (o *InvoiceCreateRequest) SetDueDate(v string)`

SetDueDate sets DueDate field to given value.

### HasDueDate

`func (o *InvoiceCreateRequest) HasDueDate() bool`

HasDueDate returns a boolean if a field has been set.

### SetDueDateNil

`func (o *InvoiceCreateRequest) SetDueDateNil(b bool)`

 SetDueDateNil sets the value for DueDate to be an explicit nil

### UnsetDueDate
`func (o *InvoiceCreateRequest) UnsetDueDate()`

UnsetDueDate ensures that no value is present for DueDate, not even an explicit nil
### GetCurrency

`func (o *InvoiceCreateRequest) GetCurrency() string`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *InvoiceCreateRequest) GetCurrencyOk() (*string, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *InvoiceCreateRequest) SetCurrency(v string)`

SetCurrency sets Currency field to given value.


### GetLocale

`func (o *InvoiceCreateRequest) GetLocale() string`

GetLocale returns the Locale field if non-nil, zero value otherwise.

### GetLocaleOk

`func (o *InvoiceCreateRequest) GetLocaleOk() (*string, bool)`

GetLocaleOk returns a tuple with the Locale field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLocale

`func (o *InvoiceCreateRequest) SetLocale(v string)`

SetLocale sets Locale field to given value.

### HasLocale

`func (o *InvoiceCreateRequest) HasLocale() bool`

HasLocale returns a boolean if a field has been set.

### SetLocaleNil

`func (o *InvoiceCreateRequest) SetLocaleNil(b bool)`

 SetLocaleNil sets the value for Locale to be an explicit nil

### UnsetLocale
`func (o *InvoiceCreateRequest) UnsetLocale()`

UnsetLocale ensures that no value is present for Locale, not even an explicit nil
### GetBusinessProfileId

`func (o *InvoiceCreateRequest) GetBusinessProfileId() string`

GetBusinessProfileId returns the BusinessProfileId field if non-nil, zero value otherwise.

### GetBusinessProfileIdOk

`func (o *InvoiceCreateRequest) GetBusinessProfileIdOk() (*string, bool)`

GetBusinessProfileIdOk returns a tuple with the BusinessProfileId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBusinessProfileId

`func (o *InvoiceCreateRequest) SetBusinessProfileId(v string)`

SetBusinessProfileId sets BusinessProfileId field to given value.


### GetCustomerId

`func (o *InvoiceCreateRequest) GetCustomerId() string`

GetCustomerId returns the CustomerId field if non-nil, zero value otherwise.

### GetCustomerIdOk

`func (o *InvoiceCreateRequest) GetCustomerIdOk() (*string, bool)`

GetCustomerIdOk returns a tuple with the CustomerId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomerId

`func (o *InvoiceCreateRequest) SetCustomerId(v string)`

SetCustomerId sets CustomerId field to given value.


### GetShipTo

`func (o *InvoiceCreateRequest) GetShipTo() PostalAddress`

GetShipTo returns the ShipTo field if non-nil, zero value otherwise.

### GetShipToOk

`func (o *InvoiceCreateRequest) GetShipToOk() (*PostalAddress, bool)`

GetShipToOk returns a tuple with the ShipTo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShipTo

`func (o *InvoiceCreateRequest) SetShipTo(v PostalAddress)`

SetShipTo sets ShipTo field to given value.

### HasShipTo

`func (o *InvoiceCreateRequest) HasShipTo() bool`

HasShipTo returns a boolean if a field has been set.

### SetShipToNil

`func (o *InvoiceCreateRequest) SetShipToNil(b bool)`

 SetShipToNil sets the value for ShipTo to be an explicit nil

### UnsetShipTo
`func (o *InvoiceCreateRequest) UnsetShipTo()`

UnsetShipTo ensures that no value is present for ShipTo, not even an explicit nil
### GetLineItems

`func (o *InvoiceCreateRequest) GetLineItems() []InvoiceLineItemInput`

GetLineItems returns the LineItems field if non-nil, zero value otherwise.

### GetLineItemsOk

`func (o *InvoiceCreateRequest) GetLineItemsOk() (*[]InvoiceLineItemInput, bool)`

GetLineItemsOk returns a tuple with the LineItems field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLineItems

`func (o *InvoiceCreateRequest) SetLineItems(v []InvoiceLineItemInput)`

SetLineItems sets LineItems field to given value.


### GetDiscounts

`func (o *InvoiceCreateRequest) GetDiscounts() []InvoiceDiscountInput`

GetDiscounts returns the Discounts field if non-nil, zero value otherwise.

### GetDiscountsOk

`func (o *InvoiceCreateRequest) GetDiscountsOk() (*[]InvoiceDiscountInput, bool)`

GetDiscountsOk returns a tuple with the Discounts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDiscounts

`func (o *InvoiceCreateRequest) SetDiscounts(v []InvoiceDiscountInput)`

SetDiscounts sets Discounts field to given value.

### HasDiscounts

`func (o *InvoiceCreateRequest) HasDiscounts() bool`

HasDiscounts returns a boolean if a field has been set.

### GetShipping

`func (o *InvoiceCreateRequest) GetShipping() InvoiceShippingInput`

GetShipping returns the Shipping field if non-nil, zero value otherwise.

### GetShippingOk

`func (o *InvoiceCreateRequest) GetShippingOk() (*InvoiceShippingInput, bool)`

GetShippingOk returns a tuple with the Shipping field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShipping

`func (o *InvoiceCreateRequest) SetShipping(v InvoiceShippingInput)`

SetShipping sets Shipping field to given value.

### HasShipping

`func (o *InvoiceCreateRequest) HasShipping() bool`

HasShipping returns a boolean if a field has been set.

### SetShippingNil

`func (o *InvoiceCreateRequest) SetShippingNil(b bool)`

 SetShippingNil sets the value for Shipping to be an explicit nil

### UnsetShipping
`func (o *InvoiceCreateRequest) UnsetShipping()`

UnsetShipping ensures that no value is present for Shipping, not even an explicit nil
### GetNotes

`func (o *InvoiceCreateRequest) GetNotes() []InvoiceNoteInput`

GetNotes returns the Notes field if non-nil, zero value otherwise.

### GetNotesOk

`func (o *InvoiceCreateRequest) GetNotesOk() (*[]InvoiceNoteInput, bool)`

GetNotesOk returns a tuple with the Notes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNotes

`func (o *InvoiceCreateRequest) SetNotes(v []InvoiceNoteInput)`

SetNotes sets Notes field to given value.

### HasNotes

`func (o *InvoiceCreateRequest) HasNotes() bool`

HasNotes returns a boolean if a field has been set.

### GetTerms

`func (o *InvoiceCreateRequest) GetTerms() []InvoiceTermInput`

GetTerms returns the Terms field if non-nil, zero value otherwise.

### GetTermsOk

`func (o *InvoiceCreateRequest) GetTermsOk() (*[]InvoiceTermInput, bool)`

GetTermsOk returns a tuple with the Terms field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTerms

`func (o *InvoiceCreateRequest) SetTerms(v []InvoiceTermInput)`

SetTerms sets Terms field to given value.

### HasTerms

`func (o *InvoiceCreateRequest) HasTerms() bool`

HasTerms returns a boolean if a field has been set.

### GetCustomFields

`func (o *InvoiceCreateRequest) GetCustomFields() []InvoiceCustomFieldInput`

GetCustomFields returns the CustomFields field if non-nil, zero value otherwise.

### GetCustomFieldsOk

`func (o *InvoiceCreateRequest) GetCustomFieldsOk() (*[]InvoiceCustomFieldInput, bool)`

GetCustomFieldsOk returns a tuple with the CustomFields field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomFields

`func (o *InvoiceCreateRequest) SetCustomFields(v []InvoiceCustomFieldInput)`

SetCustomFields sets CustomFields field to given value.

### HasCustomFields

`func (o *InvoiceCreateRequest) HasCustomFields() bool`

HasCustomFields returns a boolean if a field has been set.

### GetPayment

`func (o *InvoiceCreateRequest) GetPayment() InvoicePaymentInput`

GetPayment returns the Payment field if non-nil, zero value otherwise.

### GetPaymentOk

`func (o *InvoiceCreateRequest) GetPaymentOk() (*InvoicePaymentInput, bool)`

GetPaymentOk returns a tuple with the Payment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPayment

`func (o *InvoiceCreateRequest) SetPayment(v InvoicePaymentInput)`

SetPayment sets Payment field to given value.

### HasPayment

`func (o *InvoiceCreateRequest) HasPayment() bool`

HasPayment returns a boolean if a field has been set.

### SetPaymentNil

`func (o *InvoiceCreateRequest) SetPaymentNil(b bool)`

 SetPaymentNil sets the value for Payment to be an explicit nil

### UnsetPayment
`func (o *InvoiceCreateRequest) UnsetPayment()`

UnsetPayment ensures that no value is present for Payment, not even an explicit nil
### GetBranding

`func (o *InvoiceCreateRequest) GetBranding() InvoiceBrandingInput`

GetBranding returns the Branding field if non-nil, zero value otherwise.

### GetBrandingOk

`func (o *InvoiceCreateRequest) GetBrandingOk() (*InvoiceBrandingInput, bool)`

GetBrandingOk returns a tuple with the Branding field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBranding

`func (o *InvoiceCreateRequest) SetBranding(v InvoiceBrandingInput)`

SetBranding sets Branding field to given value.

### HasBranding

`func (o *InvoiceCreateRequest) HasBranding() bool`

HasBranding returns a boolean if a field has been set.

### SetBrandingNil

`func (o *InvoiceCreateRequest) SetBrandingNil(b bool)`

 SetBrandingNil sets the value for Branding to be an explicit nil

### UnsetBranding
`func (o *InvoiceCreateRequest) UnsetBranding()`

UnsetBranding ensures that no value is present for Branding, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


