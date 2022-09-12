# Terraform Provider for Morpheus

[![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/gomorpheus/terraform-provider-morpheus?label=release)](https://github.com/gomorpheus/terraform-provider-morpheus/releases) [![license](https://img.shields.io/github/license/gomorpheus/terraform-provider-morpheus.svg)]()

<img src="https://morpheusdata.com/wp-content/uploads/2020/04/morpheus-logo-v2.svg" width="300px">

- Website: https://www.morpheusdata.com/
- Docs: [Morpheus Documentation](https://docs.morpheusdata.com)
- Support: [Morpheus Support](https://support.morpheusdata.com)


This is the Terraform provider for the Morpheus Data Cloud Management Platform (CMP). It interfaces with the [Morpheus API](https://apidocs.morpheusdata.com/) using the morpheus-go-sdk client. Like all [Terraform Providers](https://github.com/terraform-providers/), it is written in Go.

This is being developed in conjunction with [morpheus-go-sdk](https://github.com/gomorpheus/morpheus-go-sdk).  

## Requirements
------------

* [Terraform](https://www.terraform.io/) | 0.13+
* [Go](https://golang.org/dl/) 1.17 (to build the provider plugin)


## Getting Started
---------------------

The best way to get started using the Morpheus Terraform provider is by following the [getting started guide](docs/guides/getting_started.md).

## Supported Resources
----------------------

The following list of resources are supported by the Morpheus Terraform provider:

| Resource Name | Description |
|------|---------------|
| [morpheus_ansible_playbook_task](docs/resources/ansible_playbook_task.md) | Morpheus ansible playbook automation task resource |
| [morpheus_arm_app_blueprint](docs/resources/arm_app_blueprint.md) | Morpheus ARM app blueprint resource |
| [morpheus_arm_spec_template](docs/resources/arm_spec_template.md) | Morpheus ARM spec template resource |
| [morpheus_backup_creation_policy](docs/resources/backup_creation_policy.md) | Morpheus backup creation policy resource |
| [morpheus_budget_policy](docs/resources/budget_policy.md) | Morpheus budget policy resource |
| [morpheus_checkbox_option_type](docs/resources/checkbox_option_type.md) | Morpheus checkbox option type resource |
| [morpheus_cloud_formation_app_blueprint](docs/resources/cloud_formation_app_blueprint.md) | Morpheus Cloud Formation app blueprint resource |
| [morpheus_cloud_formation_spec_template](docs/resources/cloud_formation_spec_template.md) | Morpheus Cloud Formation spec template resource |
[morpheus_cluster_layout](docs/resources/cluster_layout.md) | Morpheus cluster layout resource |
| [morpheus_cluster_resource_name_policy](docs/resources/cluster_resource_name_policy.md) | Morpheus cluster resource name policy resource |
| [morpheus_contact](docs/resources/morpheus_contact.md) | Morpheus contact resource |
| [morpheus_environment](docs/resources/environment.md) | Morpheus environment resource |
| [morpheus_execute_schedule](docs/resources/execute_schedule.md) | Morpheus execute schedule resource |
| [morpheus_file_template](docs/resources/file_template.md) | Morpheus file template resource |
| [morpheus_groovy_task](docs/resources/groovy_script_task.md) | Morpheus groovy script task resource |
| [morpheus_group](docs/resources/group.md) | Morpheus group resource |
| [morpheus_helm_app_blueprint](docs/resources/helm_app_blueprint.md) | Morpheus HELM app blueprint resource |
| [morpheus_helm_spec_template](docs/resources/helm_spec_template.md) | Morpheus HELM spec template resource |
| [morpheus_hidden_option_type](docs/resources/hidden_option_type.md) | Morpheus hidden option type resource |
| [morpheus_hostname_policy](docs/resources/hostname_policy.md) | Morpheus hostname policy resource |
| [morpheus_instance_layout](docs/resources/instance_layout.md) | Morpheus instance_layout resource |
| [morpheus_instance_type](docs/resources/instance_type.md) | Morpheus instance_type resource |
| [morpheus_kubernetes_app_blueprint](docs/resources/kubernetes_app_blueprint.md) | Morpheus Kubernetes app blueprint resource |
| [morpheus_kubernetes_spec_template](docs/resources/kubernetes_spec_template.md) | Morpheus Kubernetes spec template resource |
| [morpheus_javascript_task](docs/resources/javascript_task.md) | Morpheus javascript task resource |
| [morpheus_manual_option_list](docs/resources/manual_option_list.md) | Morpheus manual option list resource |
| [morpheus_max_containers_policy](docs/resources/max_containers_policy.md) | Morpheus max containers policy resource |
| [morpheus_max_cores_policy](docs/resources/max_cores_policy.md) | Morpheus max cores policy resource |
| [morpheus_max_hosts_policy](docs/resources/max_hosts_policy.md) | Morpheus max hosts policy resource |
| [morpheus_max_memory_policy](docs/resources/max_memory_policy.md) | Morpheus max memory policy resource |
| [morpheus_max_storage_policy](docs/resources/max_storage_policy.md) | Morpheus max storage policy resource |
| [morpheus_max_vms_policy](docs/resources/max_vms_policy.md) | Morpheus max vms policy resource |
| [morpheus_network_domain](docs/resources/network_domain.md) | Morpheus network domain resource |
| [morpheus_network_quota_policy](docs/resources/network_quota_policy.md) | Morpheus network quota policy resource |
| [morpheus_node_type](docs/resources/node_type.md) | Morpheus node_type resource |
| [morpheus_number_option_type](docs/resources/number_option_type.md) | Morpheus number option type resource |
| [morpheus_operational_workflow](docs/resources/operational_workflow.md) | Morpheus operational automation workflow resource |
| [morpheus_password_option_type](docs/resources/password_option_type.md) | Morpheus password option type resource |
| [morpheus_powershell_script_task](docs/resources/powershell_script_task.md) | Morpheus powershell script task resource |
| [morpheus_price](docs/resources/price.md) | Morpheus price resource |
| [morpheus_price_set](docs/resources/price_set.md) | Morpheus price set resource |
| [morpheus_provisiong_workflow](docs/resources/provisioning_workflow.md) | Morpheus provisioning automation workflow resource |
| [morpheus_python_script_task](docs/resources/python_script_task.md) | Morpheus python script automation task resource |
| [morpheus_rest_option_list](docs/resources/rest_option_list.md) | Morpheus REST API option list resource |
| [morpheus_restart_task](docs/resources/restart_task.md) | Morpheus restart task resource |
| [morpheus_router_quota_policy](docs/resources/router_quota_policy.md) | Morpheus router quota policy resource for configuring router quotas based upon the group, cloud, role, user or globally |
| [morpheus_ruby_script_task](docs/resources/ruby_script_task.md) | Morpheus ruby script task resource |
| [morpheus_scale_threshold](docs/resources/scale_threshold.md) | Morpheus scale threshold resource |
| [morpheus_script_template](docs/resources/script_template.md) | Morpheus script template resource |
| [morpheus_select_list_option_type](docs/resources/select_list_option_type.md) | Morpheus select list option type resource |
| [morpheus_service_plan](docs/resources/service_plan.md) | Morpheus service plan resource |
| [morpheus_shell_script_task](docs/resources/shell_script_task.md) | Morpheus shell script task resource |
| [morpheus_task_job](docs/resources/task_job.md) | Morpheus task job resource for scheduling automation tasks |
| [morpheus_tenant](docs/resources/tenant.md) | Morpheus tenant resource |
| [morpheus_terraform_app_blueprint](docs/resources/terraform_app_blueprint.md) | Morpheus Terraform app blueprint resource |
| [morpheus_terraform_spec_template](docs/resources/terraform_spec_template.md) | Morpheus Terraform spec template resource |
| [morpheus_text_option_type](docs/resources/text_option_type.md) | Morpheus text option type resource |
| [morpheus_typeahead_option_type](docs/resources/typeahead_option_type.md) | Morpheus typeahead option type resource |
| [morpheus_user_creation_policy](docs/resources/user_creation_policy.md) | Morpheus user creation policy resource for configuring user creation based upon the group, cloud, role, user or globally |
| [morpheus_vsphere_cloud](docs/resources/vsphere_cloud.md) | Morpheus VMware vSphere cloud resource |
| [morpheus_vsphere_instance](docs/resources/vsphere_instance.md) | Morpheus VMware vSphere instance resource |
| [morpheus_wiki_page](docs/resources/wiki_page.md) | Morpheus wiki page resource for creating and managing wiki pages |
| [morpheus_workflow_catalog_item](docs/resources/workflow_catalog_item.md) | Morpheus workflow catalog item resource for creating and managing operational workflow catalog items |
| [morpheus_workflow_policy](docs/resources/workflow_policy.md) | Morpheus workflow policy resource for assigning a workflow to a group, cloud, role, user or globally |
| [morpheus_write_attributes_task](docs/resources/write_attributes_task.md) | Morpheus write attributes task resource for storing values from XaaS instance phases |

## Supported Data Sources
----------------------

The following list of data sources are supported by the Morpheus Terraform provider:

| Data Source Name | Description |
|------------------|-------------|
| [morpheus_blueprint](docs/data-sources/blueprint.md) | Morpheus blueprint data source |
| [morpheus_budget](docs/data-sources/budget.md) | Morpheus budget data source |
| [morpheus_cloud](docs/data-sources/cloud.md) | Morpheus cloud data source |
| [morpheus_contact](docs/data-sources/contact.md) | Morpheus contact data source |
| [morpheus_credential](docs/data-sources/credential.md) | Morpheus credential data source |
| [morpheus_environment](docs/data-sources/environment.md) | Morpheus environment data source|
| [morpheus_execute_schedule](docs/data-sources/execute_schedule.md) | Morpheus execute schedule data source |
| [morpheus_file_template](docs/data-sources/file_template.md) | Morpheus file template data source |
| [morpheus_group](docs/data-sources/group.md) | Morpheus group data source |
| [morpheus_instance_layout](docs/data-sources/instance_layout.md) | Morpheus isntance layout data source |
| [morpheus_instance_type](docs/data-sources/instance_type.md) | Morpheus instance type data source |
| [morpheus_integration](docs/data-sources/integration.md) | Morpheus integration data source |
| [morpheus_job](docs/data-sources/job.md) | Morpheus job data source |
| [morpheus_network](docs/data-sources/network.md) | Morpheus network data source |
| [morpheus_node_type](docs/data-sources/node_type.md) | Morpheus node type data source |
| [morpheus_option_list](docs/data-sources/option_list.md) | Morpheus option list data source |
| [morpheus_option_type](docs/data-sources/option_type.md) | Morpheus option type data source |
| [morpheus_plan](docs/data-sources/plan.md) | Morpheus plan data source |
| [morpheus_policy](docs/data-sources/policy.md) | Morpheus policy data source |
| [morpheus_power_schedule](docs/data-sources/power_schedule.md) | Morpheus power schedule data source |
| [morpheus_price](docs/data-sources/price.md) | Morpheus price data source |
| [morpheus_price_set](docs/data-sources/price_set.md) | Morpheus price set data source |
| [morpheus_resource_pool](docs/data-sources/resource_pool.md) | Morpheus resources pool data source |
| [morpheus_script_template](docs/data-sources/script_template.md) | Morpheus script template data source |
| [morpheus_spec_template](docs/data-sources/spec_template.md) | Morpheus spec template data source |
| [morpheus_task](docs/data-sources/task.md) | Morpheus automation task data source |
| [morpheus_tenant_role](docs/data-sources/tenant_role.md) | Morpheus automation tenant role data source |
| [morpheus_tenant](docs/data-sources/tenant.md) | Morpheus automation tenant data source |
| [morpheus_virtual_image](docs/data-sources/virtual_image.md) | Morpheus virtual image data source |
| [morpheus_workflow](docs/data-sources/workflow.md) | Morpheus workflow data source |

## Building the provider
-------------------------

Clone repository to: `$GOPATH/src/github.com/gomorpheus/terraform-provider-morpheus`

```sh
mkdir -p $GOPATH/src/github.com/gomorpheus; cd $GOPATH/src/github.com/gomorpheus
git clone git@github.com:gomorpheus/terraform-provider-morpheus
```

As an alternative to cloning manually, you can use `go get`:

```sh
go get -v github.com/gomorpheus/terraform-provider-morpheus/...
```

Enter the provider directory.

```sh
cd $GOPATH/src/github.com/gomorpheus/terraform-provider-morpheus
```

Build the provider using `make dev`. This will place the provider onto your system in a [Terraform 0.13-compliant](https://www.terraform.io/upgrade-guides/0-13.html#in-house-providers) manner.

```bash
make dev
```

You'll need to ensure that your Terraform file contains the information necessary to find the plugin when running `terraform init`. `make dev` will use a version number of 0.0.1, so the following block will work:

```hcl
terraform {
  required_providers {
    morpheus = {
      source = "localhost/providers/morpheus"
      version = "0.0.1"
    }
  }
}
```

## Generating Docs
----------------------
From the root of the repo run:

```
go run github.com/hashicorp/terraform-plugin-docs/cmd/tfplugindocs
```

## Developing the provider
-------------------------

See the [`contributing`](contributing/) directory for more developer documentation.
