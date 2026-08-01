# DocumentLineItemTaxInput

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** |  | 
**Rate** | **string** |  | 
**Inclusive** | Pointer to **bool** |  | [optional] [default to false]

## Methods

### NewDocumentLineItemTaxInput

`func NewDocumentLineItemTaxInput(name string, rate string, ) *DocumentLineItemTaxInput`

NewDocumentLineItemTaxInput instantiates a new DocumentLineItemTaxInput object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDocumentLineItemTaxInputWithDefaults

`func NewDocumentLineItemTaxInputWithDefaults() *DocumentLineItemTaxInput`

NewDocumentLineItemTaxInputWithDefaults instantiates a new DocumentLineItemTaxInput object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *DocumentLineItemTaxInput) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *DocumentLineItemTaxInput) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *DocumentLineItemTaxInput) SetName(v string)`

SetName sets Name field to given value.


### GetRate

`func (o *DocumentLineItemTaxInput) GetRate() string`

GetRate returns the Rate field if non-nil, zero value otherwise.

### GetRateOk

`func (o *DocumentLineItemTaxInput) GetRateOk() (*string, bool)`

GetRateOk returns a tuple with the Rate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRate

`func (o *DocumentLineItemTaxInput) SetRate(v string)`

SetRate sets Rate field to given value.


### GetInclusive

`func (o *DocumentLineItemTaxInput) GetInclusive() bool`

GetInclusive returns the Inclusive field if non-nil, zero value otherwise.

### GetInclusiveOk

`func (o *DocumentLineItemTaxInput) GetInclusiveOk() (*bool, bool)`

GetInclusiveOk returns a tuple with the Inclusive field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInclusive

`func (o *DocumentLineItemTaxInput) SetInclusive(v bool)`

SetInclusive sets Inclusive field to given value.

### HasInclusive

`func (o *DocumentLineItemTaxInput) HasInclusive() bool`

HasInclusive returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


