---
title: Four Character Code Surface Stability Test (WoW64)
description: Four Character Code Surface Stability Test (WoW64)
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 15ea5024-b39c-455c-a5d5-f38a40dcb796
---

# <span id="p_hlk_test.3e108dad-b2ef-4fa5-8ffc-c0e98bbebfc4"></span>Four Character Code Surface Stability Test (WoW64)


This automated test verifies the requirements listed in the test details table.

## Test details
|||
|---|---|
| **Specifications**  | <ul><li>Device.Graphics.WDDM.DisplayRender.Stability</li><li>Device.Graphics.XDDM.Stability</li></ul> |  
| **Platforms**   | <ul><li>Windows 10, client editions (x64)</li><li>Windows Server 2016 (x64)</li><li>Windows 10, client editions (ARM64)</li></ul> |
| **Supported Releases** | <ul><li>Windows 10</li><li>Windows 10, version 1511</li><li>Windows 10, version 1607</li><li>Windows 10, version 1703</li><li>Windows 10, version 1709</li></ul> |
|**Expected run time (in minutes)**| 5 |
|**Category**| Compatibility |
|**Timeout (in minutes)**| 300 |
|**Requires reboot**| false |
|**Requires special configuration**| false |
|**Type**| automatic |

 

## <span id="Additional_documentation"></span><span id="additional_documentation"></span><span id="ADDITIONAL_DOCUMENTATION"></span>Additional documentation


Tests in this feature area might have additional documentation, including prerequisites, setup, and troubleshooting information, that can be found in the following topic(s):

-   [Device.Graphics additional documentation](device-graphics-additional-documentation.md)

## <span id="Running_the_test"></span><span id="running_the_test"></span><span id="RUNNING_THE_TEST"></span>Running the test


Before you run the test, complete the test setup as described in the test requirements: [Graphic Adapter or Chipset Testing Prerequisites](graphic-adapter-or-chipset-testing-prerequisites.md).

## <span id="Troubleshooting"></span><span id="troubleshooting"></span><span id="TROUBLESHOOTING"></span>Troubleshooting


For generic troubleshooting of HLK test failures, see [Troubleshooting Windows HLK Test Failures](..\user\troubleshooting-windows-hlk-test-failures.md).

For troubleshooting information, see [Troubleshooting Device.Graphics Testing](troubleshooting-devicegraphics-testing.md).

## <span id="More_information"></span><span id="more_information"></span><span id="MORE_INFORMATION"></span>More information


### <span id="Command_syntax"></span><span id="command_syntax"></span><span id="COMMAND_SYNTAX"></span>Command syntax

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Command option</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>FourCC.exe -!fpucheck -M:[Monitor]</strong></p></td>
<td><p>Runs the test.</p></td>
</tr>
</tbody>
</table>

>[!NOTE]
>  
For command-line help for this test binary, type **/h**.

 

### <span id="File_list"></span><span id="file_list"></span><span id="FILE_LIST"></span>File list

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>File</th>
<th>Location</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>FourCC.exe</p></td>
<td><p><em>&lt;[testbinroot]&gt;</em>\nttest\windowstest\graphics\d3d\stress\</p></td>
</tr>
</tbody>
</table>

 

### <span id="Parameters"></span><span id="parameters"></span><span id="PARAMETERS"></span>Parameters

| Parameter name               | Parameter description                                 |
|------------------------------|-------------------------------------------------------|
| **MONITOR**                  | Index of display output to target with test           |
| **MODIFIEDCMDLINE**          | Additional command line arguments for test executable |
| **LLU\_NetAccessOnly**       | LLU Name of net user                                  |
| **ConfigDisplayCommandLine** | Custom Command Line for ConfigDisplay. Default: logo  |
| **TDRArgs**                  | /get or /set                                          |

 

 

 





