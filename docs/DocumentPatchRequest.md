# DocumentPatchRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Number** | Pointer to **NullableString** |  | [optional] 
**DocumentType** | Pointer to **NullableString** |  | [optional] 
**IssueDate** | Pointer to **NullableString** |  | [optional] 
**DueDate** | Pointer to **NullableString** |  | [optional] 
**Currency** | Pointer to **NullableString** |  | [optional] 
**Locale** | Pointer to **NullableString** |  | [optional] 
**BusinessProfileId** | Pointer to **NullableString** |  | [optional] 
**CustomerId** | Pointer to **NullableString** |  | [optional] 
**SourceDocumentId** | Pointer to **NullableString** |  | [optional] 
**Reason** | Pointer to **NullableString** |  | [optional] 
**ShipTo** | Pointer to [**NullablePostalAddress**](PostalAddress.md) |  | [optional] 
**LineItems** | Pointer to [**[]StandardLineItemInput**](StandardLineItemInput.md) |  | [optional] 
**Discounts** | Pointer to [**[]LineItemDiscountInput**](LineItemDiscountInput.md) |  | [optional] 
**Shipping** | Pointer to [**NullableInvoiceShippingInput**](InvoiceShippingInput.md) |  | [optional] 
**Notes** | Pointer to [**[]InvoiceNoteInput**](InvoiceNoteInput.md) |  | [optional] 
**Terms** | Pointer to [**[]InvoiceTermInput**](InvoiceTermInput.md) |  | [optional] 
**CustomFields** | Pointer to [**[]InvoiceCustomFieldInput**](InvoiceCustomFieldInput.md) |  | [optional] 
**Payment** | Pointer to [**NullableInvoicePaymentInput**](InvoicePaymentInput.md) |  | [optional] 
**Branding** | Pointer to [**NullableInvoiceBrandingInput**](InvoiceBrandingInput.md) |  | [optional] 

## Methods

### NewDocumentPatchRequest

`func NewDocumentPatchRequest() *DocumentPatchRequest`

NewDocumentPatchRequest instantiates a new DocumentPatchRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDocumentPatchRequestWithDefaults

`func NewDocumentPatchRequestWithDefaults() *DocumentPatchRequest`

NewDocumentPatchRequestWithDefaults instantiates a new DocumentPatchRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetNumber

`func (o *DocumentPatchRequest) GetNumber() string`

GetNumber returns the Number field if non-nil, zero value otherwise.

### GetNumberOk

`func (o *DocumentPatchRequest) GetNumberOk() (*string, bool)`

GetNumberOk returns a tuple with the Number field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNumber

`func (o *DocumentPatchRequest) SetNumber(v string)`

SetNumber sets Number field to given value.

### HasNumber

`func (o *DocumentPatchRequest) HasNumber() bool`

HasNumber returns a boolean if a field has been set.

### SetNumberNil

`func (o *DocumentPatchRequest) SetNumberNil(b bool)`

 SetNumberNil sets the value for Number to be an explicit nil

### UnsetNumber
`func (o *DocumentPatchRequest) UnsetNumber()`

UnsetNumber ensures that no value is present for Number, not even an explicit nil
### GetDocumentType

`func (o *DocumentPatchRequest) GetDocumentType() string`

GetDocumentType returns the DocumentType field if non-nil, zero value otherwise.

### GetDocumentTypeOk

`func (o *DocumentPatchRequest) GetDocumentTypeOk() (*string, bool)`

GetDocumentTypeOk returns a tuple with the DocumentType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDocumentType

`func (o *DocumentPatchRequest) SetDocumentType(v string)`

SetDocumentType sets DocumentType field to given value.

### HasDocumentType

`func (o *DocumentPatchRequest) HasDocumentType() bool`

HasDocumentType returns a boolean if a field has been set.

### SetDocumentTypeNil

`func (o *DocumentPatchRequest) SetDocumentTypeNil(b bool)`

 SetDocumentTypeNil sets the value for DocumentType to be an explicit nil

### UnsetDocumentType
`func (o *DocumentPatchRequest) UnsetDocumentType()`

UnsetDocumentType ensures that no value is present for DocumentType, not even an explicit nil
### GetIssueDate

