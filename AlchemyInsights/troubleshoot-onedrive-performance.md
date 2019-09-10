---
title: OneDrive 性能疑难解答
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 222f818c3fd78a19b9952d4703755498bc080910
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822188"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="519a9-102">OneDrive 性能疑难解答</span><span class="sxs-lookup"><span data-stu-id="519a9-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="519a9-103">如果你遇到的速度比预期同步慢，或 OneDrive 中的类似性能问题：</span><span class="sxs-lookup"><span data-stu-id="519a9-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="519a9-104">使用 "[服务运行状况" 仪表板](https://portal.office.com/adminportal/home?ref=/servicehealth)确认是否存在已知问题。</span><span class="sxs-lookup"><span data-stu-id="519a9-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="519a9-105">[按需启用文件](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-US&rs=en-US&ad=US)，以便您可以访问 OneDrive 中的所有文件，而无需下载所有文件并使用设备上的存储空间。</span><span class="sxs-lookup"><span data-stu-id="519a9-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-US&rs=en-US&ad=US) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="519a9-106">查看网络规划和性能的[最佳实践](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance)。</span><span class="sxs-lookup"><span data-stu-id="519a9-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="519a9-107">[最大限度地提高上载和下载速度](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43)，尤其是在第一次同步设备时。</span><span class="sxs-lookup"><span data-stu-id="519a9-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="519a9-108">如果要同步的库包含100000以上的项目，则 OneDrive 同步可能会在很长一段时间内停滞，或者该状态显示 xMB 的 "处理 0KB"。</span><span class="sxs-lookup"><span data-stu-id="519a9-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="519a9-109">[了解有关同步超过100000个文件](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa)以及[OneDrive 支持的300000文件限制的](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa)详细信息。</span><span class="sxs-lookup"><span data-stu-id="519a9-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="519a9-p102">当用户超过使用限制时，SharePoint Online 会限制该用户帐户发出的任何进一步请求，但通常只是短时间内。在用户限制的有效期内，将限制该用户的所有用户操作。</span><span class="sxs-lookup"><span data-stu-id="519a9-p102">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period. All user actions are throttled while the throttle is in effect.</span></span>
