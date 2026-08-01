# DocumentCreateRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**DocumentType** | Pointer to **string** |  | [optional] [default to "invoice"]
**Number** | **string** |  | 
**IssueDate** | **string** |  | 
**DueDate** | Pointer to **NullableString** |  | [optional] 
**Currency** | **string** |  | 
**Locale** | Pointer to **NullableString** |  | [optional] 
**BusinessProfileId** | **string** |  | 
**CustomerId** | **string** |  | 
**SourceDocumentId** | Pointer to **NullableString** |  | [optional] 
**Reason** | Pointer to **NullableString** |  | [optional] 
**ShipTo** | Pointer to [**NullablePostalAddress**](PostalAddress.md) |  | [optional] 
**LineItems** | [**[]StandardLineItemInput**](StandardLineItemInput.md) |  | 
**Discounts** | Pointer to [**[]LineItemDiscountInput**](LineItemDiscountInput.md) |  | [optional] 
**Shipping** | Pointer to [**NullableInvoiceShippingInput**](InvoiceShippingInput.md) |  | [optional] 
**Notes** | Pointer to [**[]InvoiceNoteInput**](InvoiceNoteInput.md) |  | [optional] 
**Terms** | Pointer to [**[]InvoiceTermInput**](InvoiceTermInput.md) |  | [optional] 
**CustomFields** | Pointer to [**[]InvoiceCustomFieldInput**](InvoiceCustomFieldInput.md) |  | [optional] 
**Payment** | Pointer to [**NullableInvoicePaymentInput**](InvoicePaymentInput.md) |  | [optional] 
**Branding** | Pointer to [**NullableInvoiceBrandingInput**](InvoiceBrandingInput.md) |  | [optional] 

## Methods

### NewDocumentCreateRequest

`func NewDocumentCreateRequest(number string, issueDate string, currency string, businessProfileId string, customerId string, lineItems []StandardLineItemInput, ) *DocumentCreateRequest`

NewDocumentCreateRequest instantiates a new DocumentCreateRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDocumentCreateRequestWithDefaults

`func NewDocumentCreateRequestWithDefaults() *DocumentCreateRequest`

NewDocumentCreateRequestWithDefaults instantiates a new DocumentCreateRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDocumentType

`func (o *DocumentCreateRequest) GetDocumentType() string`

GetDocumentType returns the DocumentType field if non-nil, zero value otherwise.

### GetDocumentTypeOk

`func (o *DocumentCreateRequest) GetDocumentTypeOk() (*string, bool)`

GetDocumentTypeOk returns a tuple with the DocumentType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDocumentType

`func (o *DocumentCreateRequest) SetDocumentType(v string)`

SetDocumentType sets DocumentType field to given value.

### HasDocumentType

`func (o *DocumentCreateRequest) HasDocumentType() bool`

HasDocumentType returns a boolean if a field has been set.

### GetNumber

`func (o *DocumentCreateRequest) GetNumber() string`

GetNumber returns the Number field if non-nil, zero value otherwise.

### GetNumberOk

`func (o *DocumentCreateRequest) GetNumberOk() (*string, bool)`

GetNumberOk returns a tuple with the Number field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNumber

`func (o *DocumentCreateRequest) SetNumber(v string)`

SetNumber sets Number field to given value.


### GetIssueDate

`func (o *DocumentCreateRequest) GetIssueDate() string`

GetIssueDate returns the IssueDate field if non-nil, zero value otherwise.

### GetIssueDateOk

`func (o *DocumentCreateRequest) GetIssueDateOk() (*string, bool)`

GetIssueDateOk returns a tuple with the IssueDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIssueDate

`func (o *DocumentCreateRequest) SetIssueDate(v string)`

SetIssueDate sets IssueDate field to given value.


### GetDueDate

`func (o *DocumentCreateRequest) GetDueDate() string`

GetDueDate returns the DueDate field if non-nil, zero value otherwise.

### GetDueDateOk

`func (o *DocumentCreateRequest) GetDueDateOk() (*string, bool)`

