# DocumentOut

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**DocumentType** | **string** |  | 
**Number** | **string** |  | 
**Status** | **string** |  | 
**IssueDate** | **string** |  | 
**DueDate** | Pointer to **NullableString** |  | [optional] 
**Currency** | **string** |  | 
**Locale** | Pointer to **NullableString** |  | [optional] 
**BusinessProfileId** | **string** |  | 
**CustomerId** | **string** |  | 
**SourceDocumentId** | Pointer to **NullableString** |  | [optional] 
**Reason** | Pointer to **NullableString** |  | [optional] 
**Data** | **map[string]interface{}** |  | 
**Totals** | [**InvoiceTotalsOut**](InvoiceTotalsOut.md) |  | 
**CreatedAt** | **string** |  | 
**UpdatedAt** | **string** |  | 
**FinalizedAt** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewDocumentOut

`func NewDocumentOut(id string, documentType string, number string, status string, issueDate string, currency string, businessProfileId string, customerId string, data map[string]interface{}, totals InvoiceTotalsOut, createdAt string, updatedAt string, ) *DocumentOut`

NewDocumentOut instantiates a new DocumentOut object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDocumentOutWithDefaults

`func NewDocumentOutWithDefaults() *DocumentOut`

NewDocumentOutWithDefaults instantiates a new DocumentOut object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *DocumentOut) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *DocumentOut) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *DocumentOut) SetId(v string)`

SetId sets Id field to given value.


### GetDocumentType

`func (o *DocumentOut) GetDocumentType() string`

GetDocumentType returns the DocumentType field if non-nil, zero value otherwise.

### GetDocumentTypeOk

`func (o *DocumentOut) GetDocumentTypeOk() (*string, bool)`

GetDocumentTypeOk returns a tuple with the DocumentType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDocumentType

`func (o *DocumentOut) SetDocumentType(v string)`

SetDocumentType sets DocumentType field to given value.


### GetNumber

`func (o *DocumentOut) GetNumber() string`

GetNumber returns the Number field if non-nil, zero value otherwise.

### GetNumberOk

`func (o *DocumentOut) GetNumberOk() (*string, bool)`

GetNumberOk returns a tuple with the Number field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNumber

`func (o *DocumentOut) SetNumber(v string)`

SetNumber sets Number field to given value.


### GetStatus

`func (o *DocumentOut) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *DocumentOut) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *DocumentOut) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetIssueDate

`func (o *DocumentOut) GetIssueDate() string`

GetIssueDate returns the IssueDate field if non-nil, zero value otherwise.

### GetIssueDateOk

`func (o *DocumentOut) GetIssueDateOk() (*string, bool)`

GetIssueDateOk returns a tuple with the IssueDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIssueDate

`func (o *DocumentOut) SetIssueDate(v string)`

SetIssueDate sets IssueDate field to given value.


### GetDueDate

`func (o *DocumentOut) GetDueDate() string`

GetDueDate returns the DueDate field if non-nil, zero value otherwise.

### GetDueDateOk

`func (o *DocumentOut) GetDueDateOk() (*string, bool)`

GetDueDateOk returns a tuple with the DueDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDueDate

`func (o *DocumentOut) SetDueDate(v string)`

SetDueDate sets DueDate field to given value.

### HasDueDate

`func (o *DocumentOut) HasDueDate() bool`

HasDueDate returns a boolean if a field has been set.

### SetDueDateNil

`func (o *DocumentOut) SetDueDateNil(b bool)`

 SetDueDateNil sets the value for DueDate to be an explicit nil

### UnsetDueDate
`func (o *DocumentOut) UnsetDueDate()`

UnsetDueDate ensures that no value is present for DueDate, not even an explicit nil
### GetCurrency

