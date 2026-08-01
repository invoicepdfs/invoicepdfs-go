# DocumentOutputOptions

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Format** | Pointer to **string** |  | [optional] [default to "pdf"]
**Delivery** | Pointer to **string** |  | [optional] [default to "url"]
**ExpiresIn** | Pointer to **int32** |  | [optional] [default to 3600]

## Methods

### NewDocumentOutputOptions

`func NewDocumentOutputOptions() *DocumentOutputOptions`

NewDocumentOutputOptions instantiates a new DocumentOutputOptions object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDocumentOutputOptionsWithDefaults

`func NewDocumentOutputOptionsWithDefaults() *DocumentOutputOptions`

NewDocumentOutputOptionsWithDefaults instantiates a new DocumentOutputOptions object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetFormat

`func (o *DocumentOutputOptions) GetFormat() string`

GetFormat returns the Format field if non-nil, zero value otherwise.

### GetFormatOk

`func (o *DocumentOutputOptions) GetFormatOk() (*string, bool)`

GetFormatOk returns a tuple with the Format field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFormat

`func (o *DocumentOutputOptions) SetFormat(v string)`

SetFormat sets Format field to given value.

### HasFormat

`func (o *DocumentOutputOptions) HasFormat() bool`

HasFormat returns a boolean if a field has been set.

### GetDelivery

`func (o *DocumentOutputOptions) GetDelivery() string`

GetDelivery returns the Delivery field if non-nil, zero value otherwise.

### GetDeliveryOk

`func (o *DocumentOutputOptions) GetDeliveryOk() (*string, bool)`

GetDeliveryOk returns a tuple with the Delivery field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDelivery

`func (o *DocumentOutputOptions) SetDelivery(v string)`

SetDelivery sets Delivery field to given value.

### HasDelivery

`func (o *DocumentOutputOptions) HasDelivery() bool`

HasDelivery returns a boolean if a field has been set.

### GetExpiresIn

`func (o *DocumentOutputOptions) GetExpiresIn() int32`

GetExpiresIn returns the ExpiresIn field if non-nil, zero value otherwise.

### GetExpiresInOk

`func (o *DocumentOutputOptions) GetExpiresInOk() (*int32, bool)`

GetExpiresInOk returns a tuple with the ExpiresIn field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresIn

`func (o *DocumentOutputOptions) SetExpiresIn(v int32)`

SetExpiresIn sets ExpiresIn field to given value.

### HasExpiresIn

`func (o *DocumentOutputOptions) HasExpiresIn() bool`

HasExpiresIn returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


