---
title: 日志和报告
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50031494"
---
# <a name="logs-and-reporting"></a><span data-ttu-id="11a22-102">日志和报告</span><span class="sxs-lookup"><span data-stu-id="11a22-102">Logs and Reporting</span></span>

<span data-ttu-id="11a22-103">[Azure Active Directory 报告常见问题解答](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) 了有关 Azure Active Directory (Azure AD) 报告。</span><span class="sxs-lookup"><span data-stu-id="11a22-103">[Azure Active Directory reporting FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) answers frequently asked questions about Azure Active Directory (Azure AD) reporting.</span></span> <span data-ttu-id="11a22-104">有关详细信息，请参阅 [Azure Active Directory 报告](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports)。</span><span class="sxs-lookup"><span data-stu-id="11a22-104">For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span></span>

<span data-ttu-id="11a22-105">**审核问题疑难解答**</span><span class="sxs-lookup"><span data-stu-id="11a22-105">**Troubleshooting issues with Audit**</span></span>

1. <span data-ttu-id="11a22-106">如果你在看到某些审核活动时遇到问题，并且此列表中缺少活动，请[](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)提交支持票证。</span><span class="sxs-lookup"><span data-stu-id="11a22-106">If you are having issues seeing some audit activities and the missing Activity is in this [list](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), please file a support ticket.</span></span>
2. <span data-ttu-id="11a22-107">如果在查看租户中任何审核日志时遇到问题，请提交支持票证。</span><span class="sxs-lookup"><span data-stu-id="11a22-107">If you are having issues seeing any Audit logs in your tenant, please file a support ticket.</span></span>
3. <span data-ttu-id="11a22-108">如果你的审核活动未立即显示在 Azure 门户中，请查看我们的延迟信息[](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies)，如果延迟超过记录延迟，请提交支持票证。</span><span class="sxs-lookup"><span data-stu-id="11a22-108">If your audit activities are not showing up immediately in the Azure Portal, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. [<span data-ttu-id="11a22-109">Azure AD 活动日志保留</span><span class="sxs-lookup"><span data-stu-id="11a22-109">Azure AD Activity Logs Retention</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. <span data-ttu-id="11a22-110">如果你未看到所选日期范围的所有审核，你最多可以下载 250，000 行 (Azure 门户中的最近) 登录排序。</span><span class="sxs-lookup"><span data-stu-id="11a22-110">If you don't see all the audit for the date range you selected, you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="11a22-111">有关详细信息，请参阅审核 [活动下载](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report)。</span><span class="sxs-lookup"><span data-stu-id="11a22-111">For more information, see [Audit activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span></span>

<span data-ttu-id="11a22-112">**登录问题疑难解答**</span><span class="sxs-lookup"><span data-stu-id="11a22-112">**Troubleshooting issues with Sign-ins**</span></span>

1. <span data-ttu-id="11a22-113">如果你拥有租户的 Azure AD Premium (P1 或 P2) ，你只能看到过去 30 天的数据。</span><span class="sxs-lookup"><span data-stu-id="11a22-113">You can only see the last 30 days of data if you have an Azure AD Premium (P1 or P2) license for your tenant.</span></span>
2. <span data-ttu-id="11a22-114">登录仅适用于 Azure AD Premium 租户。</span><span class="sxs-lookup"><span data-stu-id="11a22-114">Sign-ins are available only for Azure AD Premium tenants.</span></span> <span data-ttu-id="11a22-115">它不适用于免费或基本许可租户。</span><span class="sxs-lookup"><span data-stu-id="11a22-115">It's not available for Free or Basic licensed tenants.</span></span>
3. <span data-ttu-id="11a22-116">如果你的租户具有高级 P1 许可证，但看不到登录，请查看我们的延迟信息，如果延迟超过记录[](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies)延迟，请提交支持票证。</span><span class="sxs-lookup"><span data-stu-id="11a22-116">If your tenant has a Premium P1 license and you can't see the sign-ins, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. <span data-ttu-id="11a22-117">如果你未看到所选日期范围的所有登录，请注意，你最多可以下载 250，000 行 (从 Azure 门户按最近) 登录排序。</span><span class="sxs-lookup"><span data-stu-id="11a22-117">If you don't see all the sign-ins for the date range you selected, note that you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="11a22-118">有关详细信息，请参阅登录 [活动下载](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities)。</span><span class="sxs-lookup"><span data-stu-id="11a22-118">For more information, see [Sign-ins activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span></span>

<span data-ttu-id="11a22-119">**安全报告 (有风险、有风险登录的用户)**</span><span class="sxs-lookup"><span data-stu-id="11a22-119">**Troubleshoot Security Reports (Users Flagged at Risk, Risky Sign-In)**</span></span>

1. [<span data-ttu-id="11a22-120">标记为风险安全报告的用户</span><span class="sxs-lookup"><span data-stu-id="11a22-120">Users flagged for risk security report</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [<span data-ttu-id="11a22-121">Azure Active Directory 门户中的有风险登录报告</span><span class="sxs-lookup"><span data-stu-id="11a22-121">Risky sign-ins report in the Azure Active Directory portal</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [<span data-ttu-id="11a22-122">Azure Active Directory 风险事件</span><span class="sxs-lookup"><span data-stu-id="11a22-122">Azure Active Directory risk events</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
