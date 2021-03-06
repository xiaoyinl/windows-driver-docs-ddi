---
UID: NS:fltkernel._FLT_PARAMETERS
title: _FLT_PARAMETERS (fltkernel.h)
description: The FLT_PARAMETERS union defines the request-type-specific parameters associated with an I/O operation.
old-location: ifsk\flt_parameters.htm
tech.root: ifsk
ms.assetid: 62aa20b7-ce5c-4d42-bce2-1d76a98887ed
ms.date: 10/07/2019
ms.keywords: "*PFLT_PARAMETERS, FLT_PARAMETERS, FLT_PARAMETERS union [Installable File System Drivers], FltSystemStructures_2ebb0ec7-76cc-49a3-b2ec-186f67369bbb.xml, PFLT_PARAMETERS, PFLT_PARAMETERS union pointer [Installable File System Drivers], _FLT_PARAMETERS, fltkernel/FLT_PARAMETERS, fltkernel/PFLT_PARAMETERS, ifsk.flt_parameters"
ms.topic: struct
f1_keywords:
 - "fltkernel/FLT_PARAMETERS"
req.header: fltkernel.h
req.include-header: Fltkernel.h
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- HeaderDef
api_location:
- fltkernel.h
api_name:
- FLT_PARAMETERS
product:
- Windows
targetos: Windows
req.typenames: FLT_PARAMETERS, *PFLT_PARAMETERS
---

# _FLT_PARAMETERS structure

## -description

