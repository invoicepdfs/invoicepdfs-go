# BusinessProfileOut

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**LegalName** | **string** |  | 
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
**Id** | **string** |  | 
**CreatedAt** | **string** |  | 
**UpdatedAt** | **string** |  | 

## Methods

### NewBusinessProfileOut

`func NewBusinessProfileOut(legalName string, id string, createdAt string, updatedAt string, ) *BusinessProfileOut`

NewBusinessProfileOut instantiates a new BusinessProfileOut object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBusinessProfileOutWithDefaults

`func NewBusinessProfileOutWithDefaults() *BusinessProfileOut`

NewBusinessProfileOutWithDefaults instantiates a new BusinessProfileOut object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLegalName

`func (o *BusinessProfileOut) GetLegalName() string`

GetLegalName returns the LegalName field if non-nil, zero value otherwise.

### GetLegalNameOk

`func (o *BusinessProfileOut) GetLegalNameOk() (*string, bool)`

GetLegalNameOk returns a tuple with the LegalName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLegalName

`func (o *BusinessProfileOut) SetLegalName(v string)`

SetLegalName sets LegalName field to given value.


### GetDisplayName

`func (o *BusinessProfileOut) GetDisplayName() string`

GetDisplayName returns the DisplayName field if non-nil, zero value otherwise.

### GetDisplayNameOk

`func (o *BusinessProfileOut) GetDisplayNameOk() (*string, bool)`

GetDisplayNameOk returns a tuple with the DisplayName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayName

`func (o *BusinessProfileOut) SetDisplayName(v string)`

SetDisplayName sets DisplayName field to given value.

### HasDisplayName

`func (o *BusinessProfileOut) HasDisplayName() bool`

HasDisplayName returns a boolean if a field has been set.

### SetDisplayNameNil

`func (o *BusinessProfileOut) SetDisplayNameNil(b bool)`

 SetDisplayNameNil sets the value for DisplayName to be an explicit nil

### UnsetDisplayName
`func (o *BusinessProfileOut) UnsetDisplayName()`

UnsetDisplayName ensures that no value is present for DisplayName, not even an explicit nil
### GetEmail

`func (o *BusinessProfileOut) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *BusinessProfileOut) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *BusinessProfileOut) SetEmail(v string)`

SetEmail sets Email field to given value.

### HasEmail

`func (o *BusinessProfileOut) HasEmail() bool`

HasEmail returns a boolean if a field has been set.

### SetEmailNil

`func (o *BusinessProfileOut) SetEmailNil(b bool)`

 SetEmailNil sets the value for Email to be an explicit nil

### UnsetEmail
`func (o *BusinessProfileOut) UnsetEmail()`

UnsetEmail ensures that no value is present for Email, not even an explicit nil
### GetPhone

`func (o *BusinessProfileOut) GetPhone() string`

GetPhone returns the Phone field if non-nil, zero value otherwise.

### GetPhoneOk

`func (o *BusinessProfileOut) GetPhoneOk() (*string, bool)`

GetPhoneOk returns a tuple with the Phone field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPhone

`func (o *BusinessProfileOut) SetPhone(v string)`

SetPhone sets Phone field to given value.

### HasPhone

`func (o *BusinessProfileOut) HasPhone() bool`

HasPhone returns a boolean if a field has been set.

### SetPhoneNil

`func (o *BusinessProfileOut) SetPhoneNil(b bool)`

 SetPhoneNil sets the value for Phone to be an explicit nil

### UnsetPhone
`func (o *BusinessProfileOut) UnsetPhone()`

UnsetPhone ensures that no value is present for Phone, not even an explicit nil
### GetWebsite

`func (o *BusinessProfileOut) GetWebsite() string`

GetWebsite returns the Website field if non-nil, zero value otherwise.

### GetWebsiteOk

`func (o *BusinessProfileOut) GetWebsiteOk() (*string, bool)`

GetWebsiteOk returns a tuple with the Website field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebsite

`func (o *BusinessProfileOut) SetWebsite(v string)`

SetWebsite sets Website field to given value.

### HasWebsite

`func (o *BusinessProfileOut) HasWebsite() bool`

HasWebsite returns a boolean if a field has been set.

### SetWebsiteNil

`func (o *BusinessProfileOut) SetWebsiteNil(b bool)`

 SetWebsiteNil sets the value for Website to be an explicit nil

### UnsetWebsite
`func (o *BusinessProfileOut) UnsetWebsite()`

UnsetWebsite ensures that no value is present for Website, not even an explicit nil
### GetTaxId

`func (o *BusinessProfileOut) GetTaxId() string`

GetTaxId returns the TaxId field if non-nil, zero value otherwise.

### GetTaxIdOk

`func (o *BusinessProfileOut) GetTaxIdOk() (*string, bool)`

GetTaxIdOk returns a tuple with the TaxId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTaxId

`func (o *BusinessProfileOut) SetTaxId(v string)`

SetTaxId sets TaxId field to given value.

### HasTaxId

`func (o *BusinessProfileOut) HasTaxId() bool`

HasTaxId returns a boolean if a field has been set.

### SetTaxIdNil

`func (o *BusinessProfileOut) SetTaxIdNil(b bool)`

 SetTaxIdNil sets the value for TaxId to be an explicit nil

### UnsetTaxId
`func (o *BusinessProfileOut) UnsetTaxId()`

UnsetTaxId ensures that no value is present for TaxId, not even an explicit nil
### GetAddress

`func (o *BusinessProfileOut) GetAddress() PostalAddress`

GetAddress returns the Address field if non-nil, zero value otherwise.

### GetAddressOk

`func (o *BusinessProfileOut) GetAddressOk() (*PostalAddress, bool)`

GetAddressOk returns a tuple with the Address field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddress

