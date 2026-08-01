# RecurringInvoiceCreateRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**BusinessProfileId** | **string** |  | 
**CustomerId** | **string** |  | 
**Frequency** | **string** | daily, weekly, monthly, quarterly, or yearly | 
**Interval** | Pointer to **int32** | Every N periods | [optional] [default to 1]
**StartDate** | **string** | Date of the first invoice | 
**EndDate** | Pointer to **NullableString** |  | [optional] 
**MaxOccurrences** | Pointer to **NullableInt32** |  | [optional] 
**NumberingSequenceId** | Pointer to **NullableString** |  | [optional] 
**AutoFinalize** | Pointer to **bool** | Automatically finalize generated invoices | [optional] [default to false]
**InvoiceTemplate** | [**InvoiceDraftRequest**](InvoiceDraftRequest.md) |  | 

## Methods

### NewRecurringInvoiceCreateRequest

`func NewRecurringInvoiceCreateRequest(businessProfileId string, customerId string, frequency string, startDate string, invoiceTemplate InvoiceDraftRequest, ) *RecurringInvoiceCreateRequest`

NewRecurringInvoiceCreateRequest instantiates a new RecurringInvoiceCreateRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRecurringInvoiceCreateRequestWithDefaults

`func NewRecurringInvoiceCreateRequestWithDefaults() *RecurringInvoiceCreateRequest`

NewRecurringInvoiceCreateRequestWithDefaults instantiates a new RecurringInvoiceCreateRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetBusinessProfileId

`func (o *RecurringInvoiceCreateRequest) GetBusinessProfileId() string`

GetBusinessProfileId returns the BusinessProfileId field if non-nil, zero value otherwise.

### GetBusinessProfileIdOk

`func (o *RecurringInvoiceCreateRequest) GetBusinessProfileIdOk() (*string, bool)`

GetBusinessProfileIdOk returns a tuple with the BusinessProfileId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBusinessProfileId

`func (o *RecurringInvoiceCreateRequest) SetBusinessProfileId(v string)`

SetBusinessProfileId sets BusinessProfileId field to given value.


### GetCustomerId

`func (o *RecurringInvoiceCreateRequest) GetCustomerId() string`

GetCustomerId returns the CustomerId field if non-nil, zero value otherwise.

### GetCustomerIdOk

`func (o *RecurringInvoiceCreateRequest) GetCustomerIdOk() (*string, bool)`

GetCustomerIdOk returns a tuple with the CustomerId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomerId

`func (o *RecurringInvoiceCreateRequest) SetCustomerId(v string)`

SetCustomerId sets CustomerId field to given value.


### GetFrequency

`func (o *RecurringInvoiceCreateRequest) GetFrequency() string`

GetFrequency returns the Frequency field if non-nil, zero value otherwise.

### GetFrequencyOk

`func (o *RecurringInvoiceCreateRequest) GetFrequencyOk() (*string, bool)`

GetFrequencyOk returns a tuple with the Frequency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrequency

`func (o *RecurringInvoiceCreateRequest) SetFrequency(v string)`

SetFrequency sets Frequency field to given value.


### GetInterval

`func (o *RecurringInvoiceCreateRequest) GetInterval() int32`

GetInterval returns the Interval field if non-nil, zero value otherwise.

### GetIntervalOk

`func (o *RecurringInvoiceCreateRequest) GetIntervalOk() (*int32, bool)`

GetIntervalOk returns a tuple with the Interval field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInterval

`func (o *RecurringInvoiceCreateRequest) SetInterval(v int32)`

SetInterval sets Interval field to given value.

### HasInterval

`func (o *RecurringInvoiceCreateRequest) HasInterval() bool`

HasInterval returns a boolean if a field has been set.

### GetStartDate

`func (o *RecurringInvoiceCreateRequest) GetStartDate() string`

GetStartDate returns the StartDate field if non-nil, zero value otherwise.

### GetStartDateOk

`func (o *RecurringInvoiceCreateRequest) GetStartDateOk() (*string, bool)`

GetStartDateOk returns a tuple with the StartDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStartDate

`func (o *RecurringInvoiceCreateRequest) SetStartDate(v string)`

SetStartDate sets StartDate field to given value.


### GetEndDate

`func (o *RecurringInvoiceCreateRequest) GetEndDate() string`

GetEndDate returns the EndDate field if non-nil, zero value otherwise.

### GetEndDateOk

`func (o *RecurringInvoiceCreateRequest) GetEndDateOk() (*string, bool)`

GetEndDateOk returns a tuple with the EndDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndDate

`func (o *RecurringInvoiceCreateRequest) SetEndDate(v string)`

