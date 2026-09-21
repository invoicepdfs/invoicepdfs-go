# WebhookEndpointCreatedOut

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Url** | **string** |  | 
**Description** | Pointer to **NullableString** |  | [optional] 
**Events** | **[]string** |  | 
**IsActive** | **bool** |  | 
**CreatedAt** | **string** |  | 
**UpdatedAt** | **string** |  | 
**Secret** | **string** |  | 

## Methods

### NewWebhookEndpointCreatedOut

`func NewWebhookEndpointCreatedOut(id string, url string, events []string, isActive bool, createdAt string, updatedAt string, secret string, ) *WebhookEndpointCreatedOut`

NewWebhookEndpointCreatedOut instantiates a new WebhookEndpointCreatedOut object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebhookEndpointCreatedOutWithDefaults

`func NewWebhookEndpointCreatedOutWithDefaults() *WebhookEndpointCreatedOut`

NewWebhookEndpointCreatedOutWithDefaults instantiates a new WebhookEndpointCreatedOut object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *WebhookEndpointCreatedOut) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *WebhookEndpointCreatedOut) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *WebhookEndpointCreatedOut) SetId(v string)`

SetId sets Id field to given value.


### GetUrl

`func (o *WebhookEndpointCreatedOut) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *WebhookEndpointCreatedOut) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *WebhookEndpointCreatedOut) SetUrl(v string)`

SetUrl sets Url field to given value.


### GetDescription

`func (o *WebhookEndpointCreatedOut) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *WebhookEndpointCreatedOut) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *WebhookEndpointCreatedOut) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *WebhookEndpointCreatedOut) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *WebhookEndpointCreatedOut) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *WebhookEndpointCreatedOut) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetEvents

`func (o *WebhookEndpointCreatedOut) GetEvents() []string`

GetEvents returns the Events field if non-nil, zero value otherwise.

### GetEventsOk

`func (o *WebhookEndpointCreatedOut) GetEventsOk() (*[]string, bool)`

GetEventsOk returns a tuple with the Events field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEvents

`func (o *WebhookEndpointCreatedOut) SetEvents(v []string)`

SetEvents sets Events field to given value.


### GetIsActive

`func (o *WebhookEndpointCreatedOut) GetIsActive() bool`

GetIsActive returns the IsActive field if non-nil, zero value otherwise.

### GetIsActiveOk

`func (o *WebhookEndpointCreatedOut) GetIsActiveOk() (*bool, bool)`

GetIsActiveOk returns a tuple with the IsActive field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsActive

`func (o *WebhookEndpointCreatedOut) SetIsActive(v bool)`

SetIsActive sets IsActive field to given value.


### GetCreatedAt

`func (o *WebhookEndpointCreatedOut) GetCreatedAt() string`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *WebhookEndpointCreatedOut) GetCreatedAtOk() (*string, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *WebhookEndpointCreatedOut) SetCreatedAt(v string)`

SetCreatedAt sets CreatedAt field to given value.


### GetUpdatedAt

`func (o *WebhookEndpointCreatedOut) GetUpdatedAt() string`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *WebhookEndpointCreatedOut) GetUpdatedAtOk() (*string, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *WebhookEndpointCreatedOut) SetUpdatedAt(v string)`

SetUpdatedAt sets UpdatedAt field to given value.


### GetSecret

`func (o *WebhookEndpointCreatedOut) GetSecret() string`

GetSecret returns the Secret field if non-nil, zero value otherwise.

### GetSecretOk

`func (o *WebhookEndpointCreatedOut) GetSecretOk() (*string, bool)`

GetSecretOk returns a tuple with the Secret field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecret

`func (o *WebhookEndpointCreatedOut) SetSecret(v string)`

SetSecret sets Secret field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


