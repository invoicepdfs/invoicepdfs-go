# ElectronicAddress

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Value** | **string** |  | 
**SchemeId** | **string** | EAS code list identifier — 0088 is GLN, 9930 a German VAT number. | 

## Methods

### NewElectronicAddress

`func NewElectronicAddress(value string, schemeId string, ) *ElectronicAddress`

NewElectronicAddress instantiates a new ElectronicAddress object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewElectronicAddressWithDefaults

`func NewElectronicAddressWithDefaults() *ElectronicAddress`

NewElectronicAddressWithDefaults instantiates a new ElectronicAddress object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetValue

`func (o *ElectronicAddress) GetValue() string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *ElectronicAddress) GetValueOk() (*string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *ElectronicAddress) SetValue(v string)`

SetValue sets Value field to given value.


### GetSchemeId

`func (o *ElectronicAddress) GetSchemeId() string`

GetSchemeId returns the SchemeId field if non-nil, zero value otherwise.

### GetSchemeIdOk

`func (o *ElectronicAddress) GetSchemeIdOk() (*string, bool)`

GetSchemeIdOk returns a tuple with the SchemeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSchemeId

`func (o *ElectronicAddress) SetSchemeId(v string)`

SetSchemeId sets SchemeId field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


