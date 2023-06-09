---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "morpheus_nested_workflow_task Resource - terraform-provider-morpheus"
subcategory: ""
description: |-
  Provides a Morpheus nested workflow task resource
---

# morpheus_nested_workflow_task (Resource)

Provides a Morpheus nested workflow task resource

## Example Usage

```terraform
data "morpheus_workflow" "example_workflow" {
  name = "Example Workflow"
}

resource "morpheus_nested_workflow_task" "tfexample_nested_workflow" {
  name                      = "tfexample_nested_workflow"
  code                      = "tfexample_nested_workflow"
  labels                    = ["demo", "terraform"]
  operational_workflow_id   = data.morpheus_workflow.example_workflow.id
  operational_workflow_name = data.morpheus_workflow.example_workflow.name
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `name` (String) The name of the nested workflow task

### Optional

- `allow_custom_config` (Boolean) Custom configuration data to pass during the execution of the shell script
- `code` (String) The code of the nested workflow task
- `labels` (Set of String) The organization labels associated with the task (Only supported on Morpheus 5.5.3 or higher)
- `operational_workflow_id` (Number) The ID of the operational workflow
- `operational_workflow_name` (String) The name of the operational workflow
- `retry_count` (Number) The number of times to retry the task if there is a failure
- `retry_delay_seconds` (Number) The number of seconds to wait between retry attempts
- `retryable` (Boolean) Whether to retry the task if there is a failure

### Read-Only

- `id` (String) The ID of the nested workflow task

## Import

Import is supported using the following syntax:

```shell
terraform import morpheus_nested_workflow_task.tf_example_nested_workflow_task 1
```