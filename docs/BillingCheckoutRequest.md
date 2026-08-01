# BillingCheckoutRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**PriceId** | **string** | Stripe price ID for the plan | 

## Methods

### NewBillingCheckoutRequest

`func NewBillingCheckoutRequest(priceId string, ) *BillingCheckoutRequest`

NewBillingCheckoutRequest instantiates a new BillingCheckoutRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBillingCheckoutRequestWithDefaults

`func NewBillingCheckoutRequestWithDefaults() *BillingCheckoutRequest`

NewBillingCheckoutRequestWithDefaults instantiates a new BillingCheckoutRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPriceId

`func (o *BillingCheckoutRequest) GetPriceId() string`

GetPriceId returns the PriceId field if non-nil, zero value otherwise.

### GetPriceIdOk

`func (o *BillingCheckoutRequest) GetPriceIdOk() (*string, bool)`

GetPriceIdOk returns a tuple with the PriceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriceId

`func (o *BillingCheckoutRequest) SetPriceId(v string)`

SetPriceId sets PriceId field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


