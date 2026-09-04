# BusinessProfilePatch

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**LegalName** | Pointer to **string** |  | [optional] 
**DisplayName** | Pointer to **NullableString** |  | [optional] 
**Email** | Pointer to **NullableString** |  | [optional] 
**Phone** | Pointer to **NullableString** |  | [optional] 
**Website** | Pointer to **NullableString** |  | [optional] 
**TaxId** | Pointer to **NullableString** |  | [optional] 
**Address** | Pointer to [**NullablePostalAddress**](PostalAddress.md) |  | [optional] 
**DefaultCurrency** | Pointer to **NullableString** |  | [optional] 
**DefaultLocale** | Pointer to **NullableString** |  | [optional] 
**DefaultTimezone** | Pointer to **NullableString** |  | [optional] 
**LogoFileId** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewBusinessProfilePatch

`func NewBusinessProfilePatch() *BusinessProfilePatch`

NewBusinessProfilePatch instantiates a new BusinessProfilePatch object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBusinessProfilePatchWithDefaults

`func NewBusinessProfilePatchWithDefaults() *BusinessProfilePatch`

NewBusinessProfilePatchWithDefaults instantiates a new BusinessProfilePatch object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLegalName

`func (o *BusinessProfilePatch) GetLegalName() string`

GetLegalName returns the LegalName field if non-nil, zero value otherwise.

### GetLegalNameOk

`func (o *BusinessProfilePatch) GetLegalNameOk() (*string, bool)`

GetLegalNameOk returns a tuple with the LegalName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLegalName

`func (o *BusinessProfilePatch) SetLegalName(v string)`

SetLegalName sets LegalName field to given value.

### HasLegalName

`func (o *BusinessProfilePatch) HasLegalName() bool`

HasLegalName returns a boolean if a field has been set.

### GetDisplayName

`func (o *BusinessProfilePatch) GetDisplayName() string`

GetDisplayName returns the DisplayName field if non-nil, zero value otherwise.

### GetDisplayNameOk

`func (o *BusinessProfilePatch) GetDisplayNameOk() (*string, bool)`

GetDisplayNameOk returns a tuple with the DisplayName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayName

`func (o *BusinessProfilePatch) SetDisplayName(v string)`

SetDisplayName sets DisplayName field to given value.

### HasDisplayName

`func (o *BusinessProfilePatch) HasDisplayName() bool`

HasDisplayName returns a boolean if a field has been set.

### SetDisplayNameNil

`func (o *BusinessProfilePatch) SetDisplayNameNil(b bool)`

 SetDisplayNameNil sets the value for DisplayName to be an explicit nil

### UnsetDisplayName
`func (o *BusinessProfilePatch) UnsetDisplayName()`

UnsetDisplayName ensures that no value is present for DisplayName, not even an explicit nil
### GetEmail

`func (o *BusinessProfilePatch) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *BusinessProfilePatch) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *BusinessProfilePatch) SetEmail(v string)`

SetEmail sets Email field to given value.

### HasEmail

`func (o *BusinessProfilePatch) HasEmail() bool`

HasEmail returns a boolean if a field has been set.

### SetEmailNil

`func (o *BusinessProfilePatch) SetEmailNil(b bool)`

 SetEmailNil sets the value for Email to be an explicit nil

### UnsetEmail
`func (o *BusinessProfilePatch) UnsetEmail()`

UnsetEmail ensures that no value is present for Email, not even an explicit nil
### GetPhone

`func (o *BusinessProfilePatch) GetPhone() string`

GetPhone returns the Phone field if non-nil, zero value otherwise.

### GetPhoneOk

`func (o *BusinessProfilePatch) GetPhoneOk() (*string, bool)`

GetPhoneOk returns a tuple with the Phone field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPhone

`func (o *BusinessProfilePatch) SetPhone(v string)`

SetPhone sets Phone field to given value.

### HasPhone

`func (o *BusinessProfilePatch) HasPhone() bool`

HasPhone returns a boolean if a field has been set.

### SetPhoneNil

`func (o *BusinessProfilePatch) SetPhoneNil(b bool)`

 SetPhoneNil sets the value for Phone to be an explicit nil

### UnsetPhone
`func (o *BusinessProfilePatch) UnsetPhone()`

UnsetPhone ensures that no value is present for Phone, not even an explicit nil
### GetWebsite

`func (o *BusinessProfilePatch) GetWebsite() string`

GetWebsite returns the Website field if non-nil, zero value otherwise.

### GetWebsiteOk

`func (o *BusinessProfilePatch) GetWebsiteOk() (*string, bool)`

GetWebsiteOk returns a tuple with the Website field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebsite

`func (o *BusinessProfilePatch) SetWebsite(v string)`

SetWebsite sets Website field to given value.

### HasWebsite

`func (o *BusinessProfilePatch) HasWebsite() bool`

HasWebsite returns a boolean if a field has been set.

### SetWebsiteNil

`func (o *BusinessProfilePatch) SetWebsiteNil(b bool)`

 SetWebsiteNil sets the value for Website to be an explicit nil

### UnsetWebsite
`func (o *BusinessProfilePatch) UnsetWebsite()`

UnsetWebsite ensures that no value is present for Website, not even an explicit nil
### GetTaxId

`func (o *BusinessProfilePatch) GetTaxId() string`

GetTaxId returns the TaxId field if non-nil, zero value otherwise.

### GetTaxIdOk

`func (o *BusinessProfilePatch) GetTaxIdOk() (*string, bool)`

GetTaxIdOk returns a tuple with the TaxId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTaxId

`func (o *BusinessProfilePatch) SetTaxId(v string)`

SetTaxId sets TaxId field to given value.

### HasTaxId

`func (o *BusinessProfilePatch) HasTaxId() bool`

