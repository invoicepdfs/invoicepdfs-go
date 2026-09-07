# TaxCategory

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Code** | **string** | UNCL5305 tax category code — S standard, Z zero-rated, E exempt, AE reverse charge, K intra-community, G export, O outside scope | 
**ExemptionReason** | Pointer to **NullableString** |  | [optional] 
**ExemptionReasonCode** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewTaxCategory

`func NewTaxCategory(code string, ) *TaxCategory`

NewTaxCategory instantiates a new TaxCategory object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTaxCategoryWithDefaults

`func NewTaxCategoryWithDefaults() *TaxCategory`

NewTaxCategoryWithDefaults instantiates a new TaxCategory object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCode

`func (o *TaxCategory) GetCode() string`

GetCode returns the Code field if non-nil, zero value otherwise.

### GetCodeOk

`func (o *TaxCategory) GetCodeOk() (*string, bool)`

GetCodeOk returns a tuple with the Code field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCode

`func (o *TaxCategory) SetCode(v string)`

SetCode sets Code field to given value.


### GetExemptionReason

`func (o *TaxCategory) GetExemptionReason() string`

GetExemptionReason returns the ExemptionReason field if non-nil, zero value otherwise.

### GetExemptionReasonOk

`func (o *TaxCategory) GetExemptionReasonOk() (*string, bool)`

GetExemptionReasonOk returns a tuple with the ExemptionReason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExemptionReason

`func (o *TaxCategory) SetExemptionReason(v string)`

SetExemptionReason sets ExemptionReason field to given value.

### HasExemptionReason

`func (o *TaxCategory) HasExemptionReason() bool`

HasExemptionReason returns a boolean if a field has been set.

### SetExemptionReasonNil

`func (o *TaxCategory) SetExemptionReasonNil(b bool)`

 SetExemptionReasonNil sets the value for ExemptionReason to be an explicit nil

### UnsetExemptionReason
`func (o *TaxCategory) UnsetExemptionReason()`

UnsetExemptionReason ensures that no value is present for ExemptionReason, not even an explicit nil
### GetExemptionReasonCode

`func (o *TaxCategory) GetExemptionReasonCode() string`

GetExemptionReasonCode returns the ExemptionReasonCode field if non-nil, zero value otherwise.

### GetExemptionReasonCodeOk

`func (o *TaxCategory) GetExemptionReasonCodeOk() (*string, bool)`

GetExemptionReasonCodeOk returns a tuple with the ExemptionReasonCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExemptionReasonCode

`func (o *TaxCategory) SetExemptionReasonCode(v string)`

SetExemptionReasonCode sets ExemptionReasonCode field to given value.

### HasExemptionReasonCode

`func (o *TaxCategory) HasExemptionReasonCode() bool`

HasExemptionReasonCode returns a boolean if a field has been set.

### SetExemptionReasonCodeNil

`func (o *TaxCategory) SetExemptionReasonCodeNil(b bool)`

 SetExemptionReasonCodeNil sets the value for ExemptionReasonCode to be an explicit nil

### UnsetExemptionReasonCode
`func (o *TaxCategory) UnsetExemptionReasonCode()`

UnsetExemptionReasonCode ensures that no value is present for ExemptionReasonCode, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


