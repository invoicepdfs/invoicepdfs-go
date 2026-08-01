# RecurringInvoiceOut

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Status** | **string** |  | 
**BusinessProfileId** | **string** |  | 
**CustomerId** | **string** |  | 
**Frequency** | **string** |  | 
**Interval** | **int32** |  | 
**NextOccurrenceDate** | **NullableString** |  | 
**EndDate** | **NullableString** |  | 
**OccurrencesCreated** | **int32** |  | 
**MaxOccurrences** | **NullableInt32** |  | 
**NumberingSequenceId** | **NullableString** |  | 
**AutoFinalize** | **bool** |  | 
**CreatedAt** | **string** |  | 
**UpdatedAt** | **string** |  | 

## Methods

### NewRecurringInvoiceOut

`func NewRecurringInvoiceOut(id string, status string, businessProfileId string, customerId string, frequency string, interval int32, nextOccurrenceDate NullableString, endDate NullableString, occurrencesCreated int32, maxOccurrences NullableInt32, numberingSequenceId NullableString, autoFinalize bool, createdAt string, updatedAt string, ) *RecurringInvoiceOut`

NewRecurringInvoiceOut instantiates a new RecurringInvoiceOut object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRecurringInvoiceOutWithDefaults

`func NewRecurringInvoiceOutWithDefaults() *RecurringInvoiceOut`

NewRecurringInvoiceOutWithDefaults instantiates a new RecurringInvoiceOut object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *RecurringInvoiceOut) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *RecurringInvoiceOut) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *RecurringInvoiceOut) SetId(v string)`

SetId sets Id field to given value.


### GetStatus

`func (o *RecurringInvoiceOut) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *RecurringInvoiceOut) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *RecurringInvoiceOut) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetBusinessProfileId

`func (o *RecurringInvoiceOut) GetBusinessProfileId() string`

GetBusinessProfileId returns the BusinessProfileId field if non-nil, zero value otherwise.

### GetBusinessProfileIdOk

`func (o *RecurringInvoiceOut) GetBusinessProfileIdOk() (*string, bool)`

GetBusinessProfileIdOk returns a tuple with the BusinessProfileId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBusinessProfileId

`func (o *RecurringInvoiceOut) SetBusinessProfileId(v string)`

SetBusinessProfileId sets BusinessProfileId field to given value.


### GetCustomerId

`func (o *RecurringInvoiceOut) GetCustomerId() string`

GetCustomerId returns the CustomerId field if non-nil, zero value otherwise.

### GetCustomerIdOk

`func (o *RecurringInvoiceOut) GetCustomerIdOk() (*string, bool)`

GetCustomerIdOk returns a tuple with the CustomerId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomerId

`func (o *RecurringInvoiceOut) SetCustomerId(v string)`

SetCustomerId sets CustomerId field to given value.


### GetFrequency

`func (o *RecurringInvoiceOut) GetFrequency() string`

GetFrequency returns the Frequency field if non-nil, zero value otherwise.

### GetFrequencyOk

`func (o *RecurringInvoiceOut) GetFrequencyOk() (*string, bool)`

GetFrequencyOk returns a tuple with the Frequency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrequency

`func (o *RecurringInvoiceOut) SetFrequency(v string)`

SetFrequency sets Frequency field to given value.


### GetInterval

`func (o *RecurringInvoiceOut) GetInterval() int32`

GetInterval returns the Interval field if non-nil, zero value otherwise.

### GetIntervalOk

`func (o *RecurringInvoiceOut) GetIntervalOk() (*int32, bool)`

GetIntervalOk returns a tuple with the Interval field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInterval

`func (o *RecurringInvoiceOut) SetInterval(v int32)`

SetInterval sets Interval field to given value.


### GetNextOccurrenceDate

`func (o *RecurringInvoiceOut) GetNextOccurrenceDate() string`

GetNextOccurrenceDate returns the NextOccurrenceDate field if non-nil, zero value otherwise.

### GetNextOccurrenceDateOk

`func (o *RecurringInvoiceOut) GetNextOccurrenceDateOk() (*string, bool)`

GetNextOccurrenceDateOk returns a tuple with the NextOccurrenceDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextOccurrenceDate

`func (o *RecurringInvoiceOut) SetNextOccurrenceDate(v string)`

SetNextOccurrenceDate sets NextOccurrenceDate field to given value.


### SetNextOccurrenceDateNil

`func (o *RecurringInvoiceOut) SetNextOccurrenceDateNil(b bool)`

 SetNextOccurrenceDateNil sets the value for NextOccurrenceDate to be an explicit nil

### UnsetNextOccurrenceDate
`func (o *RecurringInvoiceOut) UnsetNextOccurrenceDate()`