HasTaxId returns a boolean if a field has been set.

### SetTaxIdNil

`func (o *BusinessProfilePatch) SetTaxIdNil(b bool)`

 SetTaxIdNil sets the value for TaxId to be an explicit nil

### UnsetTaxId
`func (o *BusinessProfilePatch) UnsetTaxId()`

UnsetTaxId ensures that no value is present for TaxId, not even an explicit nil
### GetAddress

`func (o *BusinessProfilePatch) GetAddress() PostalAddress`

GetAddress returns the Address field if non-nil, zero value otherwise.

### GetAddressOk

`func (o *BusinessProfilePatch) GetAddressOk() (*PostalAddress, bool)`

GetAddressOk returns a tuple with the Address field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddress

`func (o *BusinessProfilePatch) SetAddress(v PostalAddress)`

SetAddress sets Address field to given value.

### HasAddress

`func (o *BusinessProfilePatch) HasAddress() bool`

HasAddress returns a boolean if a field has been set.

### SetAddressNil

`func (o *BusinessProfilePatch) SetAddressNil(b bool)`

 SetAddressNil sets the value for Address to be an explicit nil

### UnsetAddress
`func (o *BusinessProfilePatch) UnsetAddress()`

UnsetAddress ensures that no value is present for Address, not even an explicit nil
### GetDefaultCurrency

`func (o *BusinessProfilePatch) GetDefaultCurrency() string`

GetDefaultCurrency returns the DefaultCurrency field if non-nil, zero value otherwise.

### GetDefaultCurrencyOk

`func (o *BusinessProfilePatch) GetDefaultCurrencyOk() (*string, bool)`

GetDefaultCurrencyOk returns a tuple with the DefaultCurrency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultCurrency

`func (o *BusinessProfilePatch) SetDefaultCurrency(v string)`

SetDefaultCurrency sets DefaultCurrency field to given value.

### HasDefaultCurrency

`func (o *BusinessProfilePatch) HasDefaultCurrency() bool`

HasDefaultCurrency returns a boolean if a field has been set.

### SetDefaultCurrencyNil

`func (o *BusinessProfilePatch) SetDefaultCurrencyNil(b bool)`

 SetDefaultCurrencyNil sets the value for DefaultCurrency to be an explicit nil

### UnsetDefaultCurrency
`func (o *BusinessProfilePatch) UnsetDefaultCurrency()`

UnsetDefaultCurrency ensures that no value is present for DefaultCurrency, not even an explicit nil
### GetDefaultLocale

`func (o *BusinessProfilePatch) GetDefaultLocale() string`

GetDefaultLocale returns the DefaultLocale field if non-nil, zero value otherwise.

### GetDefaultLocaleOk

`func (o *BusinessProfilePatch) GetDefaultLocaleOk() (*string, bool)`

GetDefaultLocaleOk returns a tuple with the DefaultLocale field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultLocale

`func (o *BusinessProfilePatch) SetDefaultLocale(v string)`

SetDefaultLocale sets DefaultLocale field to given value.

### HasDefaultLocale

`func (o *BusinessProfilePatch) HasDefaultLocale() bool`

HasDefaultLocale returns a boolean if a field has been set.

### SetDefaultLocaleNil

`func (o *BusinessProfilePatch) SetDefaultLocaleNil(b bool)`

 SetDefaultLocaleNil sets the value for DefaultLocale to be an explicit nil

### UnsetDefaultLocale
`func (o *BusinessProfilePatch) UnsetDefaultLocale()`

UnsetDefaultLocale ensures that no value is present for DefaultLocale, not even an explicit nil
### GetDefaultTimezone

`func (o *BusinessProfilePatch) GetDefaultTimezone() string`

GetDefaultTimezone returns the DefaultTimezone field if non-nil, zero value otherwise.

### GetDefaultTimezoneOk

`func (o *BusinessProfilePatch) GetDefaultTimezoneOk() (*string, bool)`

GetDefaultTimezoneOk returns a tuple with the DefaultTimezone field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultTimezone

`func (o *BusinessProfilePatch) SetDefaultTimezone(v string)`

SetDefaultTimezone sets DefaultTimezone field to given value.

### HasDefaultTimezone

`func (o *BusinessProfilePatch) HasDefaultTimezone() bool`

HasDefaultTimezone returns a boolean if a field has been set.

### SetDefaultTimezoneNil

`func (o *BusinessProfilePatch) SetDefaultTimezoneNil(b bool)`

 SetDefaultTimezoneNil sets the value for DefaultTimezone to be an explicit nil

### UnsetDefaultTimezone
`func (o *BusinessProfilePatch) UnsetDefaultTimezone()`

UnsetDefaultTimezone ensures that no value is present for DefaultTimezone, not even an explicit nil
### GetLogoFileId

`func (o *BusinessProfilePatch) GetLogoFileId() string`

GetLogoFileId returns the LogoFileId field if non-nil, zero value otherwise.

### GetLogoFileIdOk

`func (o *BusinessProfilePatch) GetLogoFileIdOk() (*string, bool)`

GetLogoFileIdOk returns a tuple with the LogoFileId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogoFileId

`func (o *BusinessProfilePatch) SetLogoFileId(v string)`

SetLogoFileId sets LogoFileId field to given value.

### HasLogoFileId

`func (o *BusinessProfilePatch) HasLogoFileId() bool`

HasLogoFileId returns a boolean if a field has been set.

### SetLogoFileIdNil

`func (o *BusinessProfilePatch) SetLogoFileIdNil(b bool)`

 SetLogoFileIdNil sets the value for LogoFileId to be an explicit nil

### UnsetLogoFileId
`func (o *BusinessProfilePatch) UnsetLogoFileId()`

UnsetLogoFileId ensures that no value is present for LogoFileId, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


