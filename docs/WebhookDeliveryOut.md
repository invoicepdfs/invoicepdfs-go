# WebhookDeliveryOut

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**EndpointId** | **string** |  | 
**EventId** | **string** |  | 
**EventType** | **string** |  | 
**Status** | **string** |  | 
**HttpStatus** | Pointer to **NullableInt32** |  | [optional] 
**Attempts** | **int32** |  | 
**ErrorMessage** | Pointer to **NullableString** |  | [optional] 
**CreatedAt** | **string** |  | 
**DeliveredAt** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewWebhookDeliveryOut

`func NewWebhookDeliveryOut(id string, endpointId string, eventId string, eventType string, status string, attempts int32, createdAt string, ) *WebhookDeliveryOut`

NewWebhookDeliveryOut instantiates a new WebhookDeliveryOut object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebhookDeliveryOutWithDefaults

`func NewWebhookDeliveryOutWithDefaults() *WebhookDeliveryOut`

NewWebhookDeliveryOutWithDefaults instantiates a new WebhookDeliveryOut object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *WebhookDeliveryOut) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *WebhookDeliveryOut) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *WebhookDeliveryOut) SetId(v string)`

SetId sets Id field to given value.


### GetEndpointId

`func (o *WebhookDeliveryOut) GetEndpointId() string`

GetEndpointId returns the EndpointId field if non-nil, zero value otherwise.

### GetEndpointIdOk

`func (o *WebhookDeliveryOut) GetEndpointIdOk() (*string, bool)`

GetEndpointIdOk returns a tuple with the EndpointId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndpointId

`func (o *WebhookDeliveryOut) SetEndpointId(v string)`

SetEndpointId sets EndpointId field to given value.


### GetEventId

`func (o *WebhookDeliveryOut) GetEventId() string`

GetEventId returns the EventId field if non-nil, zero value otherwise.

### GetEventIdOk

`func (o *WebhookDeliveryOut) GetEventIdOk() (*string, bool)`

GetEventIdOk returns a tuple with the EventId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEventId

`func (o *WebhookDeliveryOut) SetEventId(v string)`

SetEventId sets EventId field to given value.


### GetEventType

`func (o *WebhookDeliveryOut) GetEventType() string`

GetEventType returns the EventType field if non-nil, zero value otherwise.

### GetEventTypeOk

`func (o *WebhookDeliveryOut) GetEventTypeOk() (*string, bool)`

GetEventTypeOk returns a tuple with the EventType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEventType

`func (o *WebhookDeliveryOut) SetEventType(v string)`

SetEventType sets EventType field to given value.


### GetStatus

`func (o *WebhookDeliveryOut) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *WebhookDeliveryOut) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *WebhookDeliveryOut) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetHttpStatus

`func (o *WebhookDeliveryOut) GetHttpStatus() int32`

GetHttpStatus returns the HttpStatus field if non-nil, zero value otherwise.

### GetHttpStatusOk

`func (o *WebhookDeliveryOut) GetHttpStatusOk() (*int32, bool)`

GetHttpStatusOk returns a tuple with the HttpStatus field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHttpStatus

`func (o *WebhookDeliveryOut) SetHttpStatus(v int32)`

SetHttpStatus sets HttpStatus field to given value.

### HasHttpStatus

`func (o *WebhookDeliveryOut) HasHttpStatus() bool`

HasHttpStatus returns a boolean if a field has been set.

### SetHttpStatusNil

`func (o *WebhookDeliveryOut) SetHttpStatusNil(b bool)`

 SetHttpStatusNil sets the value for HttpStatus to be an explicit nil

### UnsetHttpStatus
`func (o *WebhookDeliveryOut) UnsetHttpStatus()`

UnsetHttpStatus ensures that no value is present for HttpStatus, not even an explicit nil
### GetAttempts

`func (o *WebhookDeliveryOut) GetAttempts() int32`

GetAttempts returns the Attempts field if non-nil, zero value otherwise.

### GetAttemptsOk

`func (o *WebhookDeliveryOut) GetAttemptsOk() (*int32, bool)`

GetAttemptsOk returns a tuple with the Attempts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttempts

`func (o *WebhookDeliveryOut) SetAttempts(v int32)`

SetAttempts sets Attempts field to given value.


### GetErrorMessage

`func (o *WebhookDeliveryOut) GetErrorMessage() string`

GetErrorMessage returns the ErrorMessage field if non-nil, zero value otherwise.

### GetErrorMessageOk

`func (o *WebhookDeliveryOut) GetErrorMessageOk() (*string, bool)`

GetErrorMessageOk returns a tuple with the ErrorMessage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrorMessage

`func (o *WebhookDeliveryOut) SetErrorMessage(v string)`

SetErrorMessage sets ErrorMessage field to given value.

### HasErrorMessage

`func (o *WebhookDeliveryOut) HasErrorMessage() bool`

HasErrorMessage returns a boolean if a field has been set.

### SetErrorMessageNil

`func (o *WebhookDeliveryOut) SetErrorMessageNil(b bool)`

 SetErrorMessageNil sets the value for ErrorMessage to be an explicit nil

### UnsetErrorMessage
`func (o *WebhookDeliveryOut) UnsetErrorMessage()`

UnsetErrorMessage ensures that no value is present for ErrorMessage, not even an explicit nil
### GetCreatedAt

`func (o *WebhookDeliveryOut) GetCreatedAt() string`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *WebhookDeliveryOut) GetCreatedAtOk() (*string, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *WebhookDeliveryOut) SetCreatedAt(v string)`

SetCreatedAt sets CreatedAt field to given value.


### GetDeliveredAt

`func (o *WebhookDeliveryOut) GetDeliveredAt() string`

GetDeliveredAt returns the DeliveredAt field if non-nil, zero value otherwise.

### GetDeliveredAtOk

`func (o *WebhookDeliveryOut) GetDeliveredAtOk() (*string, bool)`

GetDeliveredAtOk returns a tuple with the DeliveredAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeliveredAt

`func (o *WebhookDeliveryOut) SetDeliveredAt(v string)`

SetDeliveredAt sets DeliveredAt field to given value.

### HasDeliveredAt

`func (o *WebhookDeliveryOut) HasDeliveredAt() bool`

HasDeliveredAt returns a boolean if a field has been set.

### SetDeliveredAtNil

`func (o *WebhookDeliveryOut) SetDeliveredAtNil(b bool)`

 SetDeliveredAtNil sets the value for DeliveredAt to be an explicit nil

### UnsetDeliveredAt
`func (o *WebhookDeliveryOut) UnsetDeliveredAt()`

UnsetDeliveredAt ensures that no value is present for DeliveredAt, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


