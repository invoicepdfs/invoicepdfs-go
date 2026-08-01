# InvoiceOut

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Status** | **string** |  | 
**InvoiceNumber** | **string** |  | 
**DocumentType** | **string** |  | 
**IssueDate** | **string** |  | 
**DueDate** | Pointer to **NullableString** |  | [optional] 
**Currency** | **string** |  | 
**Locale** | Pointer to **NullableString** |  | [optional] 
**BusinessProfileId** | **string** |  | 
**CustomerId** | **string** |  | 
**Invoice** | **map[string]interface{}** |  | 
**Totals** | [**InvoiceTotalsOut**](InvoiceTotalsOut.md) |  | 
**CreatedAt** | **string** |  | 
**UpdatedAt** | **string** |  | 
**FinalizedAt** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewInvoiceOut

`func NewInvoiceOut(id string, status string, invoiceNumber string, documentType string, issueDate string, currency string, businessProfileId string, customerId string, invoice map[string]interface{}, totals InvoiceTotalsOut, createdAt string, updatedAt string, ) *InvoiceOut`

NewInvoiceOut instantiates a new InvoiceOut object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewInvoiceOutWithDefaults

`func NewInvoiceOutWithDefaults() *InvoiceOut`

NewInvoiceOutWithDefaults instantiates a new InvoiceOut object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *InvoiceOut) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *InvoiceOut) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *InvoiceOut) SetId(v string)`

SetId sets Id field to given value.


### GetStatus

`func (o *InvoiceOut) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *InvoiceOut) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *InvoiceOut) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetInvoiceNumber

`func (o *InvoiceOut) GetInvoiceNumber() string`

GetInvoiceNumber returns the InvoiceNumber field if non-nil, zero value otherwise.

### GetInvoiceNumberOk

`func (o *InvoiceOut) GetInvoiceNumberOk() (*string, bool)`

GetInvoiceNumberOk returns a tuple with the InvoiceNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInvoiceNumber

`func (o *InvoiceOut) SetInvoiceNumber(v string)`

SetInvoiceNumber sets InvoiceNumber field to given value.


### GetDocumentType

`func (o *InvoiceOut) GetDocumentType() string`

GetDocumentType returns the DocumentType field if non-nil, zero value otherwise.

### GetDocumentTypeOk

`func (o *InvoiceOut) GetDocumentTypeOk() (*string, bool)`

GetDocumentTypeOk returns a tuple with the DocumentType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDocumentType

`func (o *InvoiceOut) SetDocumentType(v string)`

SetDocumentType sets DocumentType field to given value.


### GetIssueDate

`func (o *InvoiceOut) GetIssueDate() string`

GetIssueDate returns the IssueDate field if non-nil, zero value otherwise.

### GetIssueDateOk

`func (o *InvoiceOut) GetIssueDateOk() (*string, bool)`

GetIssueDateOk returns a tuple with the IssueDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIssueDate

`func (o *InvoiceOut) SetIssueDate(v string)`

SetIssueDate sets IssueDate field to given value.


### GetDueDate

`func (o *InvoiceOut) GetDueDate() string`

GetDueDate returns the DueDate field if non-nil, zero value otherwise.

### GetDueDateOk

`func (o *InvoiceOut) GetDueDateOk() (*string, bool)`

GetDueDateOk returns a tuple with the DueDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDueDate

`func (o *InvoiceOut) SetDueDate(v string)`

SetDueDate sets DueDate field to given value.

### HasDueDate

`func (o *InvoiceOut) HasDueDate() bool`

HasDueDate returns a boolean if a field has been set.

### SetDueDateNil

`func (o *InvoiceOut) SetDueDateNil(b bool)`

 SetDueDateNil sets the value for DueDate to be an explicit nil

### UnsetDueDate
`func (o *InvoiceOut) UnsetDueDate()`

UnsetDueDate ensures that no value is present for DueDate, not even an explicit nil
### GetCurrency

