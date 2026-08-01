# CreditNoteOut

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**InvoiceId** | **string** |  | 
**CreditNoteNumber** | **string** |  | 
**Status** | **string** |  | 
**Reason** | Pointer to **NullableString** |  | [optional] 
**Currency** | **string** |  | 
**Totals** | [**InvoiceTotalsOut**](InvoiceTotalsOut.md) |  | 
**IssueDate** | **string** |  | 
**CreatedAt** | **string** |  | 
**UpdatedAt** | **string** |  | 
**FinalizedAt** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewCreditNoteOut

`func NewCreditNoteOut(id string, invoiceId string, creditNoteNumber string, status string, currency string, totals InvoiceTotalsOut, issueDate string, createdAt string, updatedAt string, ) *CreditNoteOut`

NewCreditNoteOut instantiates a new CreditNoteOut object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreditNoteOutWithDefaults

`func NewCreditNoteOutWithDefaults() *CreditNoteOut`

NewCreditNoteOutWithDefaults instantiates a new CreditNoteOut object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *CreditNoteOut) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *CreditNoteOut) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *CreditNoteOut) SetId(v string)`

SetId sets Id field to given value.


### GetInvoiceId

`func (o *CreditNoteOut) GetInvoiceId() string`

GetInvoiceId returns the InvoiceId field if non-nil, zero value otherwise.

### GetInvoiceIdOk

`func (o *CreditNoteOut) GetInvoiceIdOk() (*string, bool)`

GetInvoiceIdOk returns a tuple with the InvoiceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInvoiceId

`func (o *CreditNoteOut) SetInvoiceId(v string)`

SetInvoiceId sets InvoiceId field to given value.


### GetCreditNoteNumber

`func (o *CreditNoteOut) GetCreditNoteNumber() string`

GetCreditNoteNumber returns the CreditNoteNumber field if non-nil, zero value otherwise.

### GetCreditNoteNumberOk

`func (o *CreditNoteOut) GetCreditNoteNumberOk() (*string, bool)`

GetCreditNoteNumberOk returns a tuple with the CreditNoteNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreditNoteNumber

`func (o *CreditNoteOut) SetCreditNoteNumber(v string)`

SetCreditNoteNumber sets CreditNoteNumber field to given value.


### GetStatus

`func (o *CreditNoteOut) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *CreditNoteOut) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *CreditNoteOut) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetReason

`func (o *CreditNoteOut) GetReason() string`

GetReason returns the Reason field if non-nil, zero value otherwise.

### GetReasonOk

`func (o *CreditNoteOut) GetReasonOk() (*string, bool)`

GetReasonOk returns a tuple with the Reason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReason

`func (o *CreditNoteOut) SetReason(v string)`

SetReason sets Reason field to given value.

### HasReason

`func (o *CreditNoteOut) HasReason() bool`

HasReason returns a boolean if a field has been set.

### SetReasonNil

`func (o *CreditNoteOut) SetReasonNil(b bool)`

 SetReasonNil sets the value for Reason to be an explicit nil

### UnsetReason
`func (o *CreditNoteOut) UnsetReason()`

UnsetReason ensures that no value is present for Reason, not even an explicit nil
### GetCurrency

`func (o *CreditNoteOut) GetCurrency() string`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *CreditNoteOut) GetCurrencyOk() (*string, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *CreditNoteOut) SetCurrency(v string)`

SetCurrency sets Currency field to given value.


### GetTotals

`func (o *CreditNoteOut) GetTotals() InvoiceTotalsOut`

GetTotals returns the Totals field if non-nil, zero value otherwise.

### GetTotalsOk

`func (o *CreditNoteOut) GetTotalsOk() (*InvoiceTotalsOut, bool)`

GetTotalsOk returns a tuple with the Totals field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotals

`func (o *CreditNoteOut) SetTotals(v InvoiceTotalsOut)`

SetTotals sets Totals field to given value.


### GetIssueDate

`func (o *CreditNoteOut) GetIssueDate() string`

GetIssueDate returns the IssueDate field if non-nil, zero value otherwise.

### GetIssueDateOk

`func (o *CreditNoteOut) GetIssueDateOk() (*string, bool)`

GetIssueDateOk returns a tuple with the IssueDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIssueDate

`func (o *CreditNoteOut) SetIssueDate(v string)`

SetIssueDate sets IssueDate field to given value.


### GetCreatedAt

`func (o *CreditNoteOut) GetCreatedAt() string`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *CreditNoteOut) GetCreatedAtOk() (*string, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *CreditNoteOut) SetCreatedAt(v string)`

SetCreatedAt sets CreatedAt field to given value.


### GetUpdatedAt

`func (o *CreditNoteOut) GetUpdatedAt() string`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *CreditNoteOut) GetUpdatedAtOk() (*string, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *CreditNoteOut) SetUpdatedAt(v string)`

SetUpdatedAt sets UpdatedAt field to given value.


### GetFinalizedAt

`func (o *CreditNoteOut) GetFinalizedAt() string`

GetFinalizedAt returns the FinalizedAt field if non-nil, zero value otherwise.

### GetFinalizedAtOk

`func (o *CreditNoteOut) GetFinalizedAtOk() (*string, bool)`

GetFinalizedAtOk returns a tuple with the FinalizedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFinalizedAt

`func (o *CreditNoteOut) SetFinalizedAt(v string)`

SetFinalizedAt sets FinalizedAt field to given value.

### HasFinalizedAt

`func (o *CreditNoteOut) HasFinalizedAt() bool`

HasFinalizedAt returns a boolean if a field has been set.

### SetFinalizedAtNil

`func (o *CreditNoteOut) SetFinalizedAtNil(b bool)`

 SetFinalizedAtNil sets the value for FinalizedAt to be an explicit nil

### UnsetFinalizedAt
`func (o *CreditNoteOut) UnsetFinalizedAt()`

UnsetFinalizedAt ensures that no value is present for FinalizedAt, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


