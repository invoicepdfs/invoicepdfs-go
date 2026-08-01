# \WorkspacesAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateMemberApiV1WorkspacesWorkspaceIdMembersPost**](WorkspacesAPI.md#CreateMemberApiV1WorkspacesWorkspaceIdMembersPost) | **Post** /api/v1/workspaces/{workspace_id}/members | Create Member
[**CreateWorkspaceApiV1WorkspacesPost**](WorkspacesAPI.md#CreateWorkspaceApiV1WorkspacesPost) | **Post** /api/v1/workspaces | Create Workspace
[**DeleteMemberApiV1WorkspacesWorkspaceIdMembersMemberIdDelete**](WorkspacesAPI.md#DeleteMemberApiV1WorkspacesWorkspaceIdMembersMemberIdDelete) | **Delete** /api/v1/workspaces/{workspace_id}/members/{member_id} | Delete Member
[**DeleteWorkspaceApiV1WorkspacesWorkspaceIdDelete**](WorkspacesAPI.md#DeleteWorkspaceApiV1WorkspacesWorkspaceIdDelete) | **Delete** /api/v1/workspaces/{workspace_id} | Delete Workspace
[**GetWorkspaceApiV1WorkspacesWorkspaceIdGet**](WorkspacesAPI.md#GetWorkspaceApiV1WorkspacesWorkspaceIdGet) | **Get** /api/v1/workspaces/{workspace_id} | Get Workspace
[**ListMembersApiV1WorkspacesWorkspaceIdMembersGet**](WorkspacesAPI.md#ListMembersApiV1WorkspacesWorkspaceIdMembersGet) | **Get** /api/v1/workspaces/{workspace_id}/members | List Members
[**ListWorkspacesApiV1WorkspacesGet**](WorkspacesAPI.md#ListWorkspacesApiV1WorkspacesGet) | **Get** /api/v1/workspaces | List Workspaces
[**PatchMemberApiV1WorkspacesWorkspaceIdMembersMemberIdPatch**](WorkspacesAPI.md#PatchMemberApiV1WorkspacesWorkspaceIdMembersMemberIdPatch) | **Patch** /api/v1/workspaces/{workspace_id}/members/{member_id} | Patch Member
[**PatchWorkspaceApiV1WorkspacesWorkspaceIdPatch**](WorkspacesAPI.md#PatchWorkspaceApiV1WorkspacesWorkspaceIdPatch) | **Patch** /api/v1/workspaces/{workspace_id} | Patch Workspace



## CreateMemberApiV1WorkspacesWorkspaceIdMembersPost

> WorkspaceMembersListResponse CreateMemberApiV1WorkspacesWorkspaceIdMembersPost(ctx, workspaceId).WorkspaceMemberCreateRequest(workspaceMemberCreateRequest).IdempotencyKey(idempotencyKey).Execute()

Create Member

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	workspaceId := "workspaceId_example" // string | 
	workspaceMemberCreateRequest := *openapiclient.NewWorkspaceMemberCreateRequest("teammate@acme.com") // WorkspaceMemberCreateRequest | 
	idempotencyKey := "idempotencyKey_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.CreateMemberApiV1WorkspacesWorkspaceIdMembersPost(context.Background(), workspaceId).WorkspaceMemberCreateRequest(workspaceMemberCreateRequest).IdempotencyKey(idempotencyKey).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.CreateMemberApiV1WorkspacesWorkspaceIdMembersPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateMemberApiV1WorkspacesWorkspaceIdMembersPost`: WorkspaceMembersListResponse
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.CreateMemberApiV1WorkspacesWorkspaceIdMembersPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**workspaceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateMemberApiV1WorkspacesWorkspaceIdMembersPostRequest struct via the builder pattern


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


## CreateWorkspaceApiV1WorkspacesPost

> WorkspaceResponse CreateWorkspaceApiV1WorkspacesPost(ctx).WorkspaceCreateRequest(workspaceCreateRequest).IdempotencyKey(idempotencyKey).Execute()

Create Workspace

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	workspaceCreateRequest := *openapiclient.NewWorkspaceCreateRequest("Engineering Team") // WorkspaceCreateRequest | 
	idempotencyKey := "idempotencyKey_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.CreateWorkspaceApiV1WorkspacesPost(context.Background()).WorkspaceCreateRequest(workspaceCreateRequest).IdempotencyKey(idempotencyKey).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.CreateWorkspaceApiV1WorkspacesPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateWorkspaceApiV1WorkspacesPost`: WorkspaceResponse
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.CreateWorkspaceApiV1WorkspacesPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateWorkspaceApiV1WorkspacesPostRequest struct via the builder pattern


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


## DeleteMemberApiV1WorkspacesWorkspaceIdMembersMemberIdDelete

> SimpleBoolResponse DeleteMemberApiV1WorkspacesWorkspaceIdMembersMemberIdDelete(ctx, workspaceId, memberId).Execute()

Delete Member

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	workspaceId := "workspaceId_example" // string | 
	memberId := "memberId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.DeleteMemberApiV1WorkspacesWorkspaceIdMembersMemberIdDelete(context.Background(), workspaceId, memberId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.DeleteMemberApiV1WorkspacesWorkspaceIdMembersMemberIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteMemberApiV1WorkspacesWorkspaceIdMembersMemberIdDelete`: SimpleBoolResponse
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.DeleteMemberApiV1WorkspacesWorkspaceIdMembersMemberIdDelete`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**workspaceId** | **string** |  | 
**memberId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteMemberApiV1WorkspacesWorkspaceIdMembersMemberIdDeleteRequest struct via the builder pattern


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


## DeleteWorkspaceApiV1WorkspacesWorkspaceIdDelete

> SimpleBoolResponse DeleteWorkspaceApiV1WorkspacesWorkspaceIdDelete(ctx, workspaceId).Execute()

Delete Workspace

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	workspaceId := "workspaceId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.DeleteWorkspaceApiV1WorkspacesWorkspaceIdDelete(context.Background(), workspaceId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.DeleteWorkspaceApiV1WorkspacesWorkspaceIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteWorkspaceApiV1WorkspacesWorkspaceIdDelete`: SimpleBoolResponse
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.DeleteWorkspaceApiV1WorkspacesWorkspaceIdDelete`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**workspaceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteWorkspaceApiV1WorkspacesWorkspaceIdDeleteRequest struct via the builder pattern


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


## GetWorkspaceApiV1WorkspacesWorkspaceIdGet

> WorkspaceResponse GetWorkspaceApiV1WorkspacesWorkspaceIdGet(ctx, workspaceId).Execute()

Get Workspace

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	workspaceId := "workspaceId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.GetWorkspaceApiV1WorkspacesWorkspaceIdGet(context.Background(), workspaceId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.GetWorkspaceApiV1WorkspacesWorkspaceIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetWorkspaceApiV1WorkspacesWorkspaceIdGet`: WorkspaceResponse
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.GetWorkspaceApiV1WorkspacesWorkspaceIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**workspaceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetWorkspaceApiV1WorkspacesWorkspaceIdGetRequest struct via the builder pattern


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


## ListMembersApiV1WorkspacesWorkspaceIdMembersGet

> WorkspaceMembersListResponse ListMembersApiV1WorkspacesWorkspaceIdMembersGet(ctx, workspaceId).Execute()

List Members

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	workspaceId := "workspaceId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.ListMembersApiV1WorkspacesWorkspaceIdMembersGet(context.Background(), workspaceId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.ListMembersApiV1WorkspacesWorkspaceIdMembersGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListMembersApiV1WorkspacesWorkspaceIdMembersGet`: WorkspaceMembersListResponse
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.ListMembersApiV1WorkspacesWorkspaceIdMembersGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**workspaceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListMembersApiV1WorkspacesWorkspaceIdMembersGetRequest struct via the builder pattern


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


## ListWorkspacesApiV1WorkspacesGet

> WorkspacesListResponse ListWorkspacesApiV1WorkspacesGet(ctx).Limit(limit).Cursor(cursor).Execute()

List Workspaces

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	limit := int32(56) // int32 |  (optional) (default to 50)
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.ListWorkspacesApiV1WorkspacesGet(context.Background()).Limit(limit).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.ListWorkspacesApiV1WorkspacesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListWorkspacesApiV1WorkspacesGet`: WorkspacesListResponse
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.ListWorkspacesApiV1WorkspacesGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListWorkspacesApiV1WorkspacesGetRequest struct via the builder pattern


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


## PatchMemberApiV1WorkspacesWorkspaceIdMembersMemberIdPatch

> WorkspaceMemberOut PatchMemberApiV1WorkspacesWorkspaceIdMembersMemberIdPatch(ctx, workspaceId, memberId).WorkspaceMemberPatchRequest(workspaceMemberPatchRequest).Execute()

Patch Member

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	workspaceId := "workspaceId_example" // string | 
	memberId := "memberId_example" // string | 
	workspaceMemberPatchRequest := *openapiclient.NewWorkspaceMemberPatchRequest() // WorkspaceMemberPatchRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.PatchMemberApiV1WorkspacesWorkspaceIdMembersMemberIdPatch(context.Background(), workspaceId, memberId).WorkspaceMemberPatchRequest(workspaceMemberPatchRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.PatchMemberApiV1WorkspacesWorkspaceIdMembersMemberIdPatch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PatchMemberApiV1WorkspacesWorkspaceIdMembersMemberIdPatch`: WorkspaceMemberOut
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.PatchMemberApiV1WorkspacesWorkspaceIdMembersMemberIdPatch`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**workspaceId** | **string** |  | 
**memberId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiPatchMemberApiV1WorkspacesWorkspaceIdMembersMemberIdPatchRequest struct via the builder pattern


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


## PatchWorkspaceApiV1WorkspacesWorkspaceIdPatch

> WorkspaceResponse PatchWorkspaceApiV1WorkspacesWorkspaceIdPatch(ctx, workspaceId).WorkspacePatchRequest(workspacePatchRequest).IdempotencyKey(idempotencyKey).Execute()

Patch Workspace

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	workspaceId := "workspaceId_example" // string | 
	workspacePatchRequest := *openapiclient.NewWorkspacePatchRequest() // WorkspacePatchRequest | 
	idempotencyKey := "idempotencyKey_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.PatchWorkspaceApiV1WorkspacesWorkspaceIdPatch(context.Background(), workspaceId).WorkspacePatchRequest(workspacePatchRequest).IdempotencyKey(idempotencyKey).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.PatchWorkspaceApiV1WorkspacesWorkspaceIdPatch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PatchWorkspaceApiV1WorkspacesWorkspaceIdPatch`: WorkspaceResponse
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.PatchWorkspaceApiV1WorkspacesWorkspaceIdPatch`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**workspaceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiPatchWorkspaceApiV1WorkspacesWorkspaceIdPatchRequest struct via the builder pattern


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