`func (o *InvoiceOut) GetCurrency() string`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *InvoiceOut) GetCurrencyOk() (*string, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *InvoiceOut) SetCurrency(v string)`

SetCurrency sets Currency field to given value.


### GetLocale

`func (o *InvoiceOut) GetLocale() string`

GetLocale returns the Locale field if non-nil, zero value otherwise.

### GetLocaleOk

`func (o *InvoiceOut) GetLocaleOk() (*string, bool)`

GetLocaleOk returns a tuple with the Locale field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLocale

`func (o *InvoiceOut) SetLocale(v string)`

SetLocale sets Locale field to given value.

### HasLocale

`func (o *InvoiceOut) HasLocale() bool`

HasLocale returns a boolean if a field has been set.

### SetLocaleNil

`func (o *InvoiceOut) SetLocaleNil(b bool)`

 SetLocaleNil sets the value for Locale to be an explicit nil

### UnsetLocale
`func (o *InvoiceOut) UnsetLocale()`

UnsetLocale ensures that no value is present for Locale, not even an explicit nil
### GetBusinessProfileId

`func (o *InvoiceOut) GetBusinessProfileId() string`

GetBusinessProfileId returns the BusinessProfileId field if non-nil, zero value otherwise.

### GetBusinessProfileIdOk

`func (o *InvoiceOut) GetBusinessProfileIdOk() (*string, bool)`

GetBusinessProfileIdOk returns a tuple with the BusinessProfileId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBusinessProfileId

`func (o *InvoiceOut) SetBusinessProfileId(v string)`

SetBusinessProfileId sets BusinessProfileId field to given value.


### GetCustomerId

`func (o *InvoiceOut) GetCustomerId() string`

GetCustomerId returns the CustomerId field if non-nil, zero value otherwise.

### GetCustomerIdOk

`func (o *InvoiceOut) GetCustomerIdOk() (*string, bool)`

GetCustomerIdOk returns a tuple with the CustomerId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomerId

`func (o *InvoiceOut) SetCustomerId(v string)`

SetCustomerId sets CustomerId field to given value.


### GetInvoice

`func (o *InvoiceOut) GetInvoice() map[string]interface{}`

GetInvoice returns the Invoice field if non-nil, zero value otherwise.

### GetInvoiceOk

`func (o *InvoiceOut) GetInvoiceOk() (*map[string]interface{}, bool)`

GetInvoiceOk returns a tuple with the Invoice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInvoice

`func (o *InvoiceOut) SetInvoice(v map[string]interface{})`

SetInvoice sets Invoice field to given value.


### GetTotals

`func (o *InvoiceOut) GetTotals() InvoiceTotalsOut`

GetTotals returns the Totals field if non-nil, zero value otherwise.

### GetTotalsOk

`func (o *InvoiceOut) GetTotalsOk() (*InvoiceTotalsOut, bool)`

GetTotalsOk returns a tuple with the Totals field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotals

`func (o *InvoiceOut) SetTotals(v InvoiceTotalsOut)`

SetTotals sets Totals field to given value.


### GetCreatedAt

`func (o *InvoiceOut) GetCreatedAt() string`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *InvoiceOut) GetCreatedAtOk() (*string, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *InvoiceOut) SetCreatedAt(v string)`

SetCreatedAt sets CreatedAt field to given value.


### GetUpdatedAt

`func (o *InvoiceOut) GetUpdatedAt() string`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *InvoiceOut) GetUpdatedAtOk() (*string, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *InvoiceOut) SetUpdatedAt(v string)`

SetUpdatedAt sets UpdatedAt field to given value.


### GetFinalizedAt

`func (o *InvoiceOut) GetFinalizedAt() string`

GetFinalizedAt returns the FinalizedAt field if non-nil, zero value otherwise.

### GetFinalizedAtOk

`func (o *InvoiceOut) GetFinalizedAtOk() (*string, bool)`

GetFinalizedAtOk returns a tuple with the FinalizedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFinalizedAt

`func (o *InvoiceOut) SetFinalizedAt(v string)`

SetFinalizedAt sets FinalizedAt field to given value.

### HasFinalizedAt

`func (o *InvoiceOut) HasFinalizedAt() bool`

HasFinalizedAt returns a boolean if a field has been set.

### SetFinalizedAtNil

`func (o *InvoiceOut) SetFinalizedAtNil(b bool)`

 SetFinalizedAtNil sets the value for FinalizedAt to be an explicit nil

### UnsetFinalizedAt
`func (o *InvoiceOut) UnsetFinalizedAt()`

UnsetFinalizedAt ensures that no value is present for FinalizedAt, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


