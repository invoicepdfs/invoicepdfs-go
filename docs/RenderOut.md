# RenderOut

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Status** | **string** |  | 
**DocumentType** | **string** |  | 
**Format** | **string** |  | 
**DownloadUrl** | **string** |  | 
**ExpiresAt** | **string** |  | 
**Calculation** | [**CalculationBreakdown**](CalculationBreakdown.md) |  | 
**CreatedAt** | **string** |  | 

## Methods

### NewRenderOut

`func NewRenderOut(id string, status string, documentType string, format string, downloadUrl string, expiresAt string, calculation CalculationBreakdown, createdAt string, ) *RenderOut`

NewRenderOut instantiates a new RenderOut object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRenderOutWithDefaults

`func NewRenderOutWithDefaults() *RenderOut`

NewRenderOutWithDefaults instantiates a new RenderOut object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *RenderOut) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *RenderOut) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *RenderOut) SetId(v string)`

SetId sets Id field to given value.


### GetStatus

`func (o *RenderOut) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *RenderOut) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *RenderOut) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetDocumentType

`func (o *RenderOut) GetDocumentType() string`

GetDocumentType returns the DocumentType field if non-nil, zero value otherwise.

### GetDocumentTypeOk

`func (o *RenderOut) GetDocumentTypeOk() (*string, bool)`

GetDocumentTypeOk returns a tuple with the DocumentType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDocumentType

`func (o *RenderOut) SetDocumentType(v string)`

SetDocumentType sets DocumentType field to given value.


### GetFormat

`func (o *RenderOut) GetFormat() string`

GetFormat returns the Format field if non-nil, zero value otherwise.

### GetFormatOk

`func (o *RenderOut) GetFormatOk() (*string, bool)`

GetFormatOk returns a tuple with the Format field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFormat

`func (o *RenderOut) SetFormat(v string)`

SetFormat sets Format field to given value.


### GetDownloadUrl

`func (o *RenderOut) GetDownloadUrl() string`

GetDownloadUrl returns the DownloadUrl field if non-nil, zero value otherwise.

### GetDownloadUrlOk

`func (o *RenderOut) GetDownloadUrlOk() (*string, bool)`

GetDownloadUrlOk returns a tuple with the DownloadUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDownloadUrl

`func (o *RenderOut) SetDownloadUrl(v string)`

SetDownloadUrl sets DownloadUrl field to given value.


### GetExpiresAt

`func (o *RenderOut) GetExpiresAt() string`

GetExpiresAt returns the ExpiresAt field if non-nil, zero value otherwise.

### GetExpiresAtOk

`func (o *RenderOut) GetExpiresAtOk() (*string, bool)`

GetExpiresAtOk returns a tuple with the ExpiresAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresAt

`func (o *RenderOut) SetExpiresAt(v string)`

SetExpiresAt sets ExpiresAt field to given value.


### GetCalculation

`func (o *RenderOut) GetCalculation() CalculationBreakdown`

GetCalculation returns the Calculation field if non-nil, zero value otherwise.

### GetCalculationOk

`func (o *RenderOut) GetCalculationOk() (*CalculationBreakdown, bool)`

GetCalculationOk returns a tuple with the Calculation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCalculation

`func (o *RenderOut) SetCalculation(v CalculationBreakdown)`

SetCalculation sets Calculation field to given value.


### GetCreatedAt

`func (o *RenderOut) GetCreatedAt() string`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *RenderOut) GetCreatedAtOk() (*string, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *RenderOut) SetCreatedAt(v string)`

SetCreatedAt sets CreatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


