---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "timescale_service Data Source - terraform-provider-timescale"
subcategory: ""
description: |-
  Service data source
---

# timescale_service (Data Source)

Service data source



<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `id` (String) Service ID is the unique identifier for this service

### Read-Only

- `created` (String) Created is the time this service was created.
- `name` (String) Service Name is the configurable name assigned to this resource. If none is provided, a default will be generated by the provider.
- `region_code` (String) Region Code is the physical data center where this service is located.
- `resources` (Attributes List) (see [below for nested schema](#nestedatt--resources))
- `spec` (Attributes) (see [below for nested schema](#nestedatt--spec))

<a id="nestedatt--resources"></a>
### Nested Schema for `resources`

Read-Only:

- `id` (String)
- `spec` (Attributes) (see [below for nested schema](#nestedatt--resources--spec))

<a id="nestedatt--resources--spec"></a>
### Nested Schema for `resources.spec`

Read-Only:

- `memory_gb` (Number) MemoryGB is the memory allocated for this service.
- `milli_cpu` (Number) MilliCPU is the cpu allocated for this service.
- `storage_gb` (Number) StorageGB is the storage allocated for this service.



<a id="nestedatt--spec"></a>
### Nested Schema for `spec`

Read-Only:

- `hostname` (String) Hostname is the hostname of this service.
- `port` (Number) Port is the port assigned to this service.
- `username` (String) Username is the Postgres username.