`func (o *DocumentPatchRequest) GetIssueDate() string`

GetIssueDate returns the IssueDate field if non-nil, zero value otherwise.

### GetIssueDateOk

`func (o *DocumentPatchRequest) GetIssueDateOk() (*string, bool)`

GetIssueDateOk returns a tuple with the IssueDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIssueDate

`func (o *DocumentPatchRequest) SetIssueDate(v string)`

SetIssueDate sets IssueDate field to given value.

### HasIssueDate

`func (o *DocumentPatchRequest) HasIssueDate() bool`

HasIssueDate returns a boolean if a field has been set.

### SetIssueDateNil

`func (o *DocumentPatchRequest) SetIssueDateNil(b bool)`

 SetIssueDateNil sets the value for IssueDate to be an explicit nil

### UnsetIssueDate
`func (o *DocumentPatchRequest) UnsetIssueDate()`

UnsetIssueDate ensures that no value is present for IssueDate, not even an explicit nil
### GetDueDate

`func (o *DocumentPatchRequest) GetDueDate() string`

GetDueDate returns the DueDate field if non-nil, zero value otherwise.

### GetDueDateOk

`func (o *DocumentPatchRequest) GetDueDateOk() (*string, bool)`

GetDueDateOk returns a tuple with the DueDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDueDate

`func (o *DocumentPatchRequest) SetDueDate(v string)`

SetDueDate sets DueDate field to given value.

### HasDueDate

`func (o *DocumentPatchRequest) HasDueDate() bool`

HasDueDate returns a boolean if a field has been set.

### SetDueDateNil

`func (o *DocumentPatchRequest) SetDueDateNil(b bool)`

 SetDueDateNil sets the value for DueDate to be an explicit nil

### UnsetDueDate
`func (o *DocumentPatchRequest) UnsetDueDate()`

UnsetDueDate ensures that no value is present for DueDate, not even an explicit nil
### GetCurrency

`func (o *DocumentPatchRequest) GetCurrency() string`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *DocumentPatchRequest) GetCurrencyOk() (*string, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *DocumentPatchRequest) SetCurrency(v string)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *DocumentPatchRequest) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.

### SetCurrencyNil

`func (o *DocumentPatchRequest) SetCurrencyNil(b bool)`

 SetCurrencyNil sets the value for Currency to be an explicit nil

### UnsetCurrency
`func (o *DocumentPatchRequest) UnsetCurrency()`

UnsetCurrency ensures that no value is present for Currency, not even an explicit nil
### GetLocale

`func (o *DocumentPatchRequest) GetLocale() string`

GetLocale returns the Locale field if non-nil, zero value otherwise.

### GetLocaleOk

`func (o *DocumentPatchRequest) GetLocaleOk() (*string, bool)`

GetLocaleOk returns a tuple with the Locale field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLocale

`func (o *DocumentPatchRequest) SetLocale(v string)`

SetLocale sets Locale field to given value.

### HasLocale

`func (o *DocumentPatchRequest) HasLocale() bool`

HasLocale returns a boolean if a field has been set.

### SetLocaleNil

`func (o *DocumentPatchRequest) SetLocaleNil(b bool)`

 SetLocaleNil sets the value for Locale to be an explicit nil

### UnsetLocale
`func (o *DocumentPatchRequest) UnsetLocale()`

UnsetLocale ensures that no value is present for Locale, not even an explicit nil
### GetBusinessProfileId

`func (o *DocumentPatchRequest) GetBusinessProfileId() string`

GetBusinessProfileId returns the BusinessProfileId field if non-nil, zero value otherwise.

### GetBusinessProfileIdOk

`func (o *DocumentPatchRequest) GetBusinessProfileIdOk() (*string, bool)`

GetBusinessProfileIdOk returns a tuple with the BusinessProfileId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBusinessProfileId

`func (o *DocumentPatchRequest) SetBusinessProfileId(v string)`

SetBusinessProfileId sets BusinessProfileId field to given value.

### HasBusinessProfileId

`func (o *DocumentPatchRequest) HasBusinessProfileId() bool`

