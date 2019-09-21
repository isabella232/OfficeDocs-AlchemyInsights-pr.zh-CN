---
title: 经典 SharePoint 审核日志报告
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068013"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="771eb-102">SharePoint 和 OneDrive 审核日志</span><span class="sxs-lookup"><span data-stu-id="771eb-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="771eb-103">**SharePoint 和 OneDrive 新式统一审核日志与合规性**</span><span class="sxs-lookup"><span data-stu-id="771eb-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="771eb-104">打开/关闭统一审核日志记录</span><span class="sxs-lookup"><span data-stu-id="771eb-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="771eb-105">SharePoint 或 OneDrive 中不需要其他配置。</span><span class="sxs-lookup"><span data-stu-id="771eb-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="771eb-106">使用审核日志搜索检查文件、文件夹、用户、权限的活动的活动：</span><span class="sxs-lookup"><span data-stu-id="771eb-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="771eb-107">文件和页面活动</span><span class="sxs-lookup"><span data-stu-id="771eb-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="771eb-108">文件夹活动</span><span class="sxs-lookup"><span data-stu-id="771eb-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="771eb-109">共享和访问请求活动</span><span class="sxs-lookup"><span data-stu-id="771eb-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="771eb-110">同步活动</span><span class="sxs-lookup"><span data-stu-id="771eb-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="771eb-111">网站管理活动</span><span class="sxs-lookup"><span data-stu-id="771eb-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="771eb-112">有关如何检索这些事件的详细信息，请参阅[Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)。</span><span class="sxs-lookup"><span data-stu-id="771eb-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="771eb-113">**SharePoint 经典审核日志**</span><span class="sxs-lookup"><span data-stu-id="771eb-113">**SharePoint classic Audit logs**</span></span>

<span data-ttu-id="771eb-114">我们已将 SPO 旧审核迁移到统一审核日志（UAL）。</span><span class="sxs-lookup"><span data-stu-id="771eb-114">We migrated SPO legacy auditing to Unified Audit Log (UAL).</span></span> <span data-ttu-id="771eb-115">这实际上意味着所有 SPO 的旧审核报告现在都将通过 UAL 供电，旧的审核信号已迁移到 UAL。</span><span class="sxs-lookup"><span data-stu-id="771eb-115">This essentially means that all SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="771eb-116">关键更改：</span><span class="sxs-lookup"><span data-stu-id="771eb-116">Key changes:</span></span>

- <span data-ttu-id="771eb-117">无法使用修整功能。</span><span class="sxs-lookup"><span data-stu-id="771eb-117">Trimming as a capability is NOT available.</span></span>
- <span data-ttu-id="771eb-118">您在其中选择要审核的特定事件的部分不可用。</span><span class="sxs-lookup"><span data-stu-id="771eb-118">The section where you choose specific events to audit is NOT available.</span></span> <span data-ttu-id="771eb-119">有关默认情况下可用的已审核事件的完整列表，请参阅[本文档](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)。</span><span class="sxs-lookup"><span data-stu-id="771eb-119">Please refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
- <span data-ttu-id="771eb-120">"**自定义报告**" 下的 "位置" 选项不可用。</span><span class="sxs-lookup"><span data-stu-id="771eb-120">The "Location" option under **Customized reports** is NOT available.</span></span> 
- <span data-ttu-id="771eb-121">"打开或下载文档" 事件不可用。</span><span class="sxs-lookup"><span data-stu-id="771eb-121">“Opening or downloading documents” events is NOT available.</span></span> 

