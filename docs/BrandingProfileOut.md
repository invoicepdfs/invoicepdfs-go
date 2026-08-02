# BrandingProfileOut

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Name** | **string** |  | 
**IsDefault** | **bool** |  | 
**LogoFileId** | Pointer to **NullableString** |  | [optional] 
**PrimaryColor** | **string** |  | 
**AccentColor** | **string** |  | 
**FontFamily** | Pointer to **NullableString** |  | [optional] 
**HeaderText** | Pointer to **NullableString** |  | [optional] 
**FooterText** | **string** |  | 
**HideInvoicepdfsBranding** | **bool** |  | 
**CreatedAt** | **string** |  | 
**UpdatedAt** | **string** |  | 

## Methods

### NewBrandingProfileOut

`func NewBrandingProfileOut(id string, name string, isDefault bool, primaryColor string, accentColor string, footerText string, hideInvoicepdfsBranding bool, createdAt string, updatedAt string, ) *BrandingProfileOut`

NewBrandingProfileOut instantiates a new BrandingProfileOut object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBrandingProfileOutWithDefaults

`func NewBrandingProfileOutWithDefaults() *BrandingProfileOut`

NewBrandingProfileOutWithDefaults instantiates a new BrandingProfileOut object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *BrandingProfileOut) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *BrandingProfileOut) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *BrandingProfileOut) SetId(v string)`

SetId sets Id field to given value.


### GetName

`func (o *BrandingProfileOut) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *BrandingProfileOut) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *BrandingProfileOut) SetName(v string)`

SetName sets Name field to given value.


### GetIsDefault

`func (o *BrandingProfileOut) GetIsDefault() bool`

GetIsDefault returns the IsDefault field if non-nil, zero value otherwise.

### GetIsDefaultOk

`func (o *BrandingProfileOut) GetIsDefaultOk() (*bool, bool)`

GetIsDefaultOk returns a tuple with the IsDefault field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsDefault

`func (o *BrandingProfileOut) SetIsDefault(v bool)`

SetIsDefault sets IsDefault field to given value.


### GetLogoFileId

`func (o *BrandingProfileOut) GetLogoFileId() string`

GetLogoFileId returns the LogoFileId field if non-nil, zero value otherwise.

### GetLogoFileIdOk

`func (o *BrandingProfileOut) GetLogoFileIdOk() (*string, bool)`

GetLogoFileIdOk returns a tuple with the LogoFileId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogoFileId

`func (o *BrandingProfileOut) SetLogoFileId(v string)`

SetLogoFileId sets LogoFileId field to given value.

### HasLogoFileId

`func (o *BrandingProfileOut) HasLogoFileId() bool`

HasLogoFileId returns a boolean if a field has been set.

### SetLogoFileIdNil

`func (o *BrandingProfileOut) SetLogoFileIdNil(b bool)`

 SetLogoFileIdNil sets the value for LogoFileId to be an explicit nil

### UnsetLogoFileId
`func (o *BrandingProfileOut) UnsetLogoFileId()`

UnsetLogoFileId ensures that no value is present for LogoFileId, not even an explicit nil
### GetPrimaryColor

`func (o *BrandingProfileOut) GetPrimaryColor() string`

GetPrimaryColor returns the PrimaryColor field if non-nil, zero value otherwise.

### GetPrimaryColorOk

`func (o *BrandingProfileOut) GetPrimaryColorOk() (*string, bool)`

GetPrimaryColorOk returns a tuple with the PrimaryColor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrimaryColor

`func (o *BrandingProfileOut) SetPrimaryColor(v string)`

SetPrimaryColor sets PrimaryColor field to given value.


### GetAccentColor

`func (o *BrandingProfileOut) GetAccentColor() string`

GetAccentColor returns the AccentColor field if non-nil, zero value otherwise.

### GetAccentColorOk

`func (o *BrandingProfileOut) GetAccentColorOk() (*string, bool)`

GetAccentColorOk returns a tuple with the AccentColor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccentColor

`func (o *BrandingProfileOut) SetAccentColor(v string)`

SetAccentColor sets AccentColor field to given value.


### GetFontFamily

`func (o *BrandingProfileOut) GetFontFamily() string`

GetFontFamily returns the FontFamily field if non-nil, zero value otherwise.

### GetFontFamilyOk

`func (o *BrandingProfileOut) GetFontFamilyOk() (*string, bool)`

GetFontFamilyOk returns a tuple with the FontFamily field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFontFamily

`func (o *BrandingProfileOut) SetFontFamily(v string)`

SetFontFamily sets FontFamily field to given value.

### HasFontFamily

`func (o *BrandingProfileOut) HasFontFamily() bool`

HasFontFamily returns a boolean if a field has been set.

### SetFontFamilyNil

`func (o *BrandingProfileOut) SetFontFamilyNil(b bool)`

 SetFontFamilyNil sets the value for FontFamily to be an explicit nil

### UnsetFontFamily
`func (o *BrandingProfileOut) UnsetFontFamily()`

UnsetFontFamily ensures that no value is present for FontFamily, not even an explicit nil
### GetHeaderText

`func (o *BrandingProfileOut) GetHeaderText() string`

GetHeaderText returns the HeaderText field if non-nil, zero value otherwise.

### GetHeaderTextOk

`func (o *BrandingProfileOut) GetHeaderTextOk() (*string, bool)`

GetHeaderTextOk returns a tuple with the HeaderText field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHeaderText

`func (o *BrandingProfileOut) SetHeaderText(v string)`

SetHeaderText sets HeaderText field to given value.

### HasHeaderText

`func (o *BrandingProfileOut) HasHeaderText() bool`

HasHeaderText returns a boolean if a field has been set.

### SetHeaderTextNil

`func (o *BrandingProfileOut) SetHeaderTextNil(b bool)`

 SetHeaderTextNil sets the value for HeaderText to be an explicit nil

### UnsetHeaderText
`func (o *BrandingProfileOut) UnsetHeaderText()`

UnsetHeaderText ensures that no value is present for HeaderText, not even an explicit nil
### GetFooterText

`func (o *BrandingProfileOut) GetFooterText() string`

GetFooterText returns the FooterText field if non-nil, zero value otherwise.

### GetFooterTextOk

`func (o *BrandingProfileOut) GetFooterTextOk() (*string, bool)`

GetFooterTextOk returns a tuple with the FooterText field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFooterText

`func (o *BrandingProfileOut) SetFooterText(v string)`

SetFooterText sets FooterText field to given value.


### GetHideInvoicepdfsBranding

`func (o *BrandingProfileOut) GetHideInvoicepdfsBranding() bool`

GetHideInvoicepdfsBranding returns the HideInvoicepdfsBranding field if non-nil, zero value otherwise.

### GetHideInvoicepdfsBrandingOk

`func (o *BrandingProfileOut) GetHideInvoicepdfsBrandingOk() (*bool, bool)`

GetHideInvoicepdfsBrandingOk returns a tuple with the HideInvoicepdfsBranding field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHideInvoicepdfsBranding

`func (o *BrandingProfileOut) SetHideInvoicepdfsBranding(v bool)`

SetHideInvoicepdfsBranding sets HideInvoicepdfsBranding field to given value.


### GetCreatedAt

`func (o *BrandingProfileOut) GetCreatedAt() string`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *BrandingProfileOut) GetCreatedAtOk() (*string, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *BrandingProfileOut) SetCreatedAt(v string)`

SetCreatedAt sets CreatedAt field to given value.


### GetUpdatedAt

`func (o *BrandingProfileOut) GetUpdatedAt() string`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *BrandingProfileOut) GetUpdatedAtOk() (*string, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *BrandingProfileOut) SetUpdatedAt(v string)`

SetUpdatedAt sets UpdatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


