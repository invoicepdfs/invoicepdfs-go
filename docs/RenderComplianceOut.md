# RenderComplianceOut

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Profile** | **string** | The ruleset this document was built and validated against. | 
**RulesetVersion** | **string** | The artefact versions the check actually ran. A profile is held to more than one ruleset, and they are regenerated over time, so this is what makes &#39;which rules did this pass?&#39; answerable later. | 
**FullyChecked** | **bool** | False when a ruleset could not run. The document still satisfied everything that did, but the authoritative Schematron tier being absent is a materially weaker statement than it passing. | 
**Advisories** | Pointer to [**[]ComplianceViolationOut**](ComplianceViolationOut.md) | Non-fatal findings the render proceeded past. Both rulesets grade a large share of their rules as advisory, so these are worth reading and are not a rejection. | [optional] 

## Methods

### NewRenderComplianceOut

`func NewRenderComplianceOut(profile string, rulesetVersion string, fullyChecked bool, ) *RenderComplianceOut`

NewRenderComplianceOut instantiates a new RenderComplianceOut object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRenderComplianceOutWithDefaults

`func NewRenderComplianceOutWithDefaults() *RenderComplianceOut`

NewRenderComplianceOutWithDefaults instantiates a new RenderComplianceOut object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetProfile

`func (o *RenderComplianceOut) GetProfile() string`

GetProfile returns the Profile field if non-nil, zero value otherwise.

### GetProfileOk

`func (o *RenderComplianceOut) GetProfileOk() (*string, bool)`

GetProfileOk returns a tuple with the Profile field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProfile

`func (o *RenderComplianceOut) SetProfile(v string)`

SetProfile sets Profile field to given value.


### GetRulesetVersion

`func (o *RenderComplianceOut) GetRulesetVersion() string`

GetRulesetVersion returns the RulesetVersion field if non-nil, zero value otherwise.

### GetRulesetVersionOk

`func (o *RenderComplianceOut) GetRulesetVersionOk() (*string, bool)`

GetRulesetVersionOk returns a tuple with the RulesetVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRulesetVersion

`func (o *RenderComplianceOut) SetRulesetVersion(v string)`

SetRulesetVersion sets RulesetVersion field to given value.


### GetFullyChecked

`func (o *RenderComplianceOut) GetFullyChecked() bool`

GetFullyChecked returns the FullyChecked field if non-nil, zero value otherwise.

### GetFullyCheckedOk

`func (o *RenderComplianceOut) GetFullyCheckedOk() (*bool, bool)`

GetFullyCheckedOk returns a tuple with the FullyChecked field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFullyChecked

`func (o *RenderComplianceOut) SetFullyChecked(v bool)`

SetFullyChecked sets FullyChecked field to given value.


### GetAdvisories

`func (o *RenderComplianceOut) GetAdvisories() []ComplianceViolationOut`

GetAdvisories returns the Advisories field if non-nil, zero value otherwise.

### GetAdvisoriesOk

`func (o *RenderComplianceOut) GetAdvisoriesOk() (*[]ComplianceViolationOut, bool)`

GetAdvisoriesOk returns a tuple with the Advisories field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAdvisories

`func (o *RenderComplianceOut) SetAdvisories(v []ComplianceViolationOut)`

SetAdvisories sets Advisories field to given value.

### HasAdvisories

`func (o *RenderComplianceOut) HasAdvisories() bool`

HasAdvisories returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


