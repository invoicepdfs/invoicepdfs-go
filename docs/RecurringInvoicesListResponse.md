# RecurringInvoicesListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Data** | [**[]RecurringInvoiceOut**](RecurringInvoiceOut.md) |  | 
**Pagination** | [**CursorPagination**](CursorPagination.md) |  | 

## Methods

### NewRecurringInvoicesListResponse

`func NewRecurringInvoicesListResponse(data []RecurringInvoiceOut, pagination CursorPagination, ) *RecurringInvoicesListResponse`

NewRecurringInvoicesListResponse instantiates a new RecurringInvoicesListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRecurringInvoicesListResponseWithDefaults

`func NewRecurringInvoicesListResponseWithDefaults() *RecurringInvoicesListResponse`

NewRecurringInvoicesListResponseWithDefaults instantiates a new RecurringInvoicesListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetData

`func (o *RecurringInvoicesListResponse) GetData() []RecurringInvoiceOut`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *RecurringInvoicesListResponse) GetDataOk() (*[]RecurringInvoiceOut, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *RecurringInvoicesListResponse) SetData(v []RecurringInvoiceOut)`

SetData sets Data field to given value.


### GetPagination

`func (o *RecurringInvoicesListResponse) GetPagination() CursorPagination`

GetPagination returns the Pagination field if non-nil, zero value otherwise.

### GetPaginationOk

`func (o *RecurringInvoicesListResponse) GetPaginationOk() (*CursorPagination, bool)`

GetPaginationOk returns a tuple with the Pagination field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPagination

`func (o *RecurringInvoicesListResponse) SetPagination(v CursorPagination)`

SetPagination sets Pagination field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


