# DocumentComplianceRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**DocumentType** | Pointer to **string** |  | [optional] [default to "invoice"]
**Data** | [**DocumentInvoiceDataInput**](DocumentInvoiceDataInput.md) |  | 
**Profile** | **string** | Which ruleset to hold the document to. Rulesets differ: a document valid under one can be rejected by another, so there is no default. | 

## Methods

### NewDocumentComplianceRequest

`func NewDocumentComplianceRequest(data DocumentInvoiceDataInput, profile string, ) *DocumentComplianceRequest`

NewDocumentComplianceRequest instantiates a new DocumentComplianceRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDocumentComplianceRequestWithDefaults

`func NewDocumentComplianceRequestWithDefaults() *DocumentComplianceRequest`

NewDocumentComplianceRequestWithDefaults instantiates a new DocumentComplianceRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDocumentType

`func (o *DocumentComplianceRequest) GetDocumentType() string`

GetDocumentType returns the DocumentType field if non-nil, zero value otherwise.

### GetDocumentTypeOk

`func (o *DocumentComplianceRequest) GetDocumentTypeOk() (*string, bool)`

GetDocumentTypeOk returns a tuple with the DocumentType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDocumentType

`func (o *DocumentComplianceRequest) SetDocumentType(v string)`

SetDocumentType sets DocumentType field to given value.

### HasDocumentType

`func (o *DocumentComplianceRequest) HasDocumentType() bool`

HasDocumentType returns a boolean if a field has been set.

### GetData

`func (o *DocumentComplianceRequest) GetData() DocumentInvoiceDataInput`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *DocumentComplianceRequest) GetDataOk() (*DocumentInvoiceDataInput, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *DocumentComplianceRequest) SetData(v DocumentInvoiceDataInput)`

SetData sets Data field to given value.


### GetProfile

`func (o *DocumentComplianceRequest) GetProfile() string`

GetProfile returns the Profile field if non-nil, zero value otherwise.

### GetProfileOk

`func (o *DocumentComplianceRequest) GetProfileOk() (*string, bool)`

GetProfileOk returns a tuple with the Profile field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProfile

`func (o *DocumentComplianceRequest) SetProfile(v string)`

SetProfile sets Profile field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


