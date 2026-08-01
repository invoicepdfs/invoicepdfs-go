# TaxRateCreateRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** |  | 
**Rate** | **string** |  | 
**Inclusive** | Pointer to **bool** |  | [optional] [default to false]
**Jurisdiction** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewTaxRateCreateRequest

`func NewTaxRateCreateRequest(name string, rate string, ) *TaxRateCreateRequest`

NewTaxRateCreateRequest instantiates a new TaxRateCreateRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTaxRateCreateRequestWithDefaults

`func NewTaxRateCreateRequestWithDefaults() *TaxRateCreateRequest`

NewTaxRateCreateRequestWithDefaults instantiates a new TaxRateCreateRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *TaxRateCreateRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *TaxRateCreateRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *TaxRateCreateRequest) SetName(v string)`

SetName sets Name field to given value.


### GetRate

`func (o *TaxRateCreateRequest) GetRate() string`

GetRate returns the Rate field if non-nil, zero value otherwise.

### GetRateOk

`func (o *TaxRateCreateRequest) GetRateOk() (*string, bool)`

GetRateOk returns a tuple with the Rate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRate

`func (o *TaxRateCreateRequest) SetRate(v string)`

SetRate sets Rate field to given value.


### GetInclusive

`func (o *TaxRateCreateRequest) GetInclusive() bool`

GetInclusive returns the Inclusive field if non-nil, zero value otherwise.

### GetInclusiveOk

`func (o *TaxRateCreateRequest) GetInclusiveOk() (*bool, bool)`

GetInclusiveOk returns a tuple with the Inclusive field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInclusive

`func (o *TaxRateCreateRequest) SetInclusive(v bool)`

SetInclusive sets Inclusive field to given value.

### HasInclusive

`func (o *TaxRateCreateRequest) HasInclusive() bool`

HasInclusive returns a boolean if a field has been set.

### GetJurisdiction

`func (o *TaxRateCreateRequest) GetJurisdiction() string`

GetJurisdiction returns the Jurisdiction field if non-nil, zero value otherwise.

### GetJurisdictionOk

`func (o *TaxRateCreateRequest) GetJurisdictionOk() (*string, bool)`

GetJurisdictionOk returns a tuple with the Jurisdiction field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJurisdiction

`func (o *TaxRateCreateRequest) SetJurisdiction(v string)`

SetJurisdiction sets Jurisdiction field to given value.

### HasJurisdiction

`func (o *TaxRateCreateRequest) HasJurisdiction() bool`

HasJurisdiction returns a boolean if a field has been set.

### SetJurisdictionNil

`func (o *TaxRateCreateRequest) SetJurisdictionNil(b bool)`

 SetJurisdictionNil sets the value for Jurisdiction to be an explicit nil

### UnsetJurisdiction
`func (o *TaxRateCreateRequest) UnsetJurisdiction()`

UnsetJurisdiction ensures that no value is present for Jurisdiction, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


