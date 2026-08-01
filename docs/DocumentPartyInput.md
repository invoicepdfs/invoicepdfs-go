# DocumentPartyInput

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** |  | 
**LegalName** | Pointer to **NullableString** |  | [optional] 
**Email** | Pointer to **NullableString** |  | [optional] 
**Phone** | Pointer to **NullableString** |  | [optional] 
**Website** | Pointer to **NullableString** |  | [optional] 
**TaxId** | Pointer to **NullableString** |  | [optional] 
**RegistrationNumber** | Pointer to **NullableString** |  | [optional] 
**Address** | Pointer to [**NullablePostalAddress**](PostalAddress.md) |  | [optional] 
**BankAccount** | Pointer to [**NullableInvoiceBankAccountInput**](InvoiceBankAccountInput.md) |  | [optional] 

## Methods

### NewDocumentPartyInput

`func NewDocumentPartyInput(name string, ) *DocumentPartyInput`

NewDocumentPartyInput instantiates a new DocumentPartyInput object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDocumentPartyInputWithDefaults

`func NewDocumentPartyInputWithDefaults() *DocumentPartyInput`

NewDocumentPartyInputWithDefaults instantiates a new DocumentPartyInput object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *DocumentPartyInput) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *DocumentPartyInput) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *DocumentPartyInput) SetName(v string)`

SetName sets Name field to given value.


### GetLegalName

`func (o *DocumentPartyInput) GetLegalName() string`

GetLegalName returns the LegalName field if non-nil, zero value otherwise.

### GetLegalNameOk

`func (o *DocumentPartyInput) GetLegalNameOk() (*string, bool)`

GetLegalNameOk returns a tuple with the LegalName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLegalName

`func (o *DocumentPartyInput) SetLegalName(v string)`

SetLegalName sets LegalName field to given value.

### HasLegalName

`func (o *DocumentPartyInput) HasLegalName() bool`

HasLegalName returns a boolean if a field has been set.

### SetLegalNameNil

`func (o *DocumentPartyInput) SetLegalNameNil(b bool)`

 SetLegalNameNil sets the value for LegalName to be an explicit nil

### UnsetLegalName
`func (o *DocumentPartyInput) UnsetLegalName()`

UnsetLegalName ensures that no value is present for LegalName, not even an explicit nil
### GetEmail

`func (o *DocumentPartyInput) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *DocumentPartyInput) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *DocumentPartyInput) SetEmail(v string)`

SetEmail sets Email field to given value.

### HasEmail

`func (o *DocumentPartyInput) HasEmail() bool`

HasEmail returns a boolean if a field has been set.

### SetEmailNil

`func (o *DocumentPartyInput) SetEmailNil(b bool)`

 SetEmailNil sets the value for Email to be an explicit nil

### UnsetEmail
`func (o *DocumentPartyInput) UnsetEmail()`

UnsetEmail ensures that no value is present for Email, not even an explicit nil
### GetPhone

`func (o *DocumentPartyInput) GetPhone() string`

GetPhone returns the Phone field if non-nil, zero value otherwise.

### GetPhoneOk

`func (o *DocumentPartyInput) GetPhoneOk() (*string, bool)`

GetPhoneOk returns a tuple with the Phone field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPhone

`func (o *DocumentPartyInput) SetPhone(v string)`

SetPhone sets Phone field to given value.

### HasPhone

`func (o *DocumentPartyInput) HasPhone() bool`

HasPhone returns a boolean if a field has been set.

### SetPhoneNil

`func (o *DocumentPartyInput) SetPhoneNil(b bool)`

 SetPhoneNil sets the value for Phone to be an explicit nil

### UnsetPhone
`func (o *DocumentPartyInput) UnsetPhone()`

UnsetPhone ensures that no value is present for Phone, not even an explicit nil
### GetWebsite

`func (o *DocumentPartyInput) GetWebsite() string`

GetWebsite returns the Website field if non-nil, zero value otherwise.

### GetWebsiteOk

`func (o *DocumentPartyInput) GetWebsiteOk() (*string, bool)`

GetWebsiteOk returns a tuple with the Website field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebsite

`func (o *DocumentPartyInput) SetWebsite(v string)`

SetWebsite sets Website field to given value.

### HasWebsite

`func (o *DocumentPartyInput) HasWebsite() bool`

HasWebsite returns a boolean if a field has been set.

### SetWebsiteNil

`func (o *DocumentPartyInput) SetWebsiteNil(b bool)`

 SetWebsiteNil sets the value for Website to be an explicit nil

### UnsetWebsite
`func (o *DocumentPartyInput) UnsetWebsite()`

UnsetWebsite ensures that no value is present for Website, not even an explicit nil
### GetTaxId

`func (o *DocumentPartyInput) GetTaxId() string`

GetTaxId returns the TaxId field if non-nil, zero value otherwise.

### GetTaxIdOk

`func (o *DocumentPartyInput) GetTaxIdOk() (*string, bool)`

GetTaxIdOk returns a tuple with the TaxId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTaxId

`func (o *DocumentPartyInput) SetTaxId(v string)`

SetTaxId sets TaxId field to given value.

### HasTaxId

`func (o *DocumentPartyInput) HasTaxId() bool`

HasTaxId returns a boolean if a field has been set.

### SetTaxIdNil

`func (o *DocumentPartyInput) SetTaxIdNil(b bool)`

 SetTaxIdNil sets the value for TaxId to be an explicit nil

### UnsetTaxId
`func (o *DocumentPartyInput) UnsetTaxId()`

UnsetTaxId ensures that no value is present for TaxId, not even an explicit nil
### GetRegistrationNumber

`func (o *DocumentPartyInput) GetRegistrationNumber() string`

GetRegistrationNumber returns the RegistrationNumber field if non-nil, zero value otherwise.

### GetRegistrationNumberOk

`func (o *DocumentPartyInput) GetRegistrationNumberOk() (*string, bool)`

GetRegistrationNumberOk returns a tuple with the RegistrationNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRegistrationNumber

`func (o *DocumentPartyInput) SetRegistrationNumber(v string)`

SetRegistrationNumber sets RegistrationNumber field to given value.

### HasRegistrationNumber

`func (o *DocumentPartyInput) HasRegistrationNumber() bool`

HasRegistrationNumber returns a boolean if a field has been set.

### SetRegistrationNumberNil

`func (o *DocumentPartyInput) SetRegistrationNumberNil(b bool)`

 SetRegistrationNumberNil sets the value for RegistrationNumber to be an explicit nil

### UnsetRegistrationNumber
`func (o *DocumentPartyInput) UnsetRegistrationNumber()`

UnsetRegistrationNumber ensures that no value is present for RegistrationNumber, not even an explicit nil
### GetAddress

`func (o *DocumentPartyInput) GetAddress() PostalAddress`

GetAddress returns the Address field if non-nil, zero value otherwise.

### GetAddressOk

`func (o *DocumentPartyInput) GetAddressOk() (*PostalAddress, bool)`

GetAddressOk returns a tuple with the Address field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddress

`func (o *DocumentPartyInput) SetAddress(v PostalAddress)`

SetAddress sets Address field to given value.

### HasAddress

`func (o *DocumentPartyInput) HasAddress() bool`

HasAddress returns a boolean if a field has been set.

### SetAddressNil

`func (o *DocumentPartyInput) SetAddressNil(b bool)`

 SetAddressNil sets the value for Address to be an explicit nil

### UnsetAddress
`func (o *DocumentPartyInput) UnsetAddress()`

UnsetAddress ensures that no value is present for Address, not even an explicit nil
### GetBankAccount

`func (o *DocumentPartyInput) GetBankAccount() InvoiceBankAccountInput`

GetBankAccount returns the BankAccount field if non-nil, zero value otherwise.

### GetBankAccountOk

`func (o *DocumentPartyInput) GetBankAccountOk() (*InvoiceBankAccountInput, bool)`

GetBankAccountOk returns a tuple with the BankAccount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBankAccount

`func (o *DocumentPartyInput) SetBankAccount(v InvoiceBankAccountInput)`

SetBankAccount sets BankAccount field to given value.

### HasBankAccount

`func (o *DocumentPartyInput) HasBankAccount() bool`

HasBankAccount returns a boolean if a field has been set.

### SetBankAccountNil

`func (o *DocumentPartyInput) SetBankAccountNil(b bool)`

 SetBankAccountNil sets the value for BankAccount to be an explicit nil

### UnsetBankAccount
`func (o *DocumentPartyInput) UnsetBankAccount()`

UnsetBankAccount ensures that no value is present for BankAccount, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


