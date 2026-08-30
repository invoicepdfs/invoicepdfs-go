# DocumentShippingInput

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Description** | Pointer to **string** |  | [optional] [default to "Shipping"]
**Amount** | **string** |  | 
**Taxable** | Pointer to **bool** |  | [optional] [default to false]

## Methods

### NewDocumentShippingInput

`func NewDocumentShippingInput(amount string, ) *DocumentShippingInput`

NewDocumentShippingInput instantiates a new DocumentShippingInput object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDocumentShippingInputWithDefaults

`func NewDocumentShippingInputWithDefaults() *DocumentShippingInput`

NewDocumentShippingInputWithDefaults instantiates a new DocumentShippingInput object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDescription

`func (o *DocumentShippingInput) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *DocumentShippingInput) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *DocumentShippingInput) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *DocumentShippingInput) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetAmount

`func (o *DocumentShippingInput) GetAmount() string`

GetAmount returns the Amount field if non-nil, zero value otherwise.

### GetAmountOk

`func (o *DocumentShippingInput) GetAmountOk() (*string, bool)`

GetAmountOk returns a tuple with the Amount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAmount

`func (o *DocumentShippingInput) SetAmount(v string)`

SetAmount sets Amount field to given value.


### GetTaxable

`func (o *DocumentShippingInput) GetTaxable() bool`

GetTaxable returns the Taxable field if non-nil, zero value otherwise.

### GetTaxableOk

`func (o *DocumentShippingInput) GetTaxableOk() (*bool, bool)`

GetTaxableOk returns a tuple with the Taxable field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTaxable

`func (o *DocumentShippingInput) SetTaxable(v bool)`

SetTaxable sets Taxable field to given value.

### HasTaxable

`func (o *DocumentShippingInput) HasTaxable() bool`

HasTaxable returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