HasBusinessProfileId returns a boolean if a field has been set.

### SetBusinessProfileIdNil

`func (o *DocumentPatchRequest) SetBusinessProfileIdNil(b bool)`

 SetBusinessProfileIdNil sets the value for BusinessProfileId to be an explicit nil

### UnsetBusinessProfileId
`func (o *DocumentPatchRequest) UnsetBusinessProfileId()`

UnsetBusinessProfileId ensures that no value is present for BusinessProfileId, not even an explicit nil
### GetCustomerId

`func (o *DocumentPatchRequest) GetCustomerId() string`

GetCustomerId returns the CustomerId field if non-nil, zero value otherwise.

### GetCustomerIdOk

`func (o *DocumentPatchRequest) GetCustomerIdOk() (*string, bool)`

GetCustomerIdOk returns a tuple with the CustomerId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomerId

`func (o *DocumentPatchRequest) SetCustomerId(v string)`

SetCustomerId sets CustomerId field to given value.

### HasCustomerId

`func (o *DocumentPatchRequest) HasCustomerId() bool`

HasCustomerId returns a boolean if a field has been set.

### SetCustomerIdNil

`func (o *DocumentPatchRequest) SetCustomerIdNil(b bool)`

 SetCustomerIdNil sets the value for CustomerId to be an explicit nil

### UnsetCustomerId
`func (o *DocumentPatchRequest) UnsetCustomerId()`

UnsetCustomerId ensures that no value is present for CustomerId, not even an explicit nil
### GetSourceDocumentId

`func (o *DocumentPatchRequest) GetSourceDocumentId() string`

GetSourceDocumentId returns the SourceDocumentId field if non-nil, zero value otherwise.

### GetSourceDocumentIdOk

`func (o *DocumentPatchRequest) GetSourceDocumentIdOk() (*string, bool)`

GetSourceDocumentIdOk returns a tuple with the SourceDocumentId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceDocumentId

`func (o *DocumentPatchRequest) SetSourceDocumentId(v string)`

SetSourceDocumentId sets SourceDocumentId field to given value.

### HasSourceDocumentId

`func (o *DocumentPatchRequest) HasSourceDocumentId() bool`

HasSourceDocumentId returns a boolean if a field has been set.

### SetSourceDocumentIdNil

`func (o *DocumentPatchRequest) SetSourceDocumentIdNil(b bool)`

 SetSourceDocumentIdNil sets the value for SourceDocumentId to be an explicit nil

### UnsetSourceDocumentId
`func (o *DocumentPatchRequest) UnsetSourceDocumentId()`

UnsetSourceDocumentId ensures that no value is present for SourceDocumentId, not even an explicit nil
### GetReason

`func (o *DocumentPatchRequest) GetReason() string`

GetReason returns the Reason field if non-nil, zero value otherwise.

### GetReasonOk

`func (o *DocumentPatchRequest) GetReasonOk() (*string, bool)`

GetReasonOk returns a tuple with the Reason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReason

`func (o *DocumentPatchRequest) SetReason(v string)`

SetReason sets Reason field to given value.

### HasReason

`func (o *DocumentPatchRequest) HasReason() bool`

HasReason returns a boolean if a field has been set.

### SetReasonNil

`func (o *DocumentPatchRequest) SetReasonNil(b bool)`

 SetReasonNil sets the value for Reason to be an explicit nil

### UnsetReason
`func (o *DocumentPatchRequest) UnsetReason()`

UnsetReason ensures that no value is present for Reason, not even an explicit nil
### GetShipTo

`func (o *DocumentPatchRequest) GetShipTo() PostalAddress`

GetShipTo returns the ShipTo field if non-nil, zero value otherwise.

### GetShipToOk

`func (o *DocumentPatchRequest) GetShipToOk() (*PostalAddress, bool)`

GetShipToOk returns a tuple with the ShipTo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShipTo

`func (o *DocumentPatchRequest) SetShipTo(v PostalAddress)`

SetShipTo sets ShipTo field to given value.

### HasShipTo

`func (o *DocumentPatchRequest) HasShipTo() bool`

HasShipTo returns a boolean if a field has been set.

### SetShipToNil

