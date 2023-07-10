# VdcComputePolicy

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | UUID for vDC compute policy. This is immutable.  | [optional] [default to null]
**Description** | **string** |  | [optional] [default to null]
**Name** | **string** | Display name.  | [default to null]
**CpuSpeed** | **int64** | The CPU speed in MHz of this VM. This is optional. When provided, VMs with this policy cannot have more than CPU speed defined by this field.  | [optional] [default to null]
**Memory** | **int64** | The maximum memory in MB allowed for a VM. This is optional. When provided, VMs with this policy cannot have configured memory more than defined by this field.  | [optional] [default to null]
**CpuCount** | **int32** | The maximum number of CPUs allowed for a VM. This is optional. When provided, VMs with this policy cannot have more than number of CPUs defined by this field.  | [optional] [default to null]
**CoresPerSocket** | **int32** | The cores per socket to be configured for the VM where this policy is applied.  | [optional] [default to null]
**MemoryReservationGuarantee** | **float64** | The factor of the configured memory reserved for the VM on which this policy is applied.  | [optional] [default to null]
**CpuReservationGuarantee** | **float64** | The factor of the configured CPU reserved for the VM on which this policy is applied.  | [optional] [default to null]
**CpuLimit** | **int64** | The limit of CPU in MHz for the VM on which this policy is applied. -1 means unlimited. This is optional. If not provided, limit would be equal to the vCPUSpeed multiplied by numCPU.  | [optional] [default to null]
**MemoryLimit** | **int64** | The limit of memory in MB for the VM on which this policy is applied. -1 means unlimited. This is optional. If not provided, limit would be equal to the configured memory of the VM.  | [optional] [default to null]
**CpuShares** | **int32** | The number of CPU shares for the VM on which this policy is applied. This is optional. If not provided, Normal shares would be applied to the VM.  | [optional] [default to null]
**MemoryShares** | **int32** | The number of memory shares for the VM on which this policy is applied. This is optional. If not provided, Normal shares would be applied to the VM.  | [optional] [default to null]
**ExtraConfigs** | **map[string]string** | Map of extra configs to be set on the VM with this policy.  | [optional] [default to null]
**PvdcComputePolicyRef** | [***EntityReference**](EntityReference.md) | Deprecated in Api 32.0, this property will be removed in future release.  | [optional] [default to null]
**PvdcComputePolicy** | [***EntityReference**](EntityReference.md) | This field cannot be updated and is a read-only field in the client after creation.  | [optional] [default to null]
**CompatibleVdcTypes** | **[]string** | A list of read-only compatible vDC types for this policy. | [optional] [default to null]
**IsSizingOnly** | **bool** | This field cannot be updated and is a read-only field in the client after creation. It defines whether the policy is SIZING_ONLY or if it also contains affinity information.  | [optional] [default to null]
**PvdcId** | **string** | URN for Provider VDC.  | [optional] [default to null]
**NamedVmGroups** | [**[][]EntityReference**](array.md) | List of list of vmGroups grouped together in a meaningful manner. A group of vmGroups would consist of one functionally equal vmGroup picked from each cluster of the pvdc.  | [optional] [default to null]
**LogicalVmGroupReferences** | [**[]EntityReference**](EntityReference.md) | List of logical vm group references. This value is set at creation time and cannot be edited later.  | [optional] [default to null]
**IsAutoGenerated** | **bool** | This field cannot be updated and is a read-only field in the client. It defines if the policy is auto-generated.  | [optional] [default to null]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