`func (o *BusinessProfileOut) SetAddress(v PostalAddress)`

SetAddress sets Address field to given value.

### HasAddress

`func (o *BusinessProfileOut) HasAddress() bool`

HasAddress returns a boolean if a field has been set.

### SetAddressNil

`func (o *BusinessProfileOut) SetAddressNil(b bool)`

 SetAddressNil sets the value for Address to be an explicit nil

### UnsetAddress
`func (o *BusinessProfileOut) UnsetAddress()`

UnsetAddress ensures that no value is present for Address, not even an explicit nil
### GetDefaultCurrency

`func (o *BusinessProfileOut) GetDefaultCurrency() string`

GetDefaultCurrency returns the DefaultCurrency field if non-nil, zero value otherwise.

### GetDefaultCurrencyOk

`func (o *BusinessProfileOut) GetDefaultCurrencyOk() (*string, bool)`

GetDefaultCurrencyOk returns a tuple with the DefaultCurrency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultCurrency

`func (o *BusinessProfileOut) SetDefaultCurrency(v string)`

SetDefaultCurrency sets DefaultCurrency field to given value.

### HasDefaultCurrency

`func (o *BusinessProfileOut) HasDefaultCurrency() bool`

HasDefaultCurrency returns a boolean if a field has been set.

### SetDefaultCurrencyNil

`func (o *BusinessProfileOut) SetDefaultCurrencyNil(b bool)`

 SetDefaultCurrencyNil sets the value for DefaultCurrency to be an explicit nil

### UnsetDefaultCurrency
`func (o *BusinessProfileOut) UnsetDefaultCurrency()`

UnsetDefaultCurrency ensures that no value is present for DefaultCurrency, not even an explicit nil
### GetDefaultLocale

`func (o *BusinessProfileOut) GetDefaultLocale() string`

GetDefaultLocale returns the DefaultLocale field if non-nil, zero value otherwise.

### GetDefaultLocaleOk

`func (o *BusinessProfileOut) GetDefaultLocaleOk() (*string, bool)`

GetDefaultLocaleOk returns a tuple with the DefaultLocale field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultLocale

`func (o *BusinessProfileOut) SetDefaultLocale(v string)`

SetDefaultLocale sets DefaultLocale field to given value.

### HasDefaultLocale

`func (o *BusinessProfileOut) HasDefaultLocale() bool`

HasDefaultLocale returns a boolean if a field has been set.

### SetDefaultLocaleNil

`func (o *BusinessProfileOut) SetDefaultLocaleNil(b bool)`

 SetDefaultLocaleNil sets the value for DefaultLocale to be an explicit nil

### UnsetDefaultLocale
`func (o *BusinessProfileOut) UnsetDefaultLocale()`

UnsetDefaultLocale ensures that no value is present for DefaultLocale, not even an explicit nil
### GetDefaultTimezone

`func (o *BusinessProfileOut) GetDefaultTimezone() string`

GetDefaultTimezone returns the DefaultTimezone field if non-nil, zero value otherwise.

### GetDefaultTimezoneOk

`func (o *BusinessProfileOut) GetDefaultTimezoneOk() (*string, bool)`

GetDefaultTimezoneOk returns a tuple with the DefaultTimezone field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultTimezone

`func (o *BusinessProfileOut) SetDefaultTimezone(v string)`

SetDefaultTimezone sets DefaultTimezone field to given value.

### HasDefaultTimezone

`func (o *BusinessProfileOut) HasDefaultTimezone() bool`

HasDefaultTimezone returns a boolean if a field has been set.

### SetDefaultTimezoneNil

`func (o *BusinessProfileOut) SetDefaultTimezoneNil(b bool)`

 SetDefaultTimezoneNil sets the value for DefaultTimezone to be an explicit nil

### UnsetDefaultTimezone
`func (o *BusinessProfileOut) UnsetDefaultTimezone()`

UnsetDefaultTimezone ensures that no value is present for DefaultTimezone, not even an explicit nil
### GetLogoFileId

`func (o *BusinessProfileOut) GetLogoFileId() string`

GetLogoFileId returns the LogoFileId field if non-nil, zero value otherwise.

### GetLogoFileIdOk

`func (o *BusinessProfileOut) GetLogoFileIdOk() (*string, bool)`

GetLogoFileIdOk returns a tuple with the LogoFileId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogoFileId

`func (o *BusinessProfileOut) SetLogoFileId(v string)`

SetLogoFileId sets LogoFileId field to given value.

### HasLogoFileId

`func (o *BusinessProfileOut) HasLogoFileId() bool`

HasLogoFileId returns a boolean if a field has been set.

### SetLogoFileIdNil

`func (o *BusinessProfileOut) SetLogoFileIdNil(b bool)`

 SetLogoFileIdNil sets the value for LogoFileId to be an explicit nil

### UnsetLogoFileId
`func (o *BusinessProfileOut) UnsetLogoFileId()`

UnsetLogoFileId ensures that no value is present for LogoFileId, not even an explicit nil
### GetId

`func (o *BusinessProfileOut) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *BusinessProfileOut) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *BusinessProfileOut) SetId(v string)`

SetId sets Id field to given value.


### GetCreatedAt

`func (o *BusinessProfileOut) GetCreatedAt() string`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *BusinessProfileOut) GetCreatedAtOk() (*string, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *BusinessProfileOut) SetCreatedAt(v string)`

SetCreatedAt sets CreatedAt field to given value.


### GetUpdatedAt

`func (o *BusinessProfileOut) GetUpdatedAt() string`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *BusinessProfileOut) GetUpdatedAtOk() (*string, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *BusinessProfileOut) SetUpdatedAt(v string)`

SetUpdatedAt sets UpdatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


