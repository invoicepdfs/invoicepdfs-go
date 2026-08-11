# \WorkspacesAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AddWorkspaceMember**](WorkspacesAPI.md#AddWorkspaceMember) | **Post** /api/v1/workspaces/{workspace_id}/members | Add Workspace Member
[**CreateWorkspace**](WorkspacesAPI.md#CreateWorkspace) | **Post** /api/v1/workspaces | Create Workspace
[**DeleteWorkspace**](WorkspacesAPI.md#DeleteWorkspace) | **Delete** /api/v1/workspaces/{workspace_id} | Delete Workspace
[**GetWorkspace**](WorkspacesAPI.md#GetWorkspace) | **Get** /api/v1/workspaces/{workspace_id} | Get Workspace
[**ListWorkspaceMembers**](WorkspacesAPI.md#ListWorkspaceMembers) | **Get** /api/v1/workspaces/{workspace_id}/members | List Workspace Members
[**ListWorkspaces**](WorkspacesAPI.md#ListWorkspaces) | **Get** /api/v1/workspaces | List Workspaces
[**RemoveWorkspaceMember**](WorkspacesAPI.md#RemoveWorkspaceMember) | **Delete** /api/v1/workspaces/{workspace_id}/members/{member_id} | Remove Workspace Member
[**UpdateWorkspace**](WorkspacesAPI.md#UpdateWorkspace) | **Patch** /api/v1/workspaces/{workspace_id} | Update Workspace
[**UpdateWorkspaceMember**](WorkspacesAPI.md#UpdateWorkspaceMember) | **Patch** /api/v1/workspaces/{workspace_id}/members/{member_id} | Update Workspace Member



## AddWorkspaceMember

> WorkspaceMembersListResponse AddWorkspaceMember(ctx, workspaceId).WorkspaceMemberCreateRequest(workspaceMemberCreateRequest).IdempotencyKey(idempotencyKey).Execute()

Add Workspace Member

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
	workspaceId := "workspaceId_example" // string | 
	workspaceMemberCreateRequest := *openapiclient.NewWorkspaceMemberCreateRequest("teammate@acme.com") // WorkspaceMemberCreateRequest | 
	idempotencyKey := "idempotencyKey_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.AddWorkspaceMember(context.Background(), workspaceId).WorkspaceMemberCreateRequest(workspaceMemberCreateRequest).IdempotencyKey(idempotencyKey).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.AddWorkspaceMember``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AddWorkspaceMember`: WorkspaceMembersListResponse
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.AddWorkspaceMember`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**workspaceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiAddWorkspaceMemberRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **workspaceMemberCreateRequest** | [**WorkspaceMemberCreateRequest**](WorkspaceMemberCreateRequest.md) |  | 
 **idempotencyKey** | **string** |  | 

### Return type

[**WorkspaceMembersListResponse**](WorkspaceMembersListResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateWorkspace

> WorkspaceResponse CreateWorkspace(ctx).WorkspaceCreateRequest(workspaceCreateRequest).IdempotencyKey(idempotencyKey).Execute()

Create Workspace

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
	workspaceCreateRequest := *openapiclient.NewWorkspaceCreateRequest("Engineering Team") // WorkspaceCreateRequest | 
	idempotencyKey := "idempotencyKey_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.CreateWorkspace(context.Background()).WorkspaceCreateRequest(workspaceCreateRequest).IdempotencyKey(idempotencyKey).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.CreateWorkspace``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateWorkspace`: WorkspaceResponse
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.CreateWorkspace`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateWorkspaceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspaceCreateRequest** | [**WorkspaceCreateRequest**](WorkspaceCreateRequest.md) |  | 
 **idempotencyKey** | **string** |  | 

### Return type

[**WorkspaceResponse**](WorkspaceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteWorkspace

> SimpleBoolResponse DeleteWorkspace(ctx, workspaceId).Execute()

Delete Workspace

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
	workspaceId := "workspaceId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.DeleteWorkspace(context.Background(), workspaceId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.DeleteWorkspace``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteWorkspace`: SimpleBoolResponse
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.DeleteWorkspace`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**workspaceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteWorkspaceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**SimpleBoolResponse**](SimpleBoolResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetWorkspace

> WorkspaceResponse GetWorkspace(ctx, workspaceId).Execute()

Get Workspace

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
	workspaceId := "workspaceId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.GetWorkspace(context.Background(), workspaceId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.GetWorkspace``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetWorkspace`: WorkspaceResponse
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.GetWorkspace`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**workspaceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetWorkspaceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**WorkspaceResponse**](WorkspaceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListWorkspaceMembers

> WorkspaceMembersListResponse ListWorkspaceMembers(ctx, workspaceId).Execute()

List Workspace Members

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
	workspaceId := "workspaceId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.ListWorkspaceMembers(context.Background(), workspaceId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.ListWorkspaceMembers``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListWorkspaceMembers`: WorkspaceMembersListResponse
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.ListWorkspaceMembers`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**workspaceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListWorkspaceMembersRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**WorkspaceMembersListResponse**](WorkspaceMembersListResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListWorkspaces

> WorkspacesListResponse ListWorkspaces(ctx).Limit(limit).Cursor(cursor).Execute()

List Workspaces

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.ListWorkspaces(context.Background()).Limit(limit).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.ListWorkspaces``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListWorkspaces`: WorkspacesListResponse
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.ListWorkspaces`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListWorkspacesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int32** |  | [default to 50]
 **cursor** | **string** |  | 

### Return type

[**WorkspacesListResponse**](WorkspacesListResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RemoveWorkspaceMember

> SimpleBoolResponse RemoveWorkspaceMember(ctx, workspaceId, memberId).Execute()

Remove Workspace Member

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
	workspaceId := "workspaceId_example" // string | 
	memberId := "memberId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.RemoveWorkspaceMember(context.Background(), workspaceId, memberId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.RemoveWorkspaceMember``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RemoveWorkspaceMember`: SimpleBoolResponse
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.RemoveWorkspaceMember`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**workspaceId** | **string** |  | 
**memberId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRemoveWorkspaceMemberRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**SimpleBoolResponse**](SimpleBoolResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateWorkspace

> WorkspaceResponse UpdateWorkspace(ctx, workspaceId).WorkspacePatchRequest(workspacePatchRequest).IdempotencyKey(idempotencyKey).Execute()

Update Workspace

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
	workspaceId := "workspaceId_example" // string | 
	workspacePatchRequest := *openapiclient.NewWorkspacePatchRequest() // WorkspacePatchRequest | 
	idempotencyKey := "idempotencyKey_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.UpdateWorkspace(context.Background(), workspaceId).WorkspacePatchRequest(workspacePatchRequest).IdempotencyKey(idempotencyKey).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.UpdateWorkspace``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateWorkspace`: WorkspaceResponse
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.UpdateWorkspace`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**workspaceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateWorkspaceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **workspacePatchRequest** | [**WorkspacePatchRequest**](WorkspacePatchRequest.md) |  | 
 **idempotencyKey** | **string** |  | 

### Return type

[**WorkspaceResponse**](WorkspaceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateWorkspaceMember

> WorkspaceMemberOut UpdateWorkspaceMember(ctx, workspaceId, memberId).WorkspaceMemberPatchRequest(workspaceMemberPatchRequest).Execute()

Update Workspace Member

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
	workspaceId := "workspaceId_example" // string | 
	memberId := "memberId_example" // string | 
	workspaceMemberPatchRequest := *openapiclient.NewWorkspaceMemberPatchRequest() // WorkspaceMemberPatchRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.UpdateWorkspaceMember(context.Background(), workspaceId, memberId).WorkspaceMemberPatchRequest(workspaceMemberPatchRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.UpdateWorkspaceMember``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateWorkspaceMember`: WorkspaceMemberOut
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.UpdateWorkspaceMember`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**workspaceId** | **string** |  | 
**memberId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateWorkspaceMemberRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **workspaceMemberPatchRequest** | [**WorkspaceMemberPatchRequest**](WorkspaceMemberPatchRequest.md) |  | 

### Return type

[**WorkspaceMemberOut**](WorkspaceMemberOut.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

