---
title: 未传递 SharePoint 通知通知
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: e682a1b3dbd0d3a1c2e52be725dd2b57fc66109a
ms.sourcegitcommit: a2c866d2f3cdc1e18a33a5b2a4209340e83ca3c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/14/2019
ms.locfileid: "36404792"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="8bf90-102">未传递 SharePoint 通知通知</span><span class="sxs-lookup"><span data-stu-id="8bf90-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="8bf90-103">请检查电子邮件中的垃圾邮件文件夹, 有时会出现通知。</span><span class="sxs-lookup"><span data-stu-id="8bf90-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="8bf90-104">确定是否**未传递所有警报**, 或者是否未传递来自特定文件或库**的单个警报**。</span><span class="sxs-lookup"><span data-stu-id="8bf90-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="8bf90-105">**不传递单个警报**: 如果未传递来自特定文件或库的单个通知, 则可以尝试删除并重新创建它。</span><span class="sxs-lookup"><span data-stu-id="8bf90-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="8bf90-106">请参阅[管理、查看或删除 SharePoint 警报](https://support.office.com/en-us/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=en-US&ad=US#ID0EAADAAA=Online)以重新创建警报。</span><span class="sxs-lookup"><span data-stu-id="8bf90-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/en-us/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=en-US&ad=US#ID0EAADAAA=Online) to recreate the alert.</span></span>
- <span data-ttu-id="8bf90-107">**未传递所有警报**: 如果未传递来自多个文件或库的所有警报, 请访问[服务运行状况仪表板](https://admin.microsoft.com/AdminPortal/Home#/servicehealth), 以检查 SharePoint 或 Exchange 可能发生的任何咨询/事件。</span><span class="sxs-lookup"><span data-stu-id="8bf90-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="8bf90-108">问题可能与 SharePoint 通知功能或通过 Exchange 的电子邮件延迟有关。</span><span class="sxs-lookup"><span data-stu-id="8bf90-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="8bf90-109">此外, 请务必注意是否正在传递其他电子邮件, 如果没有, 则可能是 Exchange 延迟问题。</span><span class="sxs-lookup"><span data-stu-id="8bf90-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="8bf90-110">有关警报的常见问题解答:</span><span class="sxs-lookup"><span data-stu-id="8bf90-110">FAQ on alerts:</span></span>

- <span data-ttu-id="8bf90-111">无法向通讯组发送通知, 仅支持安全和 O365 组。</span><span class="sxs-lookup"><span data-stu-id="8bf90-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="8bf90-112">您不能自定义通知电子邮件模板;您需要使用 Microsoft FLOW 或 SharePoint Designer 工作流来实现这些。</span><span class="sxs-lookup"><span data-stu-id="8bf90-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

<span data-ttu-id="8bf90-113">详细信息:</span><span class="sxs-lookup"><span data-stu-id="8bf90-113">More Information:</span></span>

- <span data-ttu-id="8bf90-114">**通知设置**: 有关设置通知的详细信息, 请参阅[创建通知以在 SharePoint 中的文件或文件夹发生更改时收到通知](https://support.office.com/en-us/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918)。</span><span class="sxs-lookup"><span data-stu-id="8bf90-114">**Alert setup**: For more information about setting up alerts, see [Create an alert to get notified when a file or folder changes in SharePoint](https://support.office.com/en-us/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span></span>
- <span data-ttu-id="8bf90-115">**警报疑难解答**: 有关排除警报的详细信息, 请参阅[用户不接收 SharePoint Online 警报通知](https://docs.microsoft.com/en-us/sharepoint/support/sites/no-alert-notifications)。</span><span class="sxs-lookup"><span data-stu-id="8bf90-115">**Troubleshoot alerts**: For more information about troubleshooting alerts, see [Users don't receive SharePoint Online alert notifications](https://docs.microsoft.com/en-us/sharepoint/support/sites/no-alert-notifications).</span></span>
- <span data-ttu-id="8bf90-116">**高级 O365 合规性警报策略**: 有关设置这些警报的详细信息, 请参阅[合规性警报策略](https://docs.microsoft.com/en-us/office365/securitycompliance/alert-policies)。</span><span class="sxs-lookup"><span data-stu-id="8bf90-116">**Advanced O365 Compliance Alert Policies**: For more information about setting up these alerts, see [Compliance Alert Policies](https://docs.microsoft.com/en-us/office365/securitycompliance/alert-policies).</span></span>
- <span data-ttu-id="8bf90-117">**SharePoint 和 OneDrive 审核日志**: 有关如何检索这些事件的详细信息, 请参阅[Search the Audit log](https://docs.microsoft.com/en-us/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)。</span><span class="sxs-lookup"><span data-stu-id="8bf90-117">**SharePoint and OneDrive Audit Logs**: For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/en-us/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
- <span data-ttu-id="8bf90-118">**高级威胁防护发送的警报**: 请参阅[适用于 SharePoint 和 OneDrive 的 ATP](https://docs.microsoft.com/en-us/office365/securitycompliance/atp-for-spo-odb-and-teams)。</span><span class="sxs-lookup"><span data-stu-id="8bf90-118">**Alerts sent by Advanced Threat Protection**: See [ATP for SharePoint and OneDrive](https://docs.microsoft.com/en-us/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
- <span data-ttu-id="8bf90-119">**数据丢失防护策略发送的警报**: 请参阅[DLP 策略的电子邮件通知](https://docs.microsoft.com/en-us/office365/securitycompliance/use-notifications-and-policy-tips)。</span><span class="sxs-lookup"><span data-stu-id="8bf90-119">**Alerts sent by Data Loss Prevention polices**: See [Email notifications for DLP policies](https://docs.microsoft.com/en-us/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

## <a name="related-topics"></a><span data-ttu-id="8bf90-120">相关主题</span><span class="sxs-lookup"><span data-stu-id="8bf90-120">Related Topics</span></span>

<span data-ttu-id="8bf90-121">想要在 SharePoint Online 中试用 Microsoft 流吗？</span><span class="sxs-lookup"><span data-stu-id="8bf90-121">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="8bf90-122">创建流</span><span class="sxs-lookup"><span data-stu-id="8bf90-122">Create Flow</span></span>](https://support.office.com/en-us/article/create-a-flow-for-a-list-or-library-in-sharepoint-online-or-onedrive-for-business-a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="8bf90-123">SharePoint 和流</span><span class="sxs-lookup"><span data-stu-id="8bf90-123">SharePoint and Flow</span></span>](https://flow.microsoft.com/en-us/blog/sharepoint-and-flow/)
