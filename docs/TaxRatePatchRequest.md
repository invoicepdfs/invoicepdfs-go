# TaxRatePatchRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **string** |  | [optional] 
**Rate** | Pointer to **string** |  | [optional] 
**Inclusive** | Pointer to **bool** |  | [optional] 
**Jurisdiction** | Pointer to **NullableString** |  | [optional] 
**IsActive** | Pointer to **bool** |  | [optional] 

## Methods

### NewTaxRatePatchRequest

`func NewTaxRatePatchRequest() *TaxRatePatchRequest`

NewTaxRatePatchRequest instantiates a new TaxRatePatchRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTaxRatePatchRequestWithDefaults

`func NewTaxRatePatchRequestWithDefaults() *TaxRatePatchRequest`

NewTaxRatePatchRequestWithDefaults instantiates a new TaxRatePatchRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *TaxRatePatchRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *TaxRatePatchRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *TaxRatePatchRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *TaxRatePatchRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### GetRate

`func (o *TaxRatePatchRequest) GetRate() string`

GetRate returns the Rate field if non-nil, zero value otherwise.

### GetRateOk

`func (o *TaxRatePatchRequest) GetRateOk() (*string, bool)`

GetRateOk returns a tuple with the Rate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRate

`func (o *TaxRatePatchRequest) SetRate(v string)`

SetRate sets Rate field to given value.

### HasRate

`func (o *TaxRatePatchRequest) HasRate() bool`

HasRate returns a boolean if a field has been set.

### GetInclusive

`func (o *TaxRatePatchRequest) GetInclusive() bool`

GetInclusive returns the Inclusive field if non-nil, zero value otherwise.

### GetInclusiveOk

`func (o *TaxRatePatchRequest) GetInclusiveOk() (*bool, bool)`

GetInclusiveOk returns a tuple with the Inclusive field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInclusive

`func (o *TaxRatePatchRequest) SetInclusive(v bool)`

SetInclusive sets Inclusive field to given value.

### HasInclusive

`func (o *TaxRatePatchRequest) HasInclusive() bool`

HasInclusive returns a boolean if a field has been set.

### GetJurisdiction

`func (o *TaxRatePatchRequest) GetJurisdiction() string`

GetJurisdiction returns the Jurisdiction field if non-nil, zero value otherwise.

### GetJurisdictionOk

`func (o *TaxRatePatchRequest) GetJurisdictionOk() (*string, bool)`

GetJurisdictionOk returns a tuple with the Jurisdiction field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJurisdiction

`func (o *TaxRatePatchRequest) SetJurisdiction(v string)`

SetJurisdiction sets Jurisdiction field to given value.

### HasJurisdiction

`func (o *TaxRatePatchRequest) HasJurisdiction() bool`

HasJurisdiction returns a boolean if a field has been set.

### SetJurisdictionNil

`func (o *TaxRatePatchRequest) SetJurisdictionNil(b bool)`

 SetJurisdictionNil sets the value for Jurisdiction to be an explicit nil

### UnsetJurisdiction
`func (o *TaxRatePatchRequest) UnsetJurisdiction()`

UnsetJurisdiction ensures that no value is present for Jurisdiction, not even an explicit nil
### GetIsActive

`func (o *TaxRatePatchRequest) GetIsActive() bool`

GetIsActive returns the IsActive field if non-nil, zero value otherwise.

### GetIsActiveOk

`func (o *TaxRatePatchRequest) GetIsActiveOk() (*bool, bool)`

GetIsActiveOk returns a tuple with the IsActive field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsActive

`func (o *TaxRatePatchRequest) SetIsActive(v bool)`

SetIsActive sets IsActive field to given value.

### HasIsActive

`func (o *TaxRatePatchRequest) HasIsActive() bool`

HasIsActive returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


