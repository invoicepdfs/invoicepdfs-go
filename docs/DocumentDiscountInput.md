# DocumentDiscountInput

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | Pointer to **string** |  | [optional] [default to "percentage"]
**Value** | **string** |  | 
**Reason** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewDocumentDiscountInput

`func NewDocumentDiscountInput(value string, ) *DocumentDiscountInput`

NewDocumentDiscountInput instantiates a new DocumentDiscountInput object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDocumentDiscountInputWithDefaults

`func NewDocumentDiscountInputWithDefaults() *DocumentDiscountInput`

NewDocumentDiscountInputWithDefaults instantiates a new DocumentDiscountInput object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *DocumentDiscountInput) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *DocumentDiscountInput) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *DocumentDiscountInput) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *DocumentDiscountInput) HasType() bool`

HasType returns a boolean if a field has been set.

### GetValue

`func (o *DocumentDiscountInput) GetValue() string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *DocumentDiscountInput) GetValueOk() (*string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *DocumentDiscountInput) SetValue(v string)`

SetValue sets Value field to given value.


### GetReason

`func (o *DocumentDiscountInput) GetReason() string`

GetReason returns the Reason field if non-nil, zero value otherwise.

### GetReasonOk

`func (o *DocumentDiscountInput) GetReasonOk() (*string, bool)`

GetReasonOk returns a tuple with the Reason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReason

`func (o *DocumentDiscountInput) SetReason(v string)`

SetReason sets Reason field to given value.

### HasReason

`func (o *DocumentDiscountInput) HasReason() bool`

HasReason returns a boolean if a field has been set.

### SetReasonNil

`func (o *DocumentDiscountInput) SetReasonNil(b bool)`

 SetReasonNil sets the value for Reason to be an explicit nil

### UnsetReason
`func (o *DocumentDiscountInput) UnsetReason()`

UnsetReason ensures that no value is present for Reason, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


