# \AuditLogAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetAuditEvent**](AuditLogAPI.md#GetAuditEvent) | **Get** /api/v1/audit-events/{audit_event_id} | Get Audit Event
[**ListAuditEvents**](AuditLogAPI.md#ListAuditEvents) | **Get** /api/v1/audit-events | List Audit Events



## GetAuditEvent

> AuditEventResponse GetAuditEvent(ctx, auditEventId).Execute()

Get Audit Event

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/invoicepdfs/invoicepdfs-go"
)

func main() {
	auditEventId := "auditEventId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuditLogAPI.GetAuditEvent(context.Background(), auditEventId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuditLogAPI.GetAuditEvent``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetAuditEvent`: AuditEventResponse
	fmt.Fprintf(os.Stdout, "Response from `AuditLogAPI.GetAuditEvent`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**auditEventId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetAuditEventRequest struct via the builder pattern


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


## ListAuditEvents

> AuditEventsListResponse ListAuditEvents(ctx).Limit(limit).Cursor(cursor).Action(action).ResourceType(resourceType).ResourceId(resourceId).Execute()

List Audit Events

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/invoicepdfs/invoicepdfs-go"
)

func main() {
	limit := int32(56) // int32 |  (optional) (default to 50)
	cursor := "cursor_example" // string |  (optional)
	action := "action_example" // string |  (optional)
	resourceType := "resourceType_example" // string |  (optional)
	resourceId := "resourceId_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuditLogAPI.ListAuditEvents(context.Background()).Limit(limit).Cursor(cursor).Action(action).ResourceType(resourceType).ResourceId(resourceId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuditLogAPI.ListAuditEvents``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListAuditEvents`: AuditEventsListResponse
	fmt.Fprintf(os.Stdout, "Response from `AuditLogAPI.ListAuditEvents`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListAuditEventsRequest struct via the builder pattern


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