SetEndDate sets EndDate field to given value.

### HasEndDate

`func (o *RecurringInvoiceCreateRequest) HasEndDate() bool`

HasEndDate returns a boolean if a field has been set.

### SetEndDateNil

`func (o *RecurringInvoiceCreateRequest) SetEndDateNil(b bool)`

 SetEndDateNil sets the value for EndDate to be an explicit nil

### UnsetEndDate
`func (o *RecurringInvoiceCreateRequest) UnsetEndDate()`

UnsetEndDate ensures that no value is present for EndDate, not even an explicit nil
### GetMaxOccurrences

`func (o *RecurringInvoiceCreateRequest) GetMaxOccurrences() int32`

GetMaxOccurrences returns the MaxOccurrences field if non-nil, zero value otherwise.

### GetMaxOccurrencesOk

`func (o *RecurringInvoiceCreateRequest) GetMaxOccurrencesOk() (*int32, bool)`

GetMaxOccurrencesOk returns a tuple with the MaxOccurrences field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxOccurrences

`func (o *RecurringInvoiceCreateRequest) SetMaxOccurrences(v int32)`

SetMaxOccurrences sets MaxOccurrences field to given value.

### HasMaxOccurrences

`func (o *RecurringInvoiceCreateRequest) HasMaxOccurrences() bool`

HasMaxOccurrences returns a boolean if a field has been set.

### SetMaxOccurrencesNil

`func (o *RecurringInvoiceCreateRequest) SetMaxOccurrencesNil(b bool)`

 SetMaxOccurrencesNil sets the value for MaxOccurrences to be an explicit nil

### UnsetMaxOccurrences
`func (o *RecurringInvoiceCreateRequest) UnsetMaxOccurrences()`

UnsetMaxOccurrences ensures that no value is present for MaxOccurrences, not even an explicit nil
### GetNumberingSequenceId

`func (o *RecurringInvoiceCreateRequest) GetNumberingSequenceId() string`

GetNumberingSequenceId returns the NumberingSequenceId field if non-nil, zero value otherwise.

### GetNumberingSequenceIdOk

`func (o *RecurringInvoiceCreateRequest) GetNumberingSequenceIdOk() (*string, bool)`

GetNumberingSequenceIdOk returns a tuple with the NumberingSequenceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNumberingSequenceId

`func (o *RecurringInvoiceCreateRequest) SetNumberingSequenceId(v string)`

SetNumberingSequenceId sets NumberingSequenceId field to given value.

### HasNumberingSequenceId

`func (o *RecurringInvoiceCreateRequest) HasNumberingSequenceId() bool`

HasNumberingSequenceId returns a boolean if a field has been set.

### SetNumberingSequenceIdNil

`func (o *RecurringInvoiceCreateRequest) SetNumberingSequenceIdNil(b bool)`

 SetNumberingSequenceIdNil sets the value for NumberingSequenceId to be an explicit nil

### UnsetNumberingSequenceId
`func (o *RecurringInvoiceCreateRequest) UnsetNumberingSequenceId()`

UnsetNumberingSequenceId ensures that no value is present for NumberingSequenceId, not even an explicit nil
### GetAutoFinalize

`func (o *RecurringInvoiceCreateRequest) GetAutoFinalize() bool`

GetAutoFinalize returns the AutoFinalize field if non-nil, zero value otherwise.

### GetAutoFinalizeOk

`func (o *RecurringInvoiceCreateRequest) GetAutoFinalizeOk() (*bool, bool)`

GetAutoFinalizeOk returns a tuple with the AutoFinalize field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAutoFinalize

`func (o *RecurringInvoiceCreateRequest) SetAutoFinalize(v bool)`

SetAutoFinalize sets AutoFinalize field to given value.

### HasAutoFinalize

`func (o *RecurringInvoiceCreateRequest) HasAutoFinalize() bool`

HasAutoFinalize returns a boolean if a field has been set.

### GetInvoiceTemplate

`func (o *RecurringInvoiceCreateRequest) GetInvoiceTemplate() InvoiceDraftRequest`

GetInvoiceTemplate returns the InvoiceTemplate field if non-nil, zero value otherwise.

### GetInvoiceTemplateOk

`func (o *RecurringInvoiceCreateRequest) GetInvoiceTemplateOk() (*InvoiceDraftRequest, bool)`

GetInvoiceTemplateOk returns a tuple with the InvoiceTemplate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInvoiceTemplate

`func (o *RecurringInvoiceCreateRequest) SetInvoiceTemplate(v InvoiceDraftRequest)`

SetInvoiceTemplate sets InvoiceTemplate field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


