# InvoicePreviewRequest

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
**TemplateId** | Pointer to **string** |  | [optional] [default to "tpl_modern"]
**PageSize** | Pointer to **string** |  | [optional] [default to "LETTER"]

## Methods

### NewInvoicePreviewRequest

`func NewInvoicePreviewRequest(invoiceNumber string, issueDate string, currency string, businessProfileId string, customerId string, lineItems []InvoiceLineItemInput, ) *InvoicePreviewRequest`

NewInvoicePreviewRequest instantiates a new InvoicePreviewRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewInvoicePreviewRequestWithDefaults

`func NewInvoicePreviewRequestWithDefaults() *InvoicePreviewRequest`

NewInvoicePreviewRequestWithDefaults instantiates a new InvoicePreviewRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetInvoiceNumber

`func (o *InvoicePreviewRequest) GetInvoiceNumber() string`

GetInvoiceNumber returns the InvoiceNumber field if non-nil, zero value otherwise.

### GetInvoiceNumberOk

`func (o *InvoicePreviewRequest) GetInvoiceNumberOk() (*string, bool)`

GetInvoiceNumberOk returns a tuple with the InvoiceNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInvoiceNumber

`func (o *InvoicePreviewRequest) SetInvoiceNumber(v string)`

SetInvoiceNumber sets InvoiceNumber field to given value.


### GetDocumentType

`func (o *InvoicePreviewRequest) GetDocumentType() string`

GetDocumentType returns the DocumentType field if non-nil, zero value otherwise.

### GetDocumentTypeOk

`func (o *InvoicePreviewRequest) GetDocumentTypeOk() (*string, bool)`

GetDocumentTypeOk returns a tuple with the DocumentType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDocumentType

`func (o *InvoicePreviewRequest) SetDocumentType(v string)`

SetDocumentType sets DocumentType field to given value.

### HasDocumentType

`func (o *InvoicePreviewRequest) HasDocumentType() bool`

HasDocumentType returns a boolean if a field has been set.

### GetIssueDate

`func (o *InvoicePreviewRequest) GetIssueDate() string`

GetIssueDate returns the IssueDate field if non-nil, zero value otherwise.

### GetIssueDateOk

`func (o *InvoicePreviewRequest) GetIssueDateOk() (*string, bool)`

GetIssueDateOk returns a tuple with the IssueDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIssueDate

`func (o *InvoicePreviewRequest) SetIssueDate(v string)`

SetIssueDate sets IssueDate field to given value.


### GetDueDate

`func (o *InvoicePreviewRequest) GetDueDate() string`

GetDueDate returns the DueDate field if non-nil, zero value otherwise.

### GetDueDateOk

`func (o *InvoicePreviewRequest) GetDueDateOk() (*string, bool)`

GetDueDateOk returns a tuple with the DueDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDueDate

`func (o *InvoicePreviewRequest) SetDueDate(v string)`

SetDueDate sets DueDate field to given value.

### HasDueDate

`func (o *InvoicePreviewRequest) HasDueDate() bool`

HasDueDate returns a boolean if a field has been set.

### SetDueDateNil

`func (o *InvoicePreviewRequest) SetDueDateNil(b bool)`

 SetDueDateNil sets the value for DueDate to be an explicit nil

### UnsetDueDate
`func (o *InvoicePreviewRequest) UnsetDueDate()`

UnsetDueDate ensures that no value is present for DueDate, not even an explicit nil
### GetCurrency

