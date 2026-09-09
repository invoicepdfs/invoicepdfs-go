# ComplianceViolationOut

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Rule** | **string** | The identifier the standard uses — a business term from the mandatory-field check, a rule id from Schematron. A rule id is what a rejection notice from an access point quotes. | 
**Path** | **string** | Where the problem is. The mandatory-field check names a field of the request; Schematron names the node in the generated XML. | 
**Message** | **string** |  | 
**Severity** | Pointer to **string** | &#x60;fatal&#x60; would get the document rejected. &#x60;warning&#x60; is a recommendation — both EN 16931 and Peppol grade a large share of their rules as advisory, and &#x60;valid&#x60; ignores those. | [optional] [default to "fatal"]
**Ruleset** | Pointer to **string** | Which ruleset found it — matches an &#x60;id&#x60; in &#x60;rulesets&#x60;. | [optional] [default to "semantic"]

## Methods

### NewComplianceViolationOut

`func NewComplianceViolationOut(rule string, path string, message string, ) *ComplianceViolationOut`

NewComplianceViolationOut instantiates a new ComplianceViolationOut object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewComplianceViolationOutWithDefaults

`func NewComplianceViolationOutWithDefaults() *ComplianceViolationOut`

NewComplianceViolationOutWithDefaults instantiates a new ComplianceViolationOut object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRule

`func (o *ComplianceViolationOut) GetRule() string`

GetRule returns the Rule field if non-nil, zero value otherwise.

### GetRuleOk

`func (o *ComplianceViolationOut) GetRuleOk() (*string, bool)`

GetRuleOk returns a tuple with the Rule field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRule

`func (o *ComplianceViolationOut) SetRule(v string)`

SetRule sets Rule field to given value.


### GetPath

`func (o *ComplianceViolationOut) GetPath() string`

GetPath returns the Path field if non-nil, zero value otherwise.

### GetPathOk

`func (o *ComplianceViolationOut) GetPathOk() (*string, bool)`

GetPathOk returns a tuple with the Path field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPath

`func (o *ComplianceViolationOut) SetPath(v string)`

SetPath sets Path field to given value.


### GetMessage

`func (o *ComplianceViolationOut) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *ComplianceViolationOut) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *ComplianceViolationOut) SetMessage(v string)`

SetMessage sets Message field to given value.


### GetSeverity

`func (o *ComplianceViolationOut) GetSeverity() string`

GetSeverity returns the Severity field if non-nil, zero value otherwise.

### GetSeverityOk

`func (o *ComplianceViolationOut) GetSeverityOk() (*string, bool)`

GetSeverityOk returns a tuple with the Severity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSeverity

`func (o *ComplianceViolationOut) SetSeverity(v string)`

SetSeverity sets Severity field to given value.

### HasSeverity

`func (o *ComplianceViolationOut) HasSeverity() bool`

HasSeverity returns a boolean if a field has been set.

### GetRuleset

`func (o *ComplianceViolationOut) GetRuleset() string`

GetRuleset returns the Ruleset field if non-nil, zero value otherwise.

### GetRulesetOk

`func (o *ComplianceViolationOut) GetRulesetOk() (*string, bool)`

GetRulesetOk returns a tuple with the Ruleset field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRuleset

`func (o *ComplianceViolationOut) SetRuleset(v string)`

SetRuleset sets Ruleset field to given value.

### HasRuleset

`func (o *ComplianceViolationOut) HasRuleset() bool`

HasRuleset returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