`func (o *DocumentPatchRequest) SetShipToNil(b bool)`

 SetShipToNil sets the value for ShipTo to be an explicit nil

### UnsetShipTo
`func (o *DocumentPatchRequest) UnsetShipTo()`

UnsetShipTo ensures that no value is present for ShipTo, not even an explicit nil
### GetLineItems

`func (o *DocumentPatchRequest) GetLineItems() []StandardLineItemInput`

GetLineItems returns the LineItems field if non-nil, zero value otherwise.

### GetLineItemsOk

`func (o *DocumentPatchRequest) GetLineItemsOk() (*[]StandardLineItemInput, bool)`

GetLineItemsOk returns a tuple with the LineItems field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLineItems

`func (o *DocumentPatchRequest) SetLineItems(v []StandardLineItemInput)`

SetLineItems sets LineItems field to given value.

### HasLineItems

`func (o *DocumentPatchRequest) HasLineItems() bool`

HasLineItems returns a boolean if a field has been set.

### SetLineItemsNil

`func (o *DocumentPatchRequest) SetLineItemsNil(b bool)`

 SetLineItemsNil sets the value for LineItems to be an explicit nil

### UnsetLineItems
`func (o *DocumentPatchRequest) UnsetLineItems()`

UnsetLineItems ensures that no value is present for LineItems, not even an explicit nil
### GetDiscounts

`func (o *DocumentPatchRequest) GetDiscounts() []LineItemDiscountInput`

GetDiscounts returns the Discounts field if non-nil, zero value otherwise.

### GetDiscountsOk

`func (o *DocumentPatchRequest) GetDiscountsOk() (*[]LineItemDiscountInput, bool)`

GetDiscountsOk returns a tuple with the Discounts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDiscounts

`func (o *DocumentPatchRequest) SetDiscounts(v []LineItemDiscountInput)`

SetDiscounts sets Discounts field to given value.

### HasDiscounts

`func (o *DocumentPatchRequest) HasDiscounts() bool`

HasDiscounts returns a boolean if a field has been set.

### SetDiscountsNil

`func (o *DocumentPatchRequest) SetDiscountsNil(b bool)`

 SetDiscountsNil sets the value for Discounts to be an explicit nil

### UnsetDiscounts
`func (o *DocumentPatchRequest) UnsetDiscounts()`

UnsetDiscounts ensures that no value is present for Discounts, not even an explicit nil
### GetShipping

`func (o *DocumentPatchRequest) GetShipping() InvoiceShippingInput`

GetShipping returns the Shipping field if non-nil, zero value otherwise.

### GetShippingOk

`func (o *DocumentPatchRequest) GetShippingOk() (*InvoiceShippingInput, bool)`

GetShippingOk returns a tuple with the Shipping field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShipping

`func (o *DocumentPatchRequest) SetShipping(v InvoiceShippingInput)`

SetShipping sets Shipping field to given value.

### HasShipping

`func (o *DocumentPatchRequest) HasShipping() bool`

HasShipping returns a boolean if a field has been set.

### SetShippingNil

`func (o *DocumentPatchRequest) SetShippingNil(b bool)`

 SetShippingNil sets the value for Shipping to be an explicit nil

### UnsetShipping
`func (o *DocumentPatchRequest) UnsetShipping()`

UnsetShipping ensures that no value is present for Shipping, not even an explicit nil
### GetNotes

`func (o *DocumentPatchRequest) GetNotes() []InvoiceNoteInput`

GetNotes returns the Notes field if non-nil, zero value otherwise.

### GetNotesOk

`func (o *DocumentPatchRequest) GetNotesOk() (*[]InvoiceNoteInput, bool)`

GetNotesOk returns a tuple with the Notes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNotes

`func (o *DocumentPatchRequest) SetNotes(v []InvoiceNoteInput)`

SetNotes sets Notes field to given value.

### HasNotes

`func (o *DocumentPatchRequest) HasNotes() bool`

HasNotes returns a boolean if a field has been set.

### SetNotesNil

`func (o *DocumentPatchRequest) SetNotesNil(b bool)`

 SetNotesNil sets the value for Notes to be an explicit nil

