# DocumentsListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Data** | [**[]DocumentOut**](DocumentOut.md) |  | 
**Pagination** | Pointer to [**CursorPagination**](CursorPagination.md) |  | [optional] 

## Methods

### NewDocumentsListResponse

`func NewDocumentsListResponse(data []DocumentOut, ) *DocumentsListResponse`

NewDocumentsListResponse instantiates a new DocumentsListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDocumentsListResponseWithDefaults

`func NewDocumentsListResponseWithDefaults() *DocumentsListResponse`

NewDocumentsListResponseWithDefaults instantiates a new DocumentsListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetData

`func (o *DocumentsListResponse) GetData() []DocumentOut`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *DocumentsListResponse) GetDataOk() (*[]DocumentOut, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *DocumentsListResponse) SetData(v []DocumentOut)`

SetData sets Data field to given value.


### GetPagination

`func (o *DocumentsListResponse) GetPagination() CursorPagination`

GetPagination returns the Pagination field if non-nil, zero value otherwise.

### GetPaginationOk

`func (o *DocumentsListResponse) GetPaginationOk() (*CursorPagination, bool)`

GetPaginationOk returns a tuple with the Pagination field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPagination

`func (o *DocumentsListResponse) SetPagination(v CursorPagination)`

SetPagination sets Pagination field to given value.

### HasPagination

`func (o *DocumentsListResponse) HasPagination() bool`

HasPagination returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