`func (o *InvoicePreviewRequest) GetCurrency() string`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *InvoicePreviewRequest) GetCurrencyOk() (*string, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *InvoicePreviewRequest) SetCurrency(v string)`

SetCurrency sets Currency field to given value.


### GetLocale

`func (o *InvoicePreviewRequest) GetLocale() string`

GetLocale returns the Locale field if non-nil, zero value otherwise.

### GetLocaleOk

`func (o *InvoicePreviewRequest) GetLocaleOk() (*string, bool)`

GetLocaleOk returns a tuple with the Locale field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLocale

`func (o *InvoicePreviewRequest) SetLocale(v string)`

SetLocale sets Locale field to given value.

### HasLocale

`func (o *InvoicePreviewRequest) HasLocale() bool`

HasLocale returns a boolean if a field has been set.

### SetLocaleNil

`func (o *InvoicePreviewRequest) SetLocaleNil(b bool)`

 SetLocaleNil sets the value for Locale to be an explicit nil

### UnsetLocale
`func (o *InvoicePreviewRequest) UnsetLocale()`

UnsetLocale ensures that no value is present for Locale, not even an explicit nil
### GetBusinessProfileId

`func (o *InvoicePreviewRequest) GetBusinessProfileId() string`

GetBusinessProfileId returns the BusinessProfileId field if non-nil, zero value otherwise.

### GetBusinessProfileIdOk

`func (o *InvoicePreviewRequest) GetBusinessProfileIdOk() (*string, bool)`

GetBusinessProfileIdOk returns a tuple with the BusinessProfileId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBusinessProfileId

`func (o *InvoicePreviewRequest) SetBusinessProfileId(v string)`

SetBusinessProfileId sets BusinessProfileId field to given value.


### GetCustomerId

`func (o *InvoicePreviewRequest) GetCustomerId() string`

GetCustomerId returns the CustomerId field if non-nil, zero value otherwise.

### GetCustomerIdOk

`func (o *InvoicePreviewRequest) GetCustomerIdOk() (*string, bool)`

GetCustomerIdOk returns a tuple with the CustomerId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomerId

`func (o *InvoicePreviewRequest) SetCustomerId(v string)`

SetCustomerId sets CustomerId field to given value.


### GetShipTo

`func (o *InvoicePreviewRequest) GetShipTo() PostalAddress`

GetShipTo returns the ShipTo field if non-nil, zero value otherwise.

### GetShipToOk

`func (o *InvoicePreviewRequest) GetShipToOk() (*PostalAddress, bool)`

GetShipToOk returns a tuple with the ShipTo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShipTo

`func (o *InvoicePreviewRequest) SetShipTo(v PostalAddress)`

SetShipTo sets ShipTo field to given value.

### HasShipTo

`func (o *InvoicePreviewRequest) HasShipTo() bool`

HasShipTo returns a boolean if a field has been set.

### SetShipToNil

`func (o *InvoicePreviewRequest) SetShipToNil(b bool)`

 SetShipToNil sets the value for ShipTo to be an explicit nil

### UnsetShipTo
`func (o *InvoicePreviewRequest) UnsetShipTo()`

UnsetShipTo ensures that no value is present for ShipTo, not even an explicit nil
### GetLineItems

`func (o *InvoicePreviewRequest) GetLineItems() []InvoiceLineItemInput`

GetLineItems returns the LineItems field if non-nil, zero value otherwise.

### GetLineItemsOk

`func (o *InvoicePreviewRequest) GetLineItemsOk() (*[]InvoiceLineItemInput, bool)`

GetLineItemsOk returns a tuple with the LineItems field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLineItems

`func (o *InvoicePreviewRequest) SetLineItems(v []InvoiceLineItemInput)`

SetLineItems sets LineItems field to given value.


### GetDiscounts

`func (o *InvoicePreviewRequest) GetDiscounts() []InvoiceDiscountInput`

GetDiscounts returns the Discounts field if non-nil, zero value otherwise.

### GetDiscountsOk

`func (o *InvoicePreviewRequest) GetDiscountsOk() (*[]InvoiceDiscountInput, bool)`

GetDiscountsOk returns a tuple with the Discounts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDiscounts

`func (o *InvoicePreviewRequest) SetDiscounts(v []InvoiceDiscountInput)`

SetDiscounts sets Discounts field to given value.

### HasDiscounts

`func (o *InvoicePreviewRequest) HasDiscounts() bool`

HasDiscounts returns a boolean if a field has been set.

### GetShipping

`func (o *InvoicePreviewRequest) GetShipping() InvoiceShippingInput`

GetShipping returns the Shipping field if non-nil, zero value otherwise.

### GetShippingOk

`func (o *InvoicePreviewRequest) GetShippingOk() (*InvoiceShippingInput, bool)`

GetShippingOk returns a tuple with the Shipping field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShipping

`func (o *InvoicePreviewRequest) SetShipping(v InvoiceShippingInput)`

SetShipping sets Shipping field to given value.

### HasShipping

`func (o *InvoicePreviewRequest) HasShipping() bool`

HasShipping returns a boolean if a field has been set.

### SetShippingNil

`func (o *InvoicePreviewRequest) SetShippingNil(b bool)`

 SetShippingNil sets the value for Shipping to be an explicit nil

### UnsetShipping
`func (o *InvoicePreviewRequest) UnsetShipping()`

UnsetShipping ensures that no value is present for Shipping, not even an explicit nil
### GetNotes

`func (o *InvoicePreviewRequest) GetNotes() []InvoiceNoteInput`

GetNotes returns the Notes field if non-nil, zero value otherwise.

### GetNotesOk

`func (o *InvoicePreviewRequest) GetNotesOk() (*[]InvoiceNoteInput, bool)`

GetNotesOk returns a tuple with the Notes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNotes

`func (o *InvoicePreviewRequest) SetNotes(v []InvoiceNoteInput)`

SetNotes sets Notes field to given value.

### HasNotes

`func (o *InvoicePreviewRequest) HasNotes() bool`

HasNotes returns a boolean if a field has been set.

### GetTerms

`func (o *InvoicePreviewRequest) GetTerms() []InvoiceTermInput`

GetTerms returns the Terms field if non-nil, zero value otherwise.

### GetTermsOk

`func (o *InvoicePreviewRequest) GetTermsOk() (*[]InvoiceTermInput, bool)`

GetTermsOk returns a tuple with the Terms field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTerms

`func (o *InvoicePreviewRequest) SetTerms(v []InvoiceTermInput)`

SetTerms sets Terms field to given value.

### HasTerms

`func (o *InvoicePreviewRequest) HasTerms() bool`

HasTerms returns a boolean if a field has been set.

### GetCustomFields

`func (o *InvoicePreviewRequest) GetCustomFields() []InvoiceCustomFieldInput`

GetCustomFields returns the CustomFields field if non-nil, zero value otherwise.

### GetCustomFieldsOk

`func (o *InvoicePreviewRequest) GetCustomFieldsOk() (*[]InvoiceCustomFieldInput, bool)`

GetCustomFieldsOk returns a tuple with the CustomFields field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomFields

`func (o *InvoicePreviewRequest) SetCustomFields(v []InvoiceCustomFieldInput)`

SetCustomFields sets CustomFields field to given value.

### HasCustomFields

`func (o *InvoicePreviewRequest) HasCustomFields() bool`

HasCustomFields returns a boolean if a field has been set.

### GetPayment

`func (o *InvoicePreviewRequest) GetPayment() InvoicePaymentInput`

GetPayment returns the Payment field if non-nil, zero value otherwise.

### GetPaymentOk

`func (o *InvoicePreviewRequest) GetPaymentOk() (*InvoicePaymentInput, bool)`

GetPaymentOk returns a tuple with the Payment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPayment

`func (o *InvoicePreviewRequest) SetPayment(v InvoicePaymentInput)`

SetPayment sets Payment field to given value.

### HasPayment

`func (o *InvoicePreviewRequest) HasPayment() bool`

HasPayment returns a boolean if a field has been set.

### SetPaymentNil

`func (o *InvoicePreviewRequest) SetPaymentNil(b bool)`

 SetPaymentNil sets the value for Payment to be an explicit nil

### UnsetPayment
`func (o *InvoicePreviewRequest) UnsetPayment()`

UnsetPayment ensures that no value is present for Payment, not even an explicit nil
### GetBranding

`func (o *InvoicePreviewRequest) GetBranding() InvoiceBrandingInput`

GetBranding returns the Branding field if non-nil, zero value otherwise.

### GetBrandingOk

`func (o *InvoicePreviewRequest) GetBrandingOk() (*InvoiceBrandingInput, bool)`

GetBrandingOk returns a tuple with the Branding field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBranding

`func (o *InvoicePreviewRequest) SetBranding(v InvoiceBrandingInput)`

SetBranding sets Branding field to given value.

### HasBranding

`func (o *InvoicePreviewRequest) HasBranding() bool`

HasBranding returns a boolean if a field has been set.

### SetBrandingNil

`func (o *InvoicePreviewRequest) SetBrandingNil(b bool)`

 SetBrandingNil sets the value for Branding to be an explicit nil

### UnsetBranding
`func (o *InvoicePreviewRequest) UnsetBranding()`

UnsetBranding ensures that no value is present for Branding, not even an explicit nil
### GetTemplateId

`func (o *InvoicePreviewRequest) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *InvoicePreviewRequest) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *InvoicePreviewRequest) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.

### HasTemplateId

`func (o *InvoicePreviewRequest) HasTemplateId() bool`

HasTemplateId returns a boolean if a field has been set.

### GetPageSize

`func (o *InvoicePreviewRequest) GetPageSize() string`

GetPageSize returns the PageSize field if non-nil, zero value otherwise.

### GetPageSizeOk

`func (o *InvoicePreviewRequest) GetPageSizeOk() (*string, bool)`

GetPageSizeOk returns a tuple with the PageSize field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPageSize

`func (o *InvoicePreviewRequest) SetPageSize(v string)`

SetPageSize sets PageSize field to given value.

### HasPageSize

`func (o *InvoicePreviewRequest) HasPageSize() bool`

HasPageSize returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


