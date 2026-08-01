# \AuditLogAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetAuditEventApiV1AuditEventsAuditEventIdGet**](AuditLogAPI.md#GetAuditEventApiV1AuditEventsAuditEventIdGet) | **Get** /api/v1/audit-events/{audit_event_id} | Get Audit Event
[**ListAuditEventsApiV1AuditEventsGet**](AuditLogAPI.md#ListAuditEventsApiV1AuditEventsGet) | **Get** /api/v1/audit-events | List Audit Events



## GetAuditEventApiV1AuditEventsAuditEventIdGet

> AuditEventResponse GetAuditEventApiV1AuditEventsAuditEventIdGet(ctx, auditEventId).Execute()

Get Audit Event

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/invoicepdfs"
)

func main() {
	auditEventId := "auditEventId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuditLogAPI.GetAuditEventApiV1AuditEventsAuditEventIdGet(context.Background(), auditEventId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuditLogAPI.GetAuditEventApiV1AuditEventsAuditEventIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetAuditEventApiV1AuditEventsAuditEventIdGet`: AuditEventResponse
	fmt.Fprintf(os.Stdout, "Response from `AuditLogAPI.GetAuditEventApiV1AuditEventsAuditEventIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**auditEventId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetAuditEventApiV1AuditEventsAuditEventIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**AuditEventResponse**](AuditEventResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListAuditEventsApiV1AuditEventsGet

> AuditEventsListResponse ListAuditEventsApiV1AuditEventsGet(ctx).Limit(limit).Cursor(cursor).Action(action).ResourceType(resourceType).ResourceId(resourceId).Execute()

List Audit Events

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/invoicepdfs"
)

func main() {
	limit := int32(56) // int32 |  (optional) (default to 50)
	cursor := "cursor_example" // string |  (optional)
	action := "action_example" // string |  (optional)
	resourceType := "resourceType_example" // string |  (optional)
	resourceId := "resourceId_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuditLogAPI.ListAuditEventsApiV1AuditEventsGet(context.Background()).Limit(limit).Cursor(cursor).Action(action).ResourceType(resourceType).ResourceId(resourceId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuditLogAPI.ListAuditEventsApiV1AuditEventsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListAuditEventsApiV1AuditEventsGet`: AuditEventsListResponse
	fmt.Fprintf(os.Stdout, "Response from `AuditLogAPI.ListAuditEventsApiV1AuditEventsGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListAuditEventsApiV1AuditEventsGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int32** |  | [default to 50]
 **cursor** | **string** |  | 
 **action** | **string** |  | 
 **resourceType** | **string** |  | 
 **resourceId** | **string** |  | 

### Return type

[**AuditEventsListResponse**](AuditEventsListResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

