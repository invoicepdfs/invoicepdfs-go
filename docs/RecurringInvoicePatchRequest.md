# RecurringInvoicePatchRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Frequency** | Pointer to **string** |  | [optional] 
**Interval** | Pointer to **int32** |  | [optional] 
**EndDate** | Pointer to **NullableString** |  | [optional] 
**MaxOccurrences** | Pointer to **NullableInt32** |  | [optional] 
**NumberingSequenceId** | Pointer to **NullableString** |  | [optional] 
**AutoFinalize** | Pointer to **bool** |  | [optional] 
**InvoiceTemplate** | Pointer to [**InvoiceDraftRequest**](InvoiceDraftRequest.md) |  | [optional] 

## Methods

### NewRecurringInvoicePatchRequest

`func NewRecurringInvoicePatchRequest() *RecurringInvoicePatchRequest`

NewRecurringInvoicePatchRequest instantiates a new RecurringInvoicePatchRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRecurringInvoicePatchRequestWithDefaults

`func NewRecurringInvoicePatchRequestWithDefaults() *RecurringInvoicePatchRequest`

NewRecurringInvoicePatchRequestWithDefaults instantiates a new RecurringInvoicePatchRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetFrequency

`func (o *RecurringInvoicePatchRequest) GetFrequency() string`

GetFrequency returns the Frequency field if non-nil, zero value otherwise.

### GetFrequencyOk

`func (o *RecurringInvoicePatchRequest) GetFrequencyOk() (*string, bool)`

GetFrequencyOk returns a tuple with the Frequency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrequency

`func (o *RecurringInvoicePatchRequest) SetFrequency(v string)`

SetFrequency sets Frequency field to given value.

### HasFrequency

`func (o *RecurringInvoicePatchRequest) HasFrequency() bool`

HasFrequency returns a boolean if a field has been set.

### GetInterval

`func (o *RecurringInvoicePatchRequest) GetInterval() int32`

GetInterval returns the Interval field if non-nil, zero value otherwise.

### GetIntervalOk

`func (o *RecurringInvoicePatchRequest) GetIntervalOk() (*int32, bool)`

GetIntervalOk returns a tuple with the Interval field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInterval

`func (o *RecurringInvoicePatchRequest) SetInterval(v int32)`

SetInterval sets Interval field to given value.

### HasInterval

`func (o *RecurringInvoicePatchRequest) HasInterval() bool`

HasInterval returns a boolean if a field has been set.

### GetEndDate

`func (o *RecurringInvoicePatchRequest) GetEndDate() string`

GetEndDate returns the EndDate field if non-nil, zero value otherwise.

### GetEndDateOk

`func (o *RecurringInvoicePatchRequest) GetEndDateOk() (*string, bool)`

GetEndDateOk returns a tuple with the EndDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndDate

`func (o *RecurringInvoicePatchRequest) SetEndDate(v string)`

SetEndDate sets EndDate field to given value.

### HasEndDate

`func (o *RecurringInvoicePatchRequest) HasEndDate() bool`

HasEndDate returns a boolean if a field has been set.

### SetEndDateNil

`func (o *RecurringInvoicePatchRequest) SetEndDateNil(b bool)`

 SetEndDateNil sets the value for EndDate to be an explicit nil

### UnsetEndDate
`func (o *RecurringInvoicePatchRequest) UnsetEndDate()`

UnsetEndDate ensures that no value is present for EndDate, not even an explicit nil
### GetMaxOccurrences

`func (o *RecurringInvoicePatchRequest) GetMaxOccurrences() int32`

GetMaxOccurrences returns the MaxOccurrences field if non-nil, zero value otherwise.

### GetMaxOccurrencesOk

`func (o *RecurringInvoicePatchRequest) GetMaxOccurrencesOk() (*int32, bool)`

GetMaxOccurrencesOk returns a tuple with the MaxOccurrences field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxOccurrences

`func (o *RecurringInvoicePatchRequest) SetMaxOccurrences(v int32)`

SetMaxOccurrences sets MaxOccurrences field to given value.

### HasMaxOccurrences

`func (o *RecurringInvoicePatchRequest) HasMaxOccurrences() bool`

HasMaxOccurrences returns a boolean if a field has been set.

### SetMaxOccurrencesNil

`func (o *RecurringInvoicePatchRequest) SetMaxOccurrencesNil(b bool)`

 SetMaxOccurrencesNil sets the value for MaxOccurrences to be an explicit nil

### UnsetMaxOccurrences
`func (o *RecurringInvoicePatchRequest) UnsetMaxOccurrences()`

UnsetMaxOccurrences ensures that no value is present for MaxOccurrences, not even an explicit nil
### GetNumberingSequenceId

`func (o *RecurringInvoicePatchRequest) GetNumberingSequenceId() string`

GetNumberingSequenceId returns the NumberingSequenceId field if non-nil, zero value otherwise.

### GetNumberingSequenceIdOk

`func (o *RecurringInvoicePatchRequest) GetNumberingSequenceIdOk() (*string, bool)`

GetNumberingSequenceIdOk returns a tuple with the NumberingSequenceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNumberingSequenceId

`func (o *RecurringInvoicePatchRequest) SetNumberingSequenceId(v string)`

SetNumberingSequenceId sets NumberingSequenceId field to given value.

### HasNumberingSequenceId

`func (o *RecurringInvoicePatchRequest) HasNumberingSequenceId() bool`

HasNumberingSequenceId returns a boolean if a field has been set.

### SetNumberingSequenceIdNil

`func (o *RecurringInvoicePatchRequest) SetNumberingSequenceIdNil(b bool)`

 SetNumberingSequenceIdNil sets the value for NumberingSequenceId to be an explicit nil

### UnsetNumberingSequenceId
`func (o *RecurringInvoicePatchRequest) UnsetNumberingSequenceId()`

UnsetNumberingSequenceId ensures that no value is present for NumberingSequenceId, not even an explicit nil
### GetAutoFinalize

`func (o *RecurringInvoicePatchRequest) GetAutoFinalize() bool`

GetAutoFinalize returns the AutoFinalize field if non-nil, zero value otherwise.

### GetAutoFinalizeOk

`func (o *RecurringInvoicePatchRequest) GetAutoFinalizeOk() (*bool, bool)`

GetAutoFinalizeOk returns a tuple with the AutoFinalize field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAutoFinalize

`func (o *RecurringInvoicePatchRequest) SetAutoFinalize(v bool)`

SetAutoFinalize sets AutoFinalize field to given value.

### HasAutoFinalize

`func (o *RecurringInvoicePatchRequest) HasAutoFinalize() bool`

HasAutoFinalize returns a boolean if a field has been set.

### GetInvoiceTemplate

`func (o *RecurringInvoicePatchRequest) GetInvoiceTemplate() InvoiceDraftRequest`

GetInvoiceTemplate returns the InvoiceTemplate field if non-nil, zero value otherwise.

### GetInvoiceTemplateOk

`func (o *RecurringInvoicePatchRequest) GetInvoiceTemplateOk() (*InvoiceDraftRequest, bool)`

GetInvoiceTemplateOk returns a tuple with the InvoiceTemplate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInvoiceTemplate

`func (o *RecurringInvoicePatchRequest) SetInvoiceTemplate(v InvoiceDraftRequest)`

SetInvoiceTemplate sets InvoiceTemplate field to given value.

### HasInvoiceTemplate

`func (o *RecurringInvoicePatchRequest) HasInvoiceTemplate() bool`

HasInvoiceTemplate returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


