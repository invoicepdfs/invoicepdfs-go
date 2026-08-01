# InvoicePaymentInput

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**BankAccount** | Pointer to [**NullableInvoiceBankAccountInput**](InvoiceBankAccountInput.md) |  | [optional] 
**PaymentUrl** | Pointer to **NullableString** |  | [optional] 
**AcceptedMethods** | Pointer to **[]string** |  | [optional] 
**Instructions** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewInvoicePaymentInput

`func NewInvoicePaymentInput() *InvoicePaymentInput`

NewInvoicePaymentInput instantiates a new InvoicePaymentInput object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewInvoicePaymentInputWithDefaults

`func NewInvoicePaymentInputWithDefaults() *InvoicePaymentInput`

NewInvoicePaymentInputWithDefaults instantiates a new InvoicePaymentInput object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetBankAccount

`func (o *InvoicePaymentInput) GetBankAccount() InvoiceBankAccountInput`

GetBankAccount returns the BankAccount field if non-nil, zero value otherwise.

### GetBankAccountOk

`func (o *InvoicePaymentInput) GetBankAccountOk() (*InvoiceBankAccountInput, bool)`

GetBankAccountOk returns a tuple with the BankAccount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBankAccount

`func (o *InvoicePaymentInput) SetBankAccount(v InvoiceBankAccountInput)`

SetBankAccount sets BankAccount field to given value.

### HasBankAccount

`func (o *InvoicePaymentInput) HasBankAccount() bool`

HasBankAccount returns a boolean if a field has been set.

### SetBankAccountNil

`func (o *InvoicePaymentInput) SetBankAccountNil(b bool)`

 SetBankAccountNil sets the value for BankAccount to be an explicit nil

### UnsetBankAccount
`func (o *InvoicePaymentInput) UnsetBankAccount()`

UnsetBankAccount ensures that no value is present for BankAccount, not even an explicit nil
### GetPaymentUrl

`func (o *InvoicePaymentInput) GetPaymentUrl() string`

GetPaymentUrl returns the PaymentUrl field if non-nil, zero value otherwise.

### GetPaymentUrlOk

`func (o *InvoicePaymentInput) GetPaymentUrlOk() (*string, bool)`

GetPaymentUrlOk returns a tuple with the PaymentUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaymentUrl

`func (o *InvoicePaymentInput) SetPaymentUrl(v string)`

SetPaymentUrl sets PaymentUrl field to given value.

### HasPaymentUrl

`func (o *InvoicePaymentInput) HasPaymentUrl() bool`

HasPaymentUrl returns a boolean if a field has been set.

### SetPaymentUrlNil

`func (o *InvoicePaymentInput) SetPaymentUrlNil(b bool)`

 SetPaymentUrlNil sets the value for PaymentUrl to be an explicit nil

### UnsetPaymentUrl
`func (o *InvoicePaymentInput) UnsetPaymentUrl()`

UnsetPaymentUrl ensures that no value is present for PaymentUrl, not even an explicit nil
### GetAcceptedMethods

`func (o *InvoicePaymentInput) GetAcceptedMethods() []string`

GetAcceptedMethods returns the AcceptedMethods field if non-nil, zero value otherwise.

### GetAcceptedMethodsOk

`func (o *InvoicePaymentInput) GetAcceptedMethodsOk() (*[]string, bool)`

GetAcceptedMethodsOk returns a tuple with the AcceptedMethods field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAcceptedMethods

`func (o *InvoicePaymentInput) SetAcceptedMethods(v []string)`

SetAcceptedMethods sets AcceptedMethods field to given value.

### HasAcceptedMethods

`func (o *InvoicePaymentInput) HasAcceptedMethods() bool`

HasAcceptedMethods returns a boolean if a field has been set.

### GetInstructions

`func (o *InvoicePaymentInput) GetInstructions() string`

GetInstructions returns the Instructions field if non-nil, zero value otherwise.

### GetInstructionsOk

`func (o *InvoicePaymentInput) GetInstructionsOk() (*string, bool)`

GetInstructionsOk returns a tuple with the Instructions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInstructions

`func (o *InvoicePaymentInput) SetInstructions(v string)`

SetInstructions sets Instructions field to given value.

### HasInstructions

`func (o *InvoicePaymentInput) HasInstructions() bool`

HasInstructions returns a boolean if a field has been set.

### SetInstructionsNil

`func (o *InvoicePaymentInput) SetInstructionsNil(b bool)`

 SetInstructionsNil sets the value for Instructions to be an explicit nil

### UnsetInstructions
`func (o *InvoicePaymentInput) UnsetInstructions()`

UnsetInstructions ensures that no value is present for Instructions, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


