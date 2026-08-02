# BrandingProfilePatchRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **NullableString** |  | [optional] 
**PrimaryColor** | Pointer to **NullableString** |  | [optional] 
**AccentColor** | Pointer to **NullableString** |  | [optional] 
**FontFamily** | Pointer to **NullableString** |  | [optional] 
**HeaderText** | Pointer to **NullableString** |  | [optional] 
**FooterText** | Pointer to **NullableString** |  | [optional] 
**HideInvoicepdfsBranding** | Pointer to **NullableBool** |  | [optional] 
**IsDefault** | Pointer to **NullableBool** |  | [optional] 

## Methods

### NewBrandingProfilePatchRequest

`func NewBrandingProfilePatchRequest() *BrandingProfilePatchRequest`

NewBrandingProfilePatchRequest instantiates a new BrandingProfilePatchRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBrandingProfilePatchRequestWithDefaults

`func NewBrandingProfilePatchRequestWithDefaults() *BrandingProfilePatchRequest`

NewBrandingProfilePatchRequestWithDefaults instantiates a new BrandingProfilePatchRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *BrandingProfilePatchRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *BrandingProfilePatchRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *BrandingProfilePatchRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *BrandingProfilePatchRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### SetNameNil

`func (o *BrandingProfilePatchRequest) SetNameNil(b bool)`

 SetNameNil sets the value for Name to be an explicit nil

### UnsetName
`func (o *BrandingProfilePatchRequest) UnsetName()`

UnsetName ensures that no value is present for Name, not even an explicit nil
### GetPrimaryColor

`func (o *BrandingProfilePatchRequest) GetPrimaryColor() string`

GetPrimaryColor returns the PrimaryColor field if non-nil, zero value otherwise.

### GetPrimaryColorOk

`func (o *BrandingProfilePatchRequest) GetPrimaryColorOk() (*string, bool)`

GetPrimaryColorOk returns a tuple with the PrimaryColor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrimaryColor

`func (o *BrandingProfilePatchRequest) SetPrimaryColor(v string)`

SetPrimaryColor sets PrimaryColor field to given value.

### HasPrimaryColor

`func (o *BrandingProfilePatchRequest) HasPrimaryColor() bool`

HasPrimaryColor returns a boolean if a field has been set.

### SetPrimaryColorNil

`func (o *BrandingProfilePatchRequest) SetPrimaryColorNil(b bool)`

 SetPrimaryColorNil sets the value for PrimaryColor to be an explicit nil

### UnsetPrimaryColor
`func (o *BrandingProfilePatchRequest) UnsetPrimaryColor()`

UnsetPrimaryColor ensures that no value is present for PrimaryColor, not even an explicit nil
### GetAccentColor

`func (o *BrandingProfilePatchRequest) GetAccentColor() string`

GetAccentColor returns the AccentColor field if non-nil, zero value otherwise.

### GetAccentColorOk

`func (o *BrandingProfilePatchRequest) GetAccentColorOk() (*string, bool)`

GetAccentColorOk returns a tuple with the AccentColor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccentColor

`func (o *BrandingProfilePatchRequest) SetAccentColor(v string)`

SetAccentColor sets AccentColor field to given value.

### HasAccentColor

`func (o *BrandingProfilePatchRequest) HasAccentColor() bool`

HasAccentColor returns a boolean if a field has been set.

### SetAccentColorNil

`func (o *BrandingProfilePatchRequest) SetAccentColorNil(b bool)`

 SetAccentColorNil sets the value for AccentColor to be an explicit nil

### UnsetAccentColor
`func (o *BrandingProfilePatchRequest) UnsetAccentColor()`

UnsetAccentColor ensures that no value is present for AccentColor, not even an explicit nil
### GetFontFamily

`func (o *BrandingProfilePatchRequest) GetFontFamily() string`

GetFontFamily returns the FontFamily field if non-nil, zero value otherwise.

### GetFontFamilyOk

`func (o *BrandingProfilePatchRequest) GetFontFamilyOk() (*string, bool)`

GetFontFamilyOk returns a tuple with the FontFamily field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFontFamily

`func (o *BrandingProfilePatchRequest) SetFontFamily(v string)`

SetFontFamily sets FontFamily field to given value.

### HasFontFamily

`func (o *BrandingProfilePatchRequest) HasFontFamily() bool`

HasFontFamily returns a boolean if a field has been set.

### SetFontFamilyNil

`func (o *BrandingProfilePatchRequest) SetFontFamilyNil(b bool)`

 SetFontFamilyNil sets the value for FontFamily to be an explicit nil

### UnsetFontFamily
`func (o *BrandingProfilePatchRequest) UnsetFontFamily()`

