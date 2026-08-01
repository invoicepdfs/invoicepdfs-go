# CreditNoteCreateRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**InvoiceId** | **string** |  | 
**CreditNoteNumber** | **string** |  | 
**IssueDate** | **string** |  | 
**Reason** | Pointer to **NullableString** |  | [optional] 
**LineItems** | [**[]CreditNoteLineItemInput**](CreditNoteLineItemInput.md) |  | 

## Methods

### NewCreditNoteCreateRequest

`func NewCreditNoteCreateRequest(invoiceId string, creditNoteNumber string, issueDate string, lineItems []CreditNoteLineItemInput, ) *CreditNoteCreateRequest`

NewCreditNoteCreateRequest instantiates a new CreditNoteCreateRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreditNoteCreateRequestWithDefaults

`func NewCreditNoteCreateRequestWithDefaults() *CreditNoteCreateRequest`

NewCreditNoteCreateRequestWithDefaults instantiates a new CreditNoteCreateRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetInvoiceId

`func (o *CreditNoteCreateRequest) GetInvoiceId() string`

GetInvoiceId returns the InvoiceId field if non-nil, zero value otherwise.

### GetInvoiceIdOk

`func (o *CreditNoteCreateRequest) GetInvoiceIdOk() (*string, bool)`

GetInvoiceIdOk returns a tuple with the InvoiceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInvoiceId

`func (o *CreditNoteCreateRequest) SetInvoiceId(v string)`

SetInvoiceId sets InvoiceId field to given value.


### GetCreditNoteNumber

`func (o *CreditNoteCreateRequest) GetCreditNoteNumber() string`

GetCreditNoteNumber returns the CreditNoteNumber field if non-nil, zero value otherwise.

### GetCreditNoteNumberOk

`func (o *CreditNoteCreateRequest) GetCreditNoteNumberOk() (*string, bool)`

GetCreditNoteNumberOk returns a tuple with the CreditNoteNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreditNoteNumber

`func (o *CreditNoteCreateRequest) SetCreditNoteNumber(v string)`

SetCreditNoteNumber sets CreditNoteNumber field to given value.


### GetIssueDate

`func (o *CreditNoteCreateRequest) GetIssueDate() string`

GetIssueDate returns the IssueDate field if non-nil, zero value otherwise.

### GetIssueDateOk

`func (o *CreditNoteCreateRequest) GetIssueDateOk() (*string, bool)`

GetIssueDateOk returns a tuple with the IssueDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIssueDate

`func (o *CreditNoteCreateRequest) SetIssueDate(v string)`

SetIssueDate sets IssueDate field to given value.


### GetReason

`func (o *CreditNoteCreateRequest) GetReason() string`

GetReason returns the Reason field if non-nil, zero value otherwise.

### GetReasonOk

`func (o *CreditNoteCreateRequest) GetReasonOk() (*string, bool)`

GetReasonOk returns a tuple with the Reason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReason

`func (o *CreditNoteCreateRequest) SetReason(v string)`

SetReason sets Reason field to given value.

### HasReason

`func (o *CreditNoteCreateRequest) HasReason() bool`

HasReason returns a boolean if a field has been set.

### SetReasonNil

`func (o *CreditNoteCreateRequest) SetReasonNil(b bool)`

 SetReasonNil sets the value for Reason to be an explicit nil

### UnsetReason
`func (o *CreditNoteCreateRequest) UnsetReason()`

UnsetReason ensures that no value is present for Reason, not even an explicit nil
### GetLineItems

`func (o *CreditNoteCreateRequest) GetLineItems() []CreditNoteLineItemInput`

GetLineItems returns the LineItems field if non-nil, zero value otherwise.

### GetLineItemsOk

`func (o *CreditNoteCreateRequest) GetLineItemsOk() (*[]CreditNoteLineItemInput, bool)`

GetLineItemsOk returns a tuple with the LineItems field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLineItems

`func (o *CreditNoteCreateRequest) SetLineItems(v []CreditNoteLineItemInput)`

SetLineItems sets LineItems field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


