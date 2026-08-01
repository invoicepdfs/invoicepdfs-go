# BatchesListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Data** | [**[]BatchOut**](BatchOut.md) |  | 
**Pagination** | Pointer to [**CursorPagination**](CursorPagination.md) |  | [optional] 

## Methods

### NewBatchesListResponse

`func NewBatchesListResponse(data []BatchOut, ) *BatchesListResponse`

NewBatchesListResponse instantiates a new BatchesListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBatchesListResponseWithDefaults

`func NewBatchesListResponseWithDefaults() *BatchesListResponse`

NewBatchesListResponseWithDefaults instantiates a new BatchesListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetData

`func (o *BatchesListResponse) GetData() []BatchOut`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *BatchesListResponse) GetDataOk() (*[]BatchOut, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *BatchesListResponse) SetData(v []BatchOut)`

SetData sets Data field to given value.


### GetPagination

`func (o *BatchesListResponse) GetPagination() CursorPagination`

GetPagination returns the Pagination field if non-nil, zero value otherwise.

### GetPaginationOk

`func (o *BatchesListResponse) GetPaginationOk() (*CursorPagination, bool)`

GetPaginationOk returns a tuple with the Pagination field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPagination

`func (o *BatchesListResponse) SetPagination(v CursorPagination)`

SetPagination sets Pagination field to given value.

### HasPagination

`func (o *BatchesListResponse) HasPagination() bool`

HasPagination returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