UnsetFontFamily ensures that no value is present for FontFamily, not even an explicit nil
### GetHeaderText

`func (o *BrandingProfilePatchRequest) GetHeaderText() string`

GetHeaderText returns the HeaderText field if non-nil, zero value otherwise.

### GetHeaderTextOk

`func (o *BrandingProfilePatchRequest) GetHeaderTextOk() (*string, bool)`

GetHeaderTextOk returns a tuple with the HeaderText field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHeaderText

`func (o *BrandingProfilePatchRequest) SetHeaderText(v string)`

SetHeaderText sets HeaderText field to given value.

### HasHeaderText

`func (o *BrandingProfilePatchRequest) HasHeaderText() bool`

HasHeaderText returns a boolean if a field has been set.

### SetHeaderTextNil

`func (o *BrandingProfilePatchRequest) SetHeaderTextNil(b bool)`

 SetHeaderTextNil sets the value for HeaderText to be an explicit nil

### UnsetHeaderText
`func (o *BrandingProfilePatchRequest) UnsetHeaderText()`

UnsetHeaderText ensures that no value is present for HeaderText, not even an explicit nil
### GetFooterText

`func (o *BrandingProfilePatchRequest) GetFooterText() string`

GetFooterText returns the FooterText field if non-nil, zero value otherwise.

### GetFooterTextOk

`func (o *BrandingProfilePatchRequest) GetFooterTextOk() (*string, bool)`

GetFooterTextOk returns a tuple with the FooterText field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFooterText

`func (o *BrandingProfilePatchRequest) SetFooterText(v string)`

SetFooterText sets FooterText field to given value.

### HasFooterText

`func (o *BrandingProfilePatchRequest) HasFooterText() bool`

HasFooterText returns a boolean if a field has been set.

### SetFooterTextNil

`func (o *BrandingProfilePatchRequest) SetFooterTextNil(b bool)`

 SetFooterTextNil sets the value for FooterText to be an explicit nil

### UnsetFooterText
`func (o *BrandingProfilePatchRequest) UnsetFooterText()`

UnsetFooterText ensures that no value is present for FooterText, not even an explicit nil
### GetHideInvoicepdfsBranding

`func (o *BrandingProfilePatchRequest) GetHideInvoicepdfsBranding() bool`

GetHideInvoicepdfsBranding returns the HideInvoicepdfsBranding field if non-nil, zero value otherwise.

### GetHideInvoicepdfsBrandingOk

`func (o *BrandingProfilePatchRequest) GetHideInvoicepdfsBrandingOk() (*bool, bool)`

GetHideInvoicepdfsBrandingOk returns a tuple with the HideInvoicepdfsBranding field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHideInvoicepdfsBranding

`func (o *BrandingProfilePatchRequest) SetHideInvoicepdfsBranding(v bool)`

SetHideInvoicepdfsBranding sets HideInvoicepdfsBranding field to given value.

### HasHideInvoicepdfsBranding

`func (o *BrandingProfilePatchRequest) HasHideInvoicepdfsBranding() bool`

HasHideInvoicepdfsBranding returns a boolean if a field has been set.

### SetHideInvoicepdfsBrandingNil

`func (o *BrandingProfilePatchRequest) SetHideInvoicepdfsBrandingNil(b bool)`

 SetHideInvoicepdfsBrandingNil sets the value for HideInvoicepdfsBranding to be an explicit nil

### UnsetHideInvoicepdfsBranding
`func (o *BrandingProfilePatchRequest) UnsetHideInvoicepdfsBranding()`

UnsetHideInvoicepdfsBranding ensures that no value is present for HideInvoicepdfsBranding, not even an explicit nil
### GetIsDefault

`func (o *BrandingProfilePatchRequest) GetIsDefault() bool`

GetIsDefault returns the IsDefault field if non-nil, zero value otherwise.

### GetIsDefaultOk

`func (o *BrandingProfilePatchRequest) GetIsDefaultOk() (*bool, bool)`

GetIsDefaultOk returns a tuple with the IsDefault field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsDefault

`func (o *BrandingProfilePatchRequest) SetIsDefault(v bool)`

SetIsDefault sets IsDefault field to given value.

### HasIsDefault

`func (o *BrandingProfilePatchRequest) HasIsDefault() bool`

HasIsDefault returns a boolean if a field has been set.

### SetIsDefaultNil

`func (o *BrandingProfilePatchRequest) SetIsDefaultNil(b bool)`

 SetIsDefaultNil sets the value for IsDefault to be an explicit nil

### UnsetIsDefault
`func (o *BrandingProfilePatchRequest) UnsetIsDefault()`

UnsetIsDefault ensures that no value is present for IsDefault, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