UnsetNextOccurrenceDate ensures that no value is present for NextOccurrenceDate, not even an explicit nil
### GetEndDate

`func (o *RecurringInvoiceOut) GetEndDate() string`

GetEndDate returns the EndDate field if non-nil, zero value otherwise.

### GetEndDateOk

`func (o *RecurringInvoiceOut) GetEndDateOk() (*string, bool)`

GetEndDateOk returns a tuple with the EndDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndDate

`func (o *RecurringInvoiceOut) SetEndDate(v string)`

SetEndDate sets EndDate field to given value.


### SetEndDateNil

`func (o *RecurringInvoiceOut) SetEndDateNil(b bool)`

 SetEndDateNil sets the value for EndDate to be an explicit nil

### UnsetEndDate
`func (o *RecurringInvoiceOut) UnsetEndDate()`

UnsetEndDate ensures that no value is present for EndDate, not even an explicit nil
### GetOccurrencesCreated

`func (o *RecurringInvoiceOut) GetOccurrencesCreated() int32`

GetOccurrencesCreated returns the OccurrencesCreated field if non-nil, zero value otherwise.

### GetOccurrencesCreatedOk

`func (o *RecurringInvoiceOut) GetOccurrencesCreatedOk() (*int32, bool)`

GetOccurrencesCreatedOk returns a tuple with the OccurrencesCreated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOccurrencesCreated

`func (o *RecurringInvoiceOut) SetOccurrencesCreated(v int32)`

SetOccurrencesCreated sets OccurrencesCreated field to given value.


### GetMaxOccurrences

`func (o *RecurringInvoiceOut) GetMaxOccurrences() int32`

GetMaxOccurrences returns the MaxOccurrences field if non-nil, zero value otherwise.

### GetMaxOccurrencesOk

`func (o *RecurringInvoiceOut) GetMaxOccurrencesOk() (*int32, bool)`

GetMaxOccurrencesOk returns a tuple with the MaxOccurrences field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxOccurrences

`func (o *RecurringInvoiceOut) SetMaxOccurrences(v int32)`

SetMaxOccurrences sets MaxOccurrences field to given value.


### SetMaxOccurrencesNil

`func (o *RecurringInvoiceOut) SetMaxOccurrencesNil(b bool)`

 SetMaxOccurrencesNil sets the value for MaxOccurrences to be an explicit nil

### UnsetMaxOccurrences
`func (o *RecurringInvoiceOut) UnsetMaxOccurrences()`

UnsetMaxOccurrences ensures that no value is present for MaxOccurrences, not even an explicit nil
### GetNumberingSequenceId

`func (o *RecurringInvoiceOut) GetNumberingSequenceId() string`

GetNumberingSequenceId returns the NumberingSequenceId field if non-nil, zero value otherwise.

### GetNumberingSequenceIdOk

`func (o *RecurringInvoiceOut) GetNumberingSequenceIdOk() (*string, bool)`

GetNumberingSequenceIdOk returns a tuple with the NumberingSequenceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNumberingSequenceId

`func (o *RecurringInvoiceOut) SetNumberingSequenceId(v string)`

SetNumberingSequenceId sets NumberingSequenceId field to given value.


### SetNumberingSequenceIdNil

`func (o *RecurringInvoiceOut) SetNumberingSequenceIdNil(b bool)`

 SetNumberingSequenceIdNil sets the value for NumberingSequenceId to be an explicit nil

### UnsetNumberingSequenceId
`func (o *RecurringInvoiceOut) UnsetNumberingSequenceId()`

UnsetNumberingSequenceId ensures that no value is present for NumberingSequenceId, not even an explicit nil
### GetAutoFinalize

`func (o *RecurringInvoiceOut) GetAutoFinalize() bool`

GetAutoFinalize returns the AutoFinalize field if non-nil, zero value otherwise.

### GetAutoFinalizeOk

`func (o *RecurringInvoiceOut) GetAutoFinalizeOk() (*bool, bool)`

GetAutoFinalizeOk returns a tuple with the AutoFinalize field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAutoFinalize

`func (o *RecurringInvoiceOut) SetAutoFinalize(v bool)`

SetAutoFinalize sets AutoFinalize field to given value.


### GetCreatedAt

`func (o *RecurringInvoiceOut) GetCreatedAt() string`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *RecurringInvoiceOut) GetCreatedAtOk() (*string, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *RecurringInvoiceOut) SetCreatedAt(v string)`

SetCreatedAt sets CreatedAt field to given value.


### GetUpdatedAt

`func (o *RecurringInvoiceOut) GetUpdatedAt() string`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *RecurringInvoiceOut) GetUpdatedAtOk() (*string, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *RecurringInvoiceOut) SetUpdatedAt(v string)`

SetUpdatedAt sets UpdatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


