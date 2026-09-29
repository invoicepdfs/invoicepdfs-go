# ReadyResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Status** | **string** |  | 
**Dependencies** | **map[string]string** |  | 
**Workers** | Pointer to **map[string]string** |  | [optional] 
**Degraded** | Pointer to **[]string** |  | [optional] 

## Methods

### NewReadyResponse

`func NewReadyResponse(status string, dependencies map[string]string, ) *ReadyResponse`

NewReadyResponse instantiates a new ReadyResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewReadyResponseWithDefaults

`func NewReadyResponseWithDefaults() *ReadyResponse`

NewReadyResponseWithDefaults instantiates a new ReadyResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetStatus

`func (o *ReadyResponse) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *ReadyResponse) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *ReadyResponse) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetDependencies

`func (o *ReadyResponse) GetDependencies() map[string]string`

GetDependencies returns the Dependencies field if non-nil, zero value otherwise.

### GetDependenciesOk

`func (o *ReadyResponse) GetDependenciesOk() (*map[string]string, bool)`

GetDependenciesOk returns a tuple with the Dependencies field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDependencies

`func (o *ReadyResponse) SetDependencies(v map[string]string)`

SetDependencies sets Dependencies field to given value.


### GetWorkers

`func (o *ReadyResponse) GetWorkers() map[string]string`

GetWorkers returns the Workers field if non-nil, zero value otherwise.

### GetWorkersOk

`func (o *ReadyResponse) GetWorkersOk() (*map[string]string, bool)`

GetWorkersOk returns a tuple with the Workers field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWorkers

`func (o *ReadyResponse) SetWorkers(v map[string]string)`

SetWorkers sets Workers field to given value.

### HasWorkers

`func (o *ReadyResponse) HasWorkers() bool`

HasWorkers returns a boolean if a field has been set.

### GetDegraded

`func (o *ReadyResponse) GetDegraded() []string`

GetDegraded returns the Degraded field if non-nil, zero value otherwise.

### GetDegradedOk

`func (o *ReadyResponse) GetDegradedOk() (*[]string, bool)`

GetDegradedOk returns a tuple with the Degraded field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDegraded

`func (o *ReadyResponse) SetDegraded(v []string)`

SetDegraded sets Degraded field to given value.

### HasDegraded

`func (o *ReadyResponse) HasDegraded() bool`

HasDegraded returns a boolean if a field has been set.

### SetDegradedNil

`func (o *ReadyResponse) SetDegradedNil(b bool)`

 SetDegradedNil sets the value for Degraded to be an explicit nil

### UnsetDegraded
`func (o *ReadyResponse) UnsetDegraded()`

UnsetDegraded ensures that no value is present for Degraded, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