GetDueDateOk returns a tuple with the DueDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDueDate

`func (o *DocumentCreateRequest) SetDueDate(v string)`

SetDueDate sets DueDate field to given value.

### HasDueDate

`func (o *DocumentCreateRequest) HasDueDate() bool`

HasDueDate returns a boolean if a field has been set.

### SetDueDateNil

`func (o *DocumentCreateRequest) SetDueDateNil(b bool)`

 SetDueDateNil sets the value for DueDate to be an explicit nil

### UnsetDueDate
`func (o *DocumentCreateRequest) UnsetDueDate()`

UnsetDueDate ensures that no value is present for DueDate, not even an explicit nil
### GetCurrency

`func (o *DocumentCreateRequest) GetCurrency() string`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *DocumentCreateRequest) GetCurrencyOk() (*string, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *DocumentCreateRequest) SetCurrency(v string)`

SetCurrency sets Currency field to given value.


### GetLocale

`func (o *DocumentCreateRequest) GetLocale() string`

GetLocale returns the Locale field if non-nil, zero value otherwise.

### GetLocaleOk

`func (o *DocumentCreateRequest) GetLocaleOk() (*string, bool)`

GetLocaleOk returns a tuple with the Locale field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLocale

`func (o *DocumentCreateRequest) SetLocale(v string)`

SetLocale sets Locale field to given value.

### HasLocale

`func (o *DocumentCreateRequest) HasLocale() bool`

HasLocale returns a boolean if a field has been set.

### SetLocaleNil

`func (o *DocumentCreateRequest) SetLocaleNil(b bool)`

 SetLocaleNil sets the value for Locale to be an explicit nil

### UnsetLocale
`func (o *DocumentCreateRequest) UnsetLocale()`

UnsetLocale ensures that no value is present for Locale, not even an explicit nil
### GetBusinessProfileId

`func (o *DocumentCreateRequest) GetBusinessProfileId() string`

GetBusinessProfileId returns the BusinessProfileId field if non-nil, zero value otherwise.

### GetBusinessProfileIdOk

`func (o *DocumentCreateRequest) GetBusinessProfileIdOk() (*string, bool)`

GetBusinessProfileIdOk returns a tuple with the BusinessProfileId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBusinessProfileId

`func (o *DocumentCreateRequest) SetBusinessProfileId(v string)`

SetBusinessProfileId sets BusinessProfileId field to given value.


### GetCustomerId

`func (o *DocumentCreateRequest) GetCustomerId() string`

GetCustomerId returns the CustomerId field if non-nil, zero value otherwise.

### GetCustomerIdOk

`func (o *DocumentCreateRequest) GetCustomerIdOk() (*string, bool)`

GetCustomerIdOk returns a tuple with the CustomerId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomerId

`func (o *DocumentCreateRequest) SetCustomerId(v string)`

SetCustomerId sets CustomerId field to given value.


### GetSourceDocumentId

`func (o *DocumentCreateRequest) GetSourceDocumentId() string`

GetSourceDocumentId returns the SourceDocumentId field if non-nil, zero value otherwise.

### GetSourceDocumentIdOk

`func (o *DocumentCreateRequest) GetSourceDocumentIdOk() (*string, bool)`

GetSourceDocumentIdOk returns a tuple with the SourceDocumentId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceDocumentId

`func (o *DocumentCreateRequest) SetSourceDocumentId(v string)`

SetSourceDocumentId sets SourceDocumentId field to given value.

### HasSourceDocumentId

`func (o *DocumentCreateRequest) HasSourceDocumentId() bool`

HasSourceDocumentId returns a boolean if a field has been set.

### SetSourceDocumentIdNil

`func (o *DocumentCreateRequest) SetSourceDocumentIdNil(b bool)`

 SetSourceDocumentIdNil sets the value for SourceDocumentId to be an explicit nil

### UnsetSourceDocumentId
`func (o *DocumentCreateRequest) UnsetSourceDocumentId()`

UnsetSourceDocumentId ensures that no value is present for SourceDocumentId, not even an explicit nil
### GetReason

`func (o *DocumentCreateRequest) GetReason() string`

GetReason returns the Reason field if non-nil, zero value otherwise.

### GetReasonOk

`func (o *DocumentCreateRequest) GetReasonOk() (*string, bool)`

GetReasonOk returns a tuple with the Reason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReason

`func (o *DocumentCreateRequest) SetReason(v string)`

SetReason sets Reason field to given value.

### HasReason

`func (o *DocumentCreateRequest) HasReason() bool`

HasReason returns a boolean if a field has been set.

### SetReasonNil

`func (o *DocumentCreateRequest) SetReasonNil(b bool)`

 SetReasonNil sets the value for Reason to be an explicit nil

### UnsetReason
`func (o *DocumentCreateRequest) UnsetReason()`

UnsetReason ensures that no value is present for Reason, not even an explicit nil
### GetShipTo

`func (o *DocumentCreateRequest) GetShipTo() PostalAddress`

GetShipTo returns the ShipTo field if non-nil, zero value otherwise.

### GetShipToOk

`func (o *DocumentCreateRequest) GetShipToOk() (*PostalAddress, bool)`

GetShipToOk returns a tuple with the ShipTo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShipTo

`func (o *DocumentCreateRequest) SetShipTo(v PostalAddress)`

SetShipTo sets ShipTo field to given value.

### HasShipTo

`func (o *DocumentCreateRequest) HasShipTo() bool`

HasShipTo returns a boolean if a field has been set.

### SetShipToNil

`func (o *DocumentCreateRequest) SetShipToNil(b bool)`

 SetShipToNil sets the value for ShipTo to be an explicit nil

### UnsetShipTo
`func (o *DocumentCreateRequest) UnsetShipTo()`

UnsetShipTo ensures that no value is present for ShipTo, not even an explicit nil
### GetLineItems

`func (o *DocumentCreateRequest) GetLineItems() []StandardLineItemInput`

GetLineItems returns the LineItems field if non-nil, zero value otherwise.

### GetLineItemsOk

`func (o *DocumentCreateRequest) GetLineItemsOk() (*[]StandardLineItemInput, bool)`

GetLineItemsOk returns a tuple with the LineItems field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLineItems

`func (o *DocumentCreateRequest) SetLineItems(v []StandardLineItemInput)`

SetLineItems sets LineItems field to given value.


### GetDiscounts

`func (o *DocumentCreateRequest) GetDiscounts() []LineItemDiscountInput`

GetDiscounts returns the Discounts field if non-nil, zero value otherwise.

### GetDiscountsOk

`func (o *DocumentCreateRequest) GetDiscountsOk() (*[]LineItemDiscountInput, bool)`

GetDiscountsOk returns a tuple with the Discounts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDiscounts

`func (o *DocumentCreateRequest) SetDiscounts(v []LineItemDiscountInput)`

SetDiscounts sets Discounts field to given value.

### HasDiscounts

`func (o *DocumentCreateRequest) HasDiscounts() bool`

HasDiscounts returns a boolean if a field has been set.

### GetShipping

`func (o *DocumentCreateRequest) GetShipping() InvoiceShippingInput`

GetShipping returns the Shipping field if non-nil, zero value otherwise.

### GetShippingOk

`func (o *DocumentCreateRequest) GetShippingOk() (*InvoiceShippingInput, bool)`

GetShippingOk returns a tuple with the Shipping field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShipping

`func (o *DocumentCreateRequest) SetShipping(v InvoiceShippingInput)`

SetShipping sets Shipping field to given value.

### HasShipping

`func (o *DocumentCreateRequest) HasShipping() bool`

HasShipping returns a boolean if a field has been set.

### SetShippingNil

`func (o *DocumentCreateRequest) SetShippingNil(b bool)`

 SetShippingNil sets the value for Shipping to be an explicit nil

### UnsetShipping
`func (o *DocumentCreateRequest) UnsetShipping()`

UnsetShipping ensures that no value is present for Shipping, not even an explicit nil
### GetNotes

`func (o *DocumentCreateRequest) GetNotes() []InvoiceNoteInput`

GetNotes returns the Notes field if non-nil, zero value otherwise.

### GetNotesOk

`func (o *DocumentCreateRequest) GetNotesOk() (*[]InvoiceNoteInput, bool)`

GetNotesOk returns a tuple with the Notes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNotes

`func (o *DocumentCreateRequest) SetNotes(v []InvoiceNoteInput)`

SetNotes sets Notes field to given value.

### HasNotes

`func (o *DocumentCreateRequest) HasNotes() bool`

HasNotes returns a boolean if a field has been set.

### GetTerms

`func (o *DocumentCreateRequest) GetTerms() []InvoiceTermInput`

GetTerms returns the Terms field if non-nil, zero value otherwise.

### GetTermsOk

`func (o *DocumentCreateRequest) GetTermsOk() (*[]InvoiceTermInput, bool)`

GetTermsOk returns a tuple with the Terms field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTerms

`func (o *DocumentCreateRequest) SetTerms(v []InvoiceTermInput)`

SetTerms sets Terms field to given value.

### HasTerms

`func (o *DocumentCreateRequest) HasTerms() bool`

HasTerms returns a boolean if a field has been set.

### GetCustomFields

`func (o *DocumentCreateRequest) GetCustomFields() []InvoiceCustomFieldInput`

GetCustomFields returns the CustomFields field if non-nil, zero value otherwise.

### GetCustomFieldsOk

`func (o *DocumentCreateRequest) GetCustomFieldsOk() (*[]InvoiceCustomFieldInput, bool)`

GetCustomFieldsOk returns a tuple with the CustomFields field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomFields

`func (o *DocumentCreateRequest) SetCustomFields(v []InvoiceCustomFieldInput)`

SetCustomFields sets CustomFields field to given value.

### HasCustomFields

`func (o *DocumentCreateRequest) HasCustomFields() bool`

HasCustomFields returns a boolean if a field has been set.

### GetPayment

`func (o *DocumentCreateRequest) GetPayment() InvoicePaymentInput`

GetPayment returns the Payment field if non-nil, zero value otherwise.

### GetPaymentOk

`func (o *DocumentCreateRequest) GetPaymentOk() (*InvoicePaymentInput, bool)`

GetPaymentOk returns a tuple with the Payment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPayment

`func (o *DocumentCreateRequest) SetPayment(v InvoicePaymentInput)`

SetPayment sets Payment field to given value.

### HasPayment

`func (o *DocumentCreateRequest) HasPayment() bool`

HasPayment returns a boolean if a field has been set.

### SetPaymentNil

`func (o *DocumentCreateRequest) SetPaymentNil(b bool)`

 SetPaymentNil sets the value for Payment to be an explicit nil

### UnsetPayment
`func (o *DocumentCreateRequest) UnsetPayment()`

UnsetPayment ensures that no value is present for Payment, not even an explicit nil
### GetBranding

`func (o *DocumentCreateRequest) GetBranding() InvoiceBrandingInput`

GetBranding returns the Branding field if non-nil, zero value otherwise.

### GetBrandingOk

`func (o *DocumentCreateRequest) GetBrandingOk() (*InvoiceBrandingInput, bool)`

GetBrandingOk returns a tuple with the Branding field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBranding

`func (o *DocumentCreateRequest) SetBranding(v InvoiceBrandingInput)`

SetBranding sets Branding field to given value.

### HasBranding

`func (o *DocumentCreateRequest) HasBranding() bool`

HasBranding returns a boolean if a field has been set.

### SetBrandingNil

`func (o *DocumentCreateRequest) SetBrandingNil(b bool)`

 SetBrandingNil sets the value for Branding to be an explicit nil

### UnsetBranding
`func (o *DocumentCreateRequest) UnsetBranding()`

UnsetBranding ensures that no value is present for Branding, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


