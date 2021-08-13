---
title: 性能OneDrive疑难解答
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 15d9067e6b55b91af312671db9209f93ffc58859aaf69d63c84dbc354aff3dd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939117"
---
# <a name="troubleshoot-onedrive-performance"></a>性能OneDrive疑难解答

如果同步速度低于预期，或遇到类似的性能问题，OneDrive：

- 使用服务运行状况仪表板确认 [没有已知问题](https://portal.office.com/adminportal/home?ref=/servicehealth)。

- [启用文件按需](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e)，以便你可以访问所有文件OneDrive而无需下载所有文件并使用你的设备的存储空间。

- [查看网络](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) 规划和性能的最佳实践。

- [最大程度地提高上传](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43)和下载速度，尤其是在第一次同步设备时。

- 如果同步的库包含的项目超过 100，000 个，OneDrive 同步可能会长时间卡住，或者状态显示"正在处理 0KB 的 xMB"。 [详细了解如何同步超过 100，000](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa)个文件，OneDrive支持[300，000](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa)个文件的限制。

- 当用户超过使用限制时，SharePoint Online 会限制该用户帐户发出的任何进一步请求，但通常只是短时间内。在用户限制的有效期内，将限制该用户的所有用户操作。
