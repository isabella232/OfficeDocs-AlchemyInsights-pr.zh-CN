---
title: 经典 SharePoint 审核日志报告
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 0aedb549f11db54d3cd480671fb0767c60680ad3
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509590"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="dfaba-102">SharePoint 和 OneDrive 审核日志</span><span class="sxs-lookup"><span data-stu-id="dfaba-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="dfaba-103">SharePoint 经典审核日志</span><span class="sxs-lookup"><span data-stu-id="dfaba-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="dfaba-104">SPO 旧版审核已迁移到统一审核日志（UAL）。</span><span class="sxs-lookup"><span data-stu-id="dfaba-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="dfaba-105">所有 SPO 的旧审核报告现在都将通过 UAL 供电，旧的审核信号已迁移到 UAL。</span><span class="sxs-lookup"><span data-stu-id="dfaba-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="dfaba-106">关键更改：</span><span class="sxs-lookup"><span data-stu-id="dfaba-106">Key changes:</span></span>

* <span data-ttu-id="dfaba-107">修整功能不可用。</span><span class="sxs-lookup"><span data-stu-id="dfaba-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="dfaba-108">选择要审核的特定事件不可用。</span><span class="sxs-lookup"><span data-stu-id="dfaba-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="dfaba-109">有关默认情况下可用的已审核事件的完整列表，请参阅[本文档](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)。</span><span class="sxs-lookup"><span data-stu-id="dfaba-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="dfaba-110">"**自定义报告**" 下的 "**位置**" 选项不可用。</span><span class="sxs-lookup"><span data-stu-id="dfaba-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="dfaba-111">"**打开或下载文档**事件" 选项不可用。</span><span class="sxs-lookup"><span data-stu-id="dfaba-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="dfaba-112">配置网站集的审核设置</span><span class="sxs-lookup"><span data-stu-id="dfaba-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="dfaba-113">SharePoint 和 OneDrive 新式统一审核日志与合规性</span><span class="sxs-lookup"><span data-stu-id="dfaba-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="dfaba-114">打开/关闭统一审核日志记录</span><span class="sxs-lookup"><span data-stu-id="dfaba-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="dfaba-115">SharePoint 或 OneDrive 中不需要其他配置。</span><span class="sxs-lookup"><span data-stu-id="dfaba-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="dfaba-116">使用审核日志搜索检查文件、文件夹、用户、权限的活动的活动：</span><span class="sxs-lookup"><span data-stu-id="dfaba-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="dfaba-117">文件和页面活动</span><span class="sxs-lookup"><span data-stu-id="dfaba-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="dfaba-118">文件夹活动</span><span class="sxs-lookup"><span data-stu-id="dfaba-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="dfaba-119">共享和访问请求活动</span><span class="sxs-lookup"><span data-stu-id="dfaba-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="dfaba-120">同步活动</span><span class="sxs-lookup"><span data-stu-id="dfaba-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="dfaba-121">网站管理活动</span><span class="sxs-lookup"><span data-stu-id="dfaba-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="dfaba-122">有关如何检索这些事件的详细信息，请参阅[Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)。</span><span class="sxs-lookup"><span data-stu-id="dfaba-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