### UnsetNotes
`func (o *DocumentPatchRequest) UnsetNotes()`

UnsetNotes ensures that no value is present for Notes, not even an explicit nil
### GetTerms

`func (o *DocumentPatchRequest) GetTerms() []InvoiceTermInput`

GetTerms returns the Terms field if non-nil, zero value otherwise.

### GetTermsOk

`func (o *DocumentPatchRequest) GetTermsOk() (*[]InvoiceTermInput, bool)`

GetTermsOk returns a tuple with the Terms field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTerms

`func (o *DocumentPatchRequest) SetTerms(v []InvoiceTermInput)`

SetTerms sets Terms field to given value.

### HasTerms

`func (o *DocumentPatchRequest) HasTerms() bool`

HasTerms returns a boolean if a field has been set.

### SetTermsNil

`func (o *DocumentPatchRequest) SetTermsNil(b bool)`

 SetTermsNil sets the value for Terms to be an explicit nil

### UnsetTerms
`func (o *DocumentPatchRequest) UnsetTerms()`

UnsetTerms ensures that no value is present for Terms, not even an explicit nil
### GetCustomFields

`func (o *DocumentPatchRequest) GetCustomFields() []InvoiceCustomFieldInput`

GetCustomFields returns the CustomFields field if non-nil, zero value otherwise.

### GetCustomFieldsOk

`func (o *DocumentPatchRequest) GetCustomFieldsOk() (*[]InvoiceCustomFieldInput, bool)`

GetCustomFieldsOk returns a tuple with the CustomFields field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomFields

`func (o *DocumentPatchRequest) SetCustomFields(v []InvoiceCustomFieldInput)`

SetCustomFields sets CustomFields field to given value.

### HasCustomFields

`func (o *DocumentPatchRequest) HasCustomFields() bool`

HasCustomFields returns a boolean if a field has been set.

### SetCustomFieldsNil

`func (o *DocumentPatchRequest) SetCustomFieldsNil(b bool)`

 SetCustomFieldsNil sets the value for CustomFields to be an explicit nil

### UnsetCustomFields
`func (o *DocumentPatchRequest) UnsetCustomFields()`

UnsetCustomFields ensures that no value is present for CustomFields, not even an explicit nil
### GetPayment

`func (o *DocumentPatchRequest) GetPayment() InvoicePaymentInput`

GetPayment returns the Payment field if non-nil, zero value otherwise.

### GetPaymentOk

`func (o *DocumentPatchRequest) GetPaymentOk() (*InvoicePaymentInput, bool)`

GetPaymentOk returns a tuple with the Payment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPayment

`func (o *DocumentPatchRequest) SetPayment(v InvoicePaymentInput)`

SetPayment sets Payment field to given value.

### HasPayment

`func (o *DocumentPatchRequest) HasPayment() bool`

HasPayment returns a boolean if a field has been set.

### SetPaymentNil

`func (o *DocumentPatchRequest) SetPaymentNil(b bool)`

 SetPaymentNil sets the value for Payment to be an explicit nil

### UnsetPayment
`func (o *DocumentPatchRequest) UnsetPayment()`

UnsetPayment ensures that no value is present for Payment, not even an explicit nil
### GetBranding

`func (o *DocumentPatchRequest) GetBranding() InvoiceBrandingInput`

GetBranding returns the Branding field if non-nil, zero value otherwise.

### GetBrandingOk

`func (o *DocumentPatchRequest) GetBrandingOk() (*InvoiceBrandingInput, bool)`

GetBrandingOk returns a tuple with the Branding field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBranding

`func (o *DocumentPatchRequest) SetBranding(v InvoiceBrandingInput)`

SetBranding sets Branding field to given value.

### HasBranding

`func (o *DocumentPatchRequest) HasBranding() bool`

HasBranding returns a boolean if a field has been set.

### SetBrandingNil

`func (o *DocumentPatchRequest) SetBrandingNil(b bool)`

 SetBrandingNil sets the value for Branding to be an explicit nil

### UnsetBranding
`func (o *DocumentPatchRequest) UnsetBranding()`

UnsetBranding ensures that no value is present for Branding, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


