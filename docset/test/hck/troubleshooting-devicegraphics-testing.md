---
author: joshbax-msft
title: Troubleshooting Device.Graphics Testing
description: Troubleshooting Device.Graphics Testing
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: ed52dec7-f3c2-44ce-a731-ca502cc8a34a
---

# Troubleshooting Device.Graphics Testing


To troubleshoot issues that occur with Device.Graphic tests, follow these steps:

1.  Review [Troubleshooting Windows HCK Test Failures](troubleshooting-windows-hck-test-failures.md).

2.  Review one of the following topics, depending on the type of graphic device that you want to test:

    -   [Display Monitor Testing Prerequisites](display-monitor-testing-prerequisites.md)

    -   [Graphic Adapter or Chipset Testing Prerequisites](graphic-adapter-or-chipset-testing-prerequisites.md)

3.  For a test failure, look for usable information in the Windows HCK Studio test log. If you find usable information, resolve the issue and rerun the test.

### Specific information about DXVA testing

The DXVA tests require the following:

-   **Supplemental Content for Windows HCK Tests for DXVA and HMFT Multimedia Tests**: Download and install the Supplemental Content for Windows HCK Tests for DXVA and HMFT Multimedia Tests from the MSDN® website at <http://msdn.microsoft.com/windows/hardware/hh852358>.

    **Important**  
    Before running the DXVA tests on x86 or amd64 systems, you must install the Windows 8 Professional SKU and then install Windows Anytime Upgrade for Media Center, otherwise the MPEG2 tests will fail.

     

### Common errors

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Error</th>
<th>Description</th>
<th>Solution</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>ERROR&gt;&gt; Failed to find input source file.</p></td>
<td><p>Content not available to client machine.</p></td>
<td><p>Ensure that the <strong>ContentSource</strong> parameter points to the correct location of the source content at run time.</p></td>
</tr>
</tbody>
</table>

 

## Related topics


[Device.Graphics Testing](devicegraphics-testing.md)

[Troubleshooting Windows HCK](troubleshooting-windows-hck.md)

 

 






