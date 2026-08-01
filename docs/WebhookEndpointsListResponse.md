# WebhookEndpointsListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Data** | [**[]WebhookEndpointOut**](WebhookEndpointOut.md) |  | 
**Pagination** | Pointer to [**CursorPagination**](CursorPagination.md) |  | [optional] 

## Methods

### NewWebhookEndpointsListResponse

`func NewWebhookEndpointsListResponse(data []WebhookEndpointOut, ) *WebhookEndpointsListResponse`

NewWebhookEndpointsListResponse instantiates a new WebhookEndpointsListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebhookEndpointsListResponseWithDefaults

`func NewWebhookEndpointsListResponseWithDefaults() *WebhookEndpointsListResponse`

NewWebhookEndpointsListResponseWithDefaults instantiates a new WebhookEndpointsListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetData

`func (o *WebhookEndpointsListResponse) GetData() []WebhookEndpointOut`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *WebhookEndpointsListResponse) GetDataOk() (*[]WebhookEndpointOut, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *WebhookEndpointsListResponse) SetData(v []WebhookEndpointOut)`

SetData sets Data field to given value.


### GetPagination

`func (o *WebhookEndpointsListResponse) GetPagination() CursorPagination`

GetPagination returns the Pagination field if non-nil, zero value otherwise.

### GetPaginationOk

`func (o *WebhookEndpointsListResponse) GetPaginationOk() (*CursorPagination, bool)`

GetPaginationOk returns a tuple with the Pagination field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPagination

`func (o *WebhookEndpointsListResponse) SetPagination(v CursorPagination)`

SetPagination sets Pagination field to given value.

### HasPagination

`func (o *WebhookEndpointsListResponse) HasPagination() bool`

HasPagination returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


