# InvoiceLineItemTaxInput

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TaxRateId** | Pointer to **NullableString** |  | [optional] 
**Name** | Pointer to **NullableString** |  | [optional] 
**Rate** | Pointer to **NullableString** |  | [optional] 
**Inclusive** | Pointer to **bool** |  | [optional] [default to false]

## Methods

### NewInvoiceLineItemTaxInput

`func NewInvoiceLineItemTaxInput() *InvoiceLineItemTaxInput`

NewInvoiceLineItemTaxInput instantiates a new InvoiceLineItemTaxInput object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewInvoiceLineItemTaxInputWithDefaults

`func NewInvoiceLineItemTaxInputWithDefaults() *InvoiceLineItemTaxInput`

NewInvoiceLineItemTaxInputWithDefaults instantiates a new InvoiceLineItemTaxInput object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTaxRateId

`func (o *InvoiceLineItemTaxInput) GetTaxRateId() string`

GetTaxRateId returns the TaxRateId field if non-nil, zero value otherwise.

### GetTaxRateIdOk

`func (o *InvoiceLineItemTaxInput) GetTaxRateIdOk() (*string, bool)`

GetTaxRateIdOk returns a tuple with the TaxRateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTaxRateId

`func (o *InvoiceLineItemTaxInput) SetTaxRateId(v string)`

SetTaxRateId sets TaxRateId field to given value.

### HasTaxRateId

`func (o *InvoiceLineItemTaxInput) HasTaxRateId() bool`

HasTaxRateId returns a boolean if a field has been set.

### SetTaxRateIdNil

`func (o *InvoiceLineItemTaxInput) SetTaxRateIdNil(b bool)`

 SetTaxRateIdNil sets the value for TaxRateId to be an explicit nil

### UnsetTaxRateId
`func (o *InvoiceLineItemTaxInput) UnsetTaxRateId()`

UnsetTaxRateId ensures that no value is present for TaxRateId, not even an explicit nil
### GetName

`func (o *InvoiceLineItemTaxInput) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *InvoiceLineItemTaxInput) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *InvoiceLineItemTaxInput) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *InvoiceLineItemTaxInput) HasName() bool`

HasName returns a boolean if a field has been set.

### SetNameNil

`func (o *InvoiceLineItemTaxInput) SetNameNil(b bool)`

 SetNameNil sets the value for Name to be an explicit nil

### UnsetName
`func (o *InvoiceLineItemTaxInput) UnsetName()`

UnsetName ensures that no value is present for Name, not even an explicit nil
### GetRate

`func (o *InvoiceLineItemTaxInput) GetRate() string`

GetRate returns the Rate field if non-nil, zero value otherwise.

### GetRateOk

`func (o *InvoiceLineItemTaxInput) GetRateOk() (*string, bool)`

GetRateOk returns a tuple with the Rate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRate

`func (o *InvoiceLineItemTaxInput) SetRate(v string)`

SetRate sets Rate field to given value.

### HasRate

`func (o *InvoiceLineItemTaxInput) HasRate() bool`

HasRate returns a boolean if a field has been set.

### SetRateNil

`func (o *InvoiceLineItemTaxInput) SetRateNil(b bool)`

 SetRateNil sets the value for Rate to be an explicit nil

### UnsetRate
`func (o *InvoiceLineItemTaxInput) UnsetRate()`

UnsetRate ensures that no value is present for Rate, not even an explicit nil
### GetInclusive

`func (o *InvoiceLineItemTaxInput) GetInclusive() bool`

GetInclusive returns the Inclusive field if non-nil, zero value otherwise.

### GetInclusiveOk

`func (o *InvoiceLineItemTaxInput) GetInclusiveOk() (*bool, bool)`

GetInclusiveOk returns a tuple with the Inclusive field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInclusive

`func (o *InvoiceLineItemTaxInput) SetInclusive(v bool)`

SetInclusive sets Inclusive field to given value.

### HasInclusive

`func (o *InvoiceLineItemTaxInput) HasInclusive() bool`

HasInclusive returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


