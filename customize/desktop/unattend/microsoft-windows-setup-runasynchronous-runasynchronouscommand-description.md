---
title: Description
description: Description
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: f44f16e9-300c-4d1e-bde2-afaf9cd28437
ms.mktglfcycl: deploy
ms.sitesec: msdn
author: alhopper-msft
ms.author: alhopper
ms.date: 05/02/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-oem
---

# Description


`Description` describes the asynchronous command to execute specified by [Path](microsoft-windows-setup-runasynchronous-runasynchronouscommand-path.md).

All [RunAsynchronous](microsoft-windows-setup-runasynchronous.md) commands run in the system context.

## Values


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><em>Command_description</em></p></td>
<td><p>Describes the command to run asynchronously during the windowsPE configuration pass. <em>Command_description</em> is a string.</p></td>
</tr>
</tbody>
</table>

 

This string type does not support empty elements. Do not create an empty value for this setting.

## Valid Passes


windowsPE

## Parent Hierarchy


[microsoft-windows-setup-](microsoft-windows-setup.md) | [RunAsynchronous](microsoft-windows-setup-runasynchronous.md) | [RunAsynchronousCommand](microsoft-windows-setup-runasynchronous-runasynchronouscommand.md) | **Description**

## Applies To


For the list of the supported Windows editions and architectures that this component supports, see [microsoft-windows-setup-](microsoft-windows-setup.md).

## XML Example


The following XML output shows how to configure asynchronous commands to run.

```
<RunAsynchronous>
   <RunAsynchronousCommand>
      <Order>1</Order>
      <Path>\\MyNetworkShare\MyApplication.exe</Path>
      <Description>DescriptionOfMyApplication</Description>
      <Credentials>
         <Domain>FabrikamDomain</Domain>
         <UserName>MyUserName</UserName>
         <Password>MyPassword</Password>
      </Credentials>
   </RunAsynchronousCommand>
   <RunAsynchronousCommand>
      <Order>2</Order>
      <Path>C:\AnotherApplication.exe</Path>
      <Description>DescriptionOfMyApplication</Description>
   </RunAsynchronousCommand>
</RunAsynchronous>
```

## Related topics


[RunAsynchronousCommand](microsoft-windows-setup-runasynchronous-runasynchronouscommand.md)

 

 