The FLT_PARAMETERS union defines the request-type-specific parameters associated with an I/O operation. The **Members** section of this reference page simply lists all structures within the union along with their members. See [**Remarks**](#remarks) for descriptions.

## -struct-fields

## -remarks

The FLT_PARAMETERS structure is stored in the **Parameters** field of the [FLT_IO_PARAMETER_BLOCK](https://docs.microsoft.com/windows-hardware/drivers/ddi/content/fltkernel/ns-fltkernel-_flt_io_parameter_block) structure for the operation. (A pointer to the FLT_IO_PARAMETER_BLOCK structure is stored in the **Iopb** field of the [FLT_CALLBACK_DATA](https://docs.microsoft.com/windows-hardware/drivers/ddi/content/fltkernel/ns-fltkernel-_flt_callback_data) structure for the operation.)

For the specific FLT_PARAMETERS union component used in each type of I/O operation, see the following reference entries.

| IRP | Reference Page |
| --- | -------------- |
| IRP_MJ_CREATE | [FLT_PARAMETERS for IRP_MJ_CREATE](https://docs.microsoft.com/windows-hardware/drivers/ifs/flt-parameters-for-irp-mj-create) |
| IRP_MJ_DEVICE_IO_CONTROL | [FLT_PARAMETERS for IRP_MJ_DEVICE_CONTROL and IRP_MJ_INTERNAL_DEVICE_CONTROL](https://docs.microsoft.com/windows-hardware/drivers/ifs/flt-parameters-for-irp-mj-device-control-and-irp-mj-internal-device-co) |
| IRP_MJ_DIRECTORY_CONTROL | [FLT_PARAMETERS for IRP_MJ_DIRECTORY_CONTROL](https://docs.microsoft.com/windows-hardware/drivers/ifs/flt-parameters-for-irp-mj-directory-control) |
| IRP_MJ_FILE_SYSTEM_CONTROL | [FLT_PARAMETERS for IRP_MJ_FILE_SYSTEM_CONTROL](https://docs.microsoft.com/windows-hardware/drivers/ifs/flt-parameters-for-irp-mj-file-system-control) |
| IRP_MJ_INTERNAL_DEVICE_IO_CONTROL | [FLT_PARAMETERS for IRP_MJ_DEVICE_CONTROL and IRP_MJ_INTERNAL_DEVICE_CONTROL](https://docs.microsoft.com/windows-hardware/drivers/ifs/flt-parameters-for-irp-mj-device-control-and-irp-mj-internal-device-co) |
| IRP_MJ_LOCK_CONTROL | [FLT_PARAMETERS for IRP_MJ_LOCK_CONTROL](https://docs.microsoft.com/windows-hardware/drivers/ifs/flt-parameters-for-irp-mj-lock-control) |
| IRP_MJ_PNP | [FLT_PARAMETERS for IRP_MJ_PNP](https://docs.microsoft.com/windows-hardware/drivers/ifs/flt-parameters-for-irp-mj-pnp) |
| IRP_MJ_QUERY_EA | [FLT_PARAMETERS for IRP_MJ_QUERY_EA](https://docs.microsoft.com/windows-hardware/drivers/ifs/flt-parameters-for-irp-mj-query-ea) |
| IRP_MJ_QUERY_INFORMATION | [FLT_PARAMETERS for IRP_MJ_QUERY_INFORMATION](https://docs.microsoft.com/windows-hardware/drivers/ifs/flt-parameters-for-irp-mj-query-information) |
| IRP_MJ_QUERY_QUOTA | [FLT_PARAMETERS for IRP_MJ_QUERY_QUOTA](https://docs.microsoft.com/windows-hardware/drivers/ifs/flt-parameters-for-irp-mj-query-quota) |
| IRP_MJ_QUERY_SECURITY | [FLT_PARAMETERS for IRP_MJ_QUERY_SECURITY](https://docs.microsoft.com/windows-hardware/drivers/ifs/flt-parameters-for-irp-mj-query-security) |
| IRP_MJ_QUERY_VOLUME_INFORMATION | [FLT_PARAMETERS for IRP_MJ_QUERY_VOLUME_INFORMATION](https://docs.microsoft.com/windows-hardware/drivers/ifs/flt-parameters-for-irp-mj-query-volume-information) |
| IRP_MJ_READ | [FLT_PARAMETERS for IRP_MJ_READ](https://docs.microsoft.com/windows-hardware/drivers/ifs/flt-parameters-for-irp-mj-read) |
| IRP_MJ_SET_EA | [FLT_PARAMETERS for IRP_MJ_SET_EA](https://docs.microsoft.com/windows-hardware/drivers/ifs/flt-parameters-for-irp-mj-set-ea) |
| IRP_MJ_SET_INFORMATION | [FLT_PARAMETERS for IRP_MJ_SET_INFORMATION](https://docs.microsoft.com/windows-hardware/drivers/ifs/flt-parameters-for-irp-mj-set-information) |
| IRP_MJ_SET_QUOTA | [FLT_PARAMETERS for IRP_MJ_SET_QUOTA](https://docs.microsoft.com/windows-hardware/drivers/ifs/flt-parameters-for-irp-mj-set-quota) |
| IRP_MJ_SET_SECURITY | [FLT_PARAMETERS for IRP_MJ_SET_SECURITY](https://docs.microsoft.com/windows-hardware/drivers/ifs/flt-parameters-for-irp-mj-set-security) |
| IRP_MJ_SET_VOLUME_INFORMATION | [FLT_PARAMETERS for IRP_MJ_SET_VOLUME_INFORMATION](https://docs.microsoft.com/windows-hardware/drivers/ifs/flt-parameters-for-irp-mj-set-volume-information) |
| IRP_MJ_WRITE | [FLT_PARAMETERS for IRP_MJ_WRITE](https://docs.microsoft.com/windows-hardware/drivers/ifs/flt-parameters-for-irp-mj-write) |
| IRP_MJ_ACQUIRE_FOR_MOD_WRITE | [FLT_PARAMETERS for IRP_MJ_ACQUIRE_FOR_MOD_WRITE](https://docs.microsoft.com/windows-hardware/drivers/ifs/flt-parameters-for-irp-mj-acquire-for-mod-write) |
| IRP_MJ_ACQUIRE_FOR_CC_FLUSH | This I/O operation does not have parameters. |
| IRP_MJ_ACQUIRE_FOR_SECTION_SYNCHRONIZATION | [FLT_PARAMETERS for IRP_MJ_ACQUIRE_FOR_SECTION_SYNCHRONIZATION](https://docs.microsoft.com/windows-hardware/drivers/ifs/flt-parameters-for-irp-mj-acquire-for-section-synchronization) |
| IRP_MJ_CLEANUP | This I/O operation does not have parameters. |
| IRP_MJ_CLOSE   | This I/O operation does not have parameters. |
| IRP_MJ_QUERY_OPEN | [FLT_PARAMETERS for IRP_MJ_QUERY_OPEN](https://docs.microsoft.com/windows-hardware/drivers/ifs/flt-parameters-for-irp-mj-query-open) |
| IRP_MJ_FAST_IO_CHECK_IF_POSSIBLE] | [FLT_PARAMETERS for IRP_MJ_FAST_IO_CHECK_IF_POSSIBLE](https://docs.microsoft.com/windows-hardware/drivers/ifs/flt-parameters-for-irp-mj-fast-io-check-if-possible) |
| IRP_MJ_FLUSH_BUFFERS   | This I/O operation does not have parameters. |
| IRP_MJ_MDL_READ | [FLT_PARAMETERS for IRP_MJ_MDL_READ](https://docs.microsoft.com/windows-hardware/drivers/ifs/flt-parameters-for-irp-mj-mdl-read) |
| IRP_MJ_MDL_READ_COMPLETE | [FLT_PARAMETERS for IRP_MJ_MDL_READ_COMPLETE](https://docs.microsoft.com/windows-hardware/drivers/ifs/flt-parameters-for-irp-mj-mdl-read-complete) |
| IRP_MJ_MDL_WRITE_COMPLETE | [FLT_PARAMETERS for IRP_MJ_MDL_WRITE_COMPLETE](https://docs.microsoft.com/windows-hardware/drivers/ifs/flt-parameters-for-irp-mj-mdl-write-complete) |
| IRP_MJ_NETWORK_QUERY_OPEN | [FLT_PARAMETERS for IRP_MJ_NETWORK_QUERY_OPEN](https://docs.microsoft.com/windows-hardware/drivers/ifs/flt-parameters-for-irp-mj-network-query-open) |
| IRP_MJ_PREPARE_MDL_WRITE | [FLT_PARAMETERS for IRP_MJ_PREPARE_MDL_WRITE](https://docs.microsoft.com/windows-hardware/drivers/ifs/flt-parameters-for-irp-mj-prepare-mdl-write) |
| IRP_MJ_RELEASE_FOR_CC_FLUSH   | This I/O operation does not have parameters. |
| IRP_MJ_RELEASE_FOR_MOD_WRITE | [FLT_PARAMETERS for IRP_MJ_RELEASE_FOR_MOD_WRITE](https://docs.microsoft.com/windows-hardware/drivers/ifs/flt-parameters-for-irp-mj-release-for-mod-write) |
| IRP_MJ_RELEASE_FOR_SECTION_SYNCHRONIZATION | This I/O operation does not have parameters. |
| IRP_MJ_SHUTDOWN   | This I/O operation does not have parameters. |
| IRP_MJ_VOLUME_DISMOUNT   | This I/O operation does not have parameters. |
| IRP_MJ_VOLUME_MOUNT | [FLT_PARAMETERS for IRP_MJ_VOLUME_MOUNT](https://docs.microsoft.com/windows-hardware/drivers/ifs/flt-parameters-for-irp-mj-volume-mount) |

## -see-also

[FLT_CALLBACK_DATA](https://docs.microsoft.com/windows-hardware/drivers/ddi/content/fltkernel/ns-fltkernel-_flt_callback_data)

[FLT_IO_PARAMETER_BLOCK](https://docs.microsoft.com/windows-hardware/drivers/ddi/content/fltkernel/ns-fltkernel-_flt_io_parameter_block)

[FltSetCallbackDataDirty](https://docs.microsoft.com/windows-hardware/drivers/ddi/content/fltkernel/nf-fltkernel-fltsetcallbackdatadirty)
