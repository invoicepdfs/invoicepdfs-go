# InvoicesListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Data** | [**[]InvoiceOut**](InvoiceOut.md) |  | 
**Pagination** | Pointer to [**CursorPagination**](CursorPagination.md) |  | [optional] 

## Methods

### NewInvoicesListResponse

`func NewInvoicesListResponse(data []InvoiceOut, ) *InvoicesListResponse`

NewInvoicesListResponse instantiates a new InvoicesListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewInvoicesListResponseWithDefaults

`func NewInvoicesListResponseWithDefaults() *InvoicesListResponse`

NewInvoicesListResponseWithDefaults instantiates a new InvoicesListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetData

`func (o *InvoicesListResponse) GetData() []InvoiceOut`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *InvoicesListResponse) GetDataOk() (*[]InvoiceOut, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *InvoicesListResponse) SetData(v []InvoiceOut)`

SetData sets Data field to given value.


### GetPagination

`func (o *InvoicesListResponse) GetPagination() CursorPagination`

GetPagination returns the Pagination field if non-nil, zero value otherwise.

### GetPaginationOk

`func (o *InvoicesListResponse) GetPaginationOk() (*CursorPagination, bool)`

GetPaginationOk returns a tuple with the Pagination field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPagination

`func (o *InvoicesListResponse) SetPagination(v CursorPagination)`

SetPagination sets Pagination field to given value.

### HasPagination

`func (o *InvoicesListResponse) HasPagination() bool`

HasPagination returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


