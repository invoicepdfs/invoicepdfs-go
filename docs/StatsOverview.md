# StatsOverview

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Counts** | [**StatsCounts**](StatsCounts.md) |  | 
**InvoiceStatusCounts** | **map[string]int32** |  | 
**RecentInvoices** | [**[]StatsRecentInvoice**](StatsRecentInvoice.md) |  | 

## Methods

### NewStatsOverview

`func NewStatsOverview(counts StatsCounts, invoiceStatusCounts map[string]int32, recentInvoices []StatsRecentInvoice, ) *StatsOverview`

NewStatsOverview instantiates a new StatsOverview object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewStatsOverviewWithDefaults

`func NewStatsOverviewWithDefaults() *StatsOverview`

NewStatsOverviewWithDefaults instantiates a new StatsOverview object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCounts

`func (o *StatsOverview) GetCounts() StatsCounts`

GetCounts returns the Counts field if non-nil, zero value otherwise.

### GetCountsOk

`func (o *StatsOverview) GetCountsOk() (*StatsCounts, bool)`

GetCountsOk returns a tuple with the Counts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCounts

`func (o *StatsOverview) SetCounts(v StatsCounts)`

SetCounts sets Counts field to given value.


### GetInvoiceStatusCounts

`func (o *StatsOverview) GetInvoiceStatusCounts() map[string]int32`

GetInvoiceStatusCounts returns the InvoiceStatusCounts field if non-nil, zero value otherwise.

### GetInvoiceStatusCountsOk

`func (o *StatsOverview) GetInvoiceStatusCountsOk() (*map[string]int32, bool)`

GetInvoiceStatusCountsOk returns a tuple with the InvoiceStatusCounts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInvoiceStatusCounts

`func (o *StatsOverview) SetInvoiceStatusCounts(v map[string]int32)`

SetInvoiceStatusCounts sets InvoiceStatusCounts field to given value.


### GetRecentInvoices

`func (o *StatsOverview) GetRecentInvoices() []StatsRecentInvoice`

GetRecentInvoices returns the RecentInvoices field if non-nil, zero value otherwise.

### GetRecentInvoicesOk

`func (o *StatsOverview) GetRecentInvoicesOk() (*[]StatsRecentInvoice, bool)`

GetRecentInvoicesOk returns a tuple with the RecentInvoices field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRecentInvoices

`func (o *StatsOverview) SetRecentInvoices(v []StatsRecentInvoice)`

SetRecentInvoices sets RecentInvoices field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


