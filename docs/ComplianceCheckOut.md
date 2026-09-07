# ComplianceCheckOut

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Profile** | **string** |  | 
**RulesetVersion** | **string** | The version these rules came from. Worth recording alongside any document you file — rulesets revise, and &#39;which rules did this pass?&#39; is what an audit asks years later. | 
**Valid** | **bool** |  | 
**Violations** | Pointer to [**[]ComplianceViolationOut**](ComplianceViolationOut.md) | Every violation found, not the first — fixing one field per round trip is the experience this avoids. | [optional] 

## Methods

### NewComplianceCheckOut

`func NewComplianceCheckOut(profile string, rulesetVersion string, valid bool, ) *ComplianceCheckOut`

NewComplianceCheckOut instantiates a new ComplianceCheckOut object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewComplianceCheckOutWithDefaults

`func NewComplianceCheckOutWithDefaults() *ComplianceCheckOut`

NewComplianceCheckOutWithDefaults instantiates a new ComplianceCheckOut object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetProfile

`func (o *ComplianceCheckOut) GetProfile() string`

GetProfile returns the Profile field if non-nil, zero value otherwise.

### GetProfileOk

`func (o *ComplianceCheckOut) GetProfileOk() (*string, bool)`

GetProfileOk returns a tuple with the Profile field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProfile

`func (o *ComplianceCheckOut) SetProfile(v string)`

SetProfile sets Profile field to given value.


### GetRulesetVersion

`func (o *ComplianceCheckOut) GetRulesetVersion() string`

GetRulesetVersion returns the RulesetVersion field if non-nil, zero value otherwise.

### GetRulesetVersionOk

`func (o *ComplianceCheckOut) GetRulesetVersionOk() (*string, bool)`

GetRulesetVersionOk returns a tuple with the RulesetVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRulesetVersion

`func (o *ComplianceCheckOut) SetRulesetVersion(v string)`

SetRulesetVersion sets RulesetVersion field to given value.


### GetValid

`func (o *ComplianceCheckOut) GetValid() bool`

GetValid returns the Valid field if non-nil, zero value otherwise.

### GetValidOk

`func (o *ComplianceCheckOut) GetValidOk() (*bool, bool)`

GetValidOk returns a tuple with the Valid field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValid

`func (o *ComplianceCheckOut) SetValid(v bool)`

SetValid sets Valid field to given value.


### GetViolations

`func (o *ComplianceCheckOut) GetViolations() []ComplianceViolationOut`

GetViolations returns the Violations field if non-nil, zero value otherwise.

### GetViolationsOk

`func (o *ComplianceCheckOut) GetViolationsOk() (*[]ComplianceViolationOut, bool)`

GetViolationsOk returns a tuple with the Violations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetViolations

`func (o *ComplianceCheckOut) SetViolations(v []ComplianceViolationOut)`

SetViolations sets Violations field to given value.

### HasViolations

`func (o *ComplianceCheckOut) HasViolations() bool`

HasViolations returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


