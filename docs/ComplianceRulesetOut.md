# ComplianceRulesetOut

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Label** | **string** |  | 
**Version** | Pointer to **string** | The upstream release of the rules. Empty for checks with no version of their own. | [optional] [default to ""]
**Ran** | **bool** | False when this ruleset could not be run at all. A ruleset that did not run is not a pass — &#x60;valid&#x60; only reports what was checked. | 
**Reason** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewComplianceRulesetOut

`func NewComplianceRulesetOut(id string, label string, ran bool, ) *ComplianceRulesetOut`

NewComplianceRulesetOut instantiates a new ComplianceRulesetOut object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewComplianceRulesetOutWithDefaults

`func NewComplianceRulesetOutWithDefaults() *ComplianceRulesetOut`

NewComplianceRulesetOutWithDefaults instantiates a new ComplianceRulesetOut object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ComplianceRulesetOut) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ComplianceRulesetOut) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ComplianceRulesetOut) SetId(v string)`

SetId sets Id field to given value.


### GetLabel

`func (o *ComplianceRulesetOut) GetLabel() string`

GetLabel returns the Label field if non-nil, zero value otherwise.

### GetLabelOk

`func (o *ComplianceRulesetOut) GetLabelOk() (*string, bool)`

GetLabelOk returns a tuple with the Label field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabel

`func (o *ComplianceRulesetOut) SetLabel(v string)`

SetLabel sets Label field to given value.


### GetVersion

`func (o *ComplianceRulesetOut) GetVersion() string`

GetVersion returns the Version field if non-nil, zero value otherwise.

### GetVersionOk

`func (o *ComplianceRulesetOut) GetVersionOk() (*string, bool)`

GetVersionOk returns a tuple with the Version field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersion

`func (o *ComplianceRulesetOut) SetVersion(v string)`

SetVersion sets Version field to given value.

### HasVersion

`func (o *ComplianceRulesetOut) HasVersion() bool`

HasVersion returns a boolean if a field has been set.

### GetRan

`func (o *ComplianceRulesetOut) GetRan() bool`

GetRan returns the Ran field if non-nil, zero value otherwise.

### GetRanOk

`func (o *ComplianceRulesetOut) GetRanOk() (*bool, bool)`

GetRanOk returns a tuple with the Ran field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRan

`func (o *ComplianceRulesetOut) SetRan(v bool)`

SetRan sets Ran field to given value.


### GetReason

`func (o *ComplianceRulesetOut) GetReason() string`

GetReason returns the Reason field if non-nil, zero value otherwise.

### GetReasonOk

`func (o *ComplianceRulesetOut) GetReasonOk() (*string, bool)`

GetReasonOk returns a tuple with the Reason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReason

`func (o *ComplianceRulesetOut) SetReason(v string)`

SetReason sets Reason field to given value.

### HasReason

`func (o *ComplianceRulesetOut) HasReason() bool`

HasReason returns a boolean if a field has been set.

### SetReasonNil

`func (o *ComplianceRulesetOut) SetReasonNil(b bool)`

 SetReasonNil sets the value for Reason to be an explicit nil

### UnsetReason
`func (o *ComplianceRulesetOut) UnsetReason()`

UnsetReason ensures that no value is present for Reason, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