`func (o *DocumentOut) GetCurrency() string`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *DocumentOut) GetCurrencyOk() (*string, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *DocumentOut) SetCurrency(v string)`

SetCurrency sets Currency field to given value.


### GetLocale

`func (o *DocumentOut) GetLocale() string`

GetLocale returns the Locale field if non-nil, zero value otherwise.

### GetLocaleOk

`func (o *DocumentOut) GetLocaleOk() (*string, bool)`

GetLocaleOk returns a tuple with the Locale field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLocale

`func (o *DocumentOut) SetLocale(v string)`

SetLocale sets Locale field to given value.

### HasLocale

`func (o *DocumentOut) HasLocale() bool`

HasLocale returns a boolean if a field has been set.

### SetLocaleNil

`func (o *DocumentOut) SetLocaleNil(b bool)`

 SetLocaleNil sets the value for Locale to be an explicit nil

### UnsetLocale
`func (o *DocumentOut) UnsetLocale()`

UnsetLocale ensures that no value is present for Locale, not even an explicit nil
### GetBusinessProfileId

`func (o *DocumentOut) GetBusinessProfileId() string`

GetBusinessProfileId returns the BusinessProfileId field if non-nil, zero value otherwise.

### GetBusinessProfileIdOk

`func (o *DocumentOut) GetBusinessProfileIdOk() (*string, bool)`

GetBusinessProfileIdOk returns a tuple with the BusinessProfileId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBusinessProfileId

`func (o *DocumentOut) SetBusinessProfileId(v string)`

SetBusinessProfileId sets BusinessProfileId field to given value.


### GetCustomerId

`func (o *DocumentOut) GetCustomerId() string`

GetCustomerId returns the CustomerId field if non-nil, zero value otherwise.

### GetCustomerIdOk

`func (o *DocumentOut) GetCustomerIdOk() (*string, bool)`

GetCustomerIdOk returns a tuple with the CustomerId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomerId

`func (o *DocumentOut) SetCustomerId(v string)`

SetCustomerId sets CustomerId field to given value.


### GetSourceDocumentId

`func (o *DocumentOut) GetSourceDocumentId() string`

GetSourceDocumentId returns the SourceDocumentId field if non-nil, zero value otherwise.

### GetSourceDocumentIdOk

`func (o *DocumentOut) GetSourceDocumentIdOk() (*string, bool)`

GetSourceDocumentIdOk returns a tuple with the SourceDocumentId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceDocumentId

`func (o *DocumentOut) SetSourceDocumentId(v string)`

SetSourceDocumentId sets SourceDocumentId field to given value.

### HasSourceDocumentId

`func (o *DocumentOut) HasSourceDocumentId() bool`

HasSourceDocumentId returns a boolean if a field has been set.

### SetSourceDocumentIdNil

`func (o *DocumentOut) SetSourceDocumentIdNil(b bool)`

 SetSourceDocumentIdNil sets the value for SourceDocumentId to be an explicit nil

### UnsetSourceDocumentId
`func (o *DocumentOut) UnsetSourceDocumentId()`

UnsetSourceDocumentId ensures that no value is present for SourceDocumentId, not even an explicit nil
### GetReason

`func (o *DocumentOut) GetReason() string`

GetReason returns the Reason field if non-nil, zero value otherwise.

### GetReasonOk

`func (o *DocumentOut) GetReasonOk() (*string, bool)`

GetReasonOk returns a tuple with the Reason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReason

`func (o *DocumentOut) SetReason(v string)`

SetReason sets Reason field to given value.

### HasReason

`func (o *DocumentOut) HasReason() bool`

HasReason returns a boolean if a field has been set.

### SetReasonNil

`func (o *DocumentOut) SetReasonNil(b bool)`

 SetReasonNil sets the value for Reason to be an explicit nil

### UnsetReason
`func (o *DocumentOut) UnsetReason()`

UnsetReason ensures that no value is present for Reason, not even an explicit nil
### GetData

`func (o *DocumentOut) GetData() map[string]interface{}`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *DocumentOut) GetDataOk() (*map[string]interface{}, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *DocumentOut) SetData(v map[string]interface{})`

SetData sets Data field to given value.


### GetTotals

`func (o *DocumentOut) GetTotals() InvoiceTotalsOut`

GetTotals returns the Totals field if non-nil, zero value otherwise.

### GetTotalsOk

`func (o *DocumentOut) GetTotalsOk() (*InvoiceTotalsOut, bool)`

GetTotalsOk returns a tuple with the Totals field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotals

`func (o *DocumentOut) SetTotals(v InvoiceTotalsOut)`

SetTotals sets Totals field to given value.


### GetCreatedAt

`func (o *DocumentOut) GetCreatedAt() string`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *DocumentOut) GetCreatedAtOk() (*string, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *DocumentOut) SetCreatedAt(v string)`

SetCreatedAt sets CreatedAt field to given value.


### GetUpdatedAt

`func (o *DocumentOut) GetUpdatedAt() string`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *DocumentOut) GetUpdatedAtOk() (*string, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *DocumentOut) SetUpdatedAt(v string)`

SetUpdatedAt sets UpdatedAt field to given value.


### GetFinalizedAt

`func (o *DocumentOut) GetFinalizedAt() string`

GetFinalizedAt returns the FinalizedAt field if non-nil, zero value otherwise.

### GetFinalizedAtOk

`func (o *DocumentOut) GetFinalizedAtOk() (*string, bool)`

GetFinalizedAtOk returns a tuple with the FinalizedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFinalizedAt

`func (o *DocumentOut) SetFinalizedAt(v string)`

SetFinalizedAt sets FinalizedAt field to given value.

### HasFinalizedAt

`func (o *DocumentOut) HasFinalizedAt() bool`

HasFinalizedAt returns a boolean if a field has been set.

### SetFinalizedAtNil

`func (o *DocumentOut) SetFinalizedAtNil(b bool)`

 SetFinalizedAtNil sets the value for FinalizedAt to be an explicit nil

### UnsetFinalizedAt
`func (o *DocumentOut) UnsetFinalizedAt()`

UnsetFinalizedAt ensures that no value is present for FinalizedAt, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


