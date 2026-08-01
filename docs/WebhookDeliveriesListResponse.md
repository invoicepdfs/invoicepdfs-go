# WebhookDeliveriesListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Data** | [**[]WebhookDeliveryOut**](WebhookDeliveryOut.md) |  | 
**Pagination** | Pointer to [**CursorPagination**](CursorPagination.md) |  | [optional] 

## Methods

### NewWebhookDeliveriesListResponse

`func NewWebhookDeliveriesListResponse(data []WebhookDeliveryOut, ) *WebhookDeliveriesListResponse`

NewWebhookDeliveriesListResponse instantiates a new WebhookDeliveriesListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebhookDeliveriesListResponseWithDefaults

`func NewWebhookDeliveriesListResponseWithDefaults() *WebhookDeliveriesListResponse`

NewWebhookDeliveriesListResponseWithDefaults instantiates a new WebhookDeliveriesListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetData

`func (o *WebhookDeliveriesListResponse) GetData() []WebhookDeliveryOut`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *WebhookDeliveriesListResponse) GetDataOk() (*[]WebhookDeliveryOut, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *WebhookDeliveriesListResponse) SetData(v []WebhookDeliveryOut)`

SetData sets Data field to given value.


### GetPagination

`func (o *WebhookDeliveriesListResponse) GetPagination() CursorPagination`

GetPagination returns the Pagination field if non-nil, zero value otherwise.

### GetPaginationOk

`func (o *WebhookDeliveriesListResponse) GetPaginationOk() (*CursorPagination, bool)`

GetPaginationOk returns a tuple with the Pagination field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPagination

`func (o *WebhookDeliveriesListResponse) SetPagination(v CursorPagination)`

SetPagination sets Pagination field to given value.

### HasPagination

`func (o *WebhookDeliveriesListResponse) HasPagination() bool`

HasPagination returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


