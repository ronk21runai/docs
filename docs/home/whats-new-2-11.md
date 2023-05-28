# Run:ai version 2.11
## Release date

May 2023

## Release content

### Compatibility

Removed support for OpenShift 4.8 and 4.9, and Kubernetes 1.21 and 1.22.

Added support for OpenShift 4.12 and Kubernetes 1.27.

Added support for multiple OpenShift clusters. For configuration information, see [Installing additional Clusters](../admin/runai-setup/self-hosted/ocp/additional-clusters.md)

The `runai top job` command was deprecated.

When SSO is enabled, you can still create and authenticate with Local users. For configuration of local users and SSO users, see [Create a new user](../admin/admin-ui-setup/admin-ui-users.md#create-a-user).

### Researcher tools enhancements

**OpenShift Dev Spaces**

Added support fort Openshift Dev Spaces custom resource definitions using the RunAI scheduler.

**Cluster API**

Added the following new capabilities for Researchers in the Cluster API:

1. Check the status of the job using the API Researcher API.
2. Get container logs using the API - to investigate in case something failed.
3. Submit a job using the backend.
4. Stop, Suspend and Resume jobs.

**Comet Integration**

Comet builds tools that help data scientists, engineers, and team leaders accelerate and optimize machine learning and deep learning models. This integration with Run:ai provides organizations of every size a platform to build better ML models faster. For more information, see [Comet](https://www.comet.com/site/){target=_blank}. For configuration information, see [Comet integration](../admin/integration/comet.md)
## Known issues

|Internal ID|Description|Workaround|
|-----------|--------------|--------------|

## Fixed issues

|Internal ID|Description|
|-----------|--------------|
| RUN-6827 | Fixed an issue where the elipsis remains in the Dashboard when using Firefox after a long idle time. |
| RUN-8621 | Fixed the error response to 204 when changing to a custom logo. |
| RUN-8662 | Fixed grayed out submit button when using a template with pvc. |
| RUN-8890 | Fixed a scheduler panic when both a project and a department use the same name. |
| RUN-9035 | Fixed an issue that allowed a scheduler from any node pool to delete reservation pods created on a different node pool which may have caused a failure to schedule jobs with fractional GPU allocations. |
| RUN-9089 | Added the `port forward` CLI command. |
| RUN-9166 | Fixed incorrect response about resource availability in messages indicating why a specific job failed to schedule. |
| RUN-9259 | Fixed an issue where cluster sync requests are not working at scale due to a large number of requests. |