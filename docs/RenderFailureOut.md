# RenderFailureOut

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Code** | **string** | &#x60;compliance_failed&#x60; for a document that is well-formed and would be rejected by the ruleset it asked for; &#x60;unprocessable_entity&#x60; for one the renderer could not make sense of. The same codes the synchronous path returns. | 
**Message** | **string** |  | 
**Details** | Pointer to **map[string]interface{}** |  | [optional] 

## Methods

### NewRenderFailureOut

`func NewRenderFailureOut(code string, message string, ) *RenderFailureOut`

NewRenderFailureOut instantiates a new RenderFailureOut object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRenderFailureOutWithDefaults

`func NewRenderFailureOutWithDefaults() *RenderFailureOut`

NewRenderFailureOutWithDefaults instantiates a new RenderFailureOut object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCode

`func (o *RenderFailureOut) GetCode() string`

GetCode returns the Code field if non-nil, zero value otherwise.

### GetCodeOk

`func (o *RenderFailureOut) GetCodeOk() (*string, bool)`

GetCodeOk returns a tuple with the Code field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCode

`func (o *RenderFailureOut) SetCode(v string)`

SetCode sets Code field to given value.


### GetMessage

`func (o *RenderFailureOut) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *RenderFailureOut) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *RenderFailureOut) SetMessage(v string)`

SetMessage sets Message field to given value.


### GetDetails

`func (o *RenderFailureOut) GetDetails() map[string]interface{}`

GetDetails returns the Details field if non-nil, zero value otherwise.

### GetDetailsOk

`func (o *RenderFailureOut) GetDetailsOk() (*map[string]interface{}, bool)`

GetDetailsOk returns a tuple with the Details field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDetails

`func (o *RenderFailureOut) SetDetails(v map[string]interface{})`

SetDetails sets Details field to given value.

### HasDetails

`func (o *RenderFailureOut) HasDetails() bool`

HasDetails returns a boolean if a field has been set.

### SetDetailsNil

`func (o *RenderFailureOut) SetDetailsNil(b bool)`

 SetDetailsNil sets the value for Details to be an explicit nil

### UnsetDetails
`func (o *RenderFailureOut) UnsetDetails()`

UnsetDetails ensures that no value is present for Details, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


