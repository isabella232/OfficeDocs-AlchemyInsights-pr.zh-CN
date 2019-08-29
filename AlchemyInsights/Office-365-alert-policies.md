---
title: 1385-Office-365-警报-策略
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: edff5a265cf31ce9a242f73ae7121ccb8b591d5f
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/29/2019
ms.locfileid: "36661286"
---
# <a name="office-365-alert-policies"></a><span data-ttu-id="82dce-102">Office 365 通知策略</span><span class="sxs-lookup"><span data-stu-id="82dce-102">Office 365 Alert policies</span></span>

<span data-ttu-id="82dce-103">Office 365 Security & 合规性中心提供了[默认通知策略](https://docs.microsoft.com/office365/securitycompliance/alert-policies#default-alert-policies), 这些策略将触发 Office 365 企业版或 OFFICE 365 美国政府 E1/G1、E3/G3 或 E5/G5 订阅的组织的警报。</span><span class="sxs-lookup"><span data-stu-id="82dce-103">The Office 365 Security & Compliance Center offers [default alert policies](https://docs.microsoft.com/office365/securitycompliance/alert-policies#default-alert-policies) that trigger alerts for organizations with an Office 365 Enterprise or Office 365 US Government E1/G1, E3/G3, or E5/G5 subscription.</span></span> <span data-ttu-id="82dce-104">因此, 管理员可能会收到由 Office365Alerts@microsoft.com 发送的通知电子邮件通知, 其中包含 "低严重性警报:*警报策略的名称*" 等主题行。</span><span class="sxs-lookup"><span data-stu-id="82dce-104">Therefore, admins may receive an alert email notification sent by Office365Alerts@microsoft.com with a subject line such as "A low-severity alert: *name of alert policy*".</span></span> <span data-ttu-id="82dce-105">当常见活动触发警报时, 将发送警报通知, 例如当用户执行以下操作时:</span><span class="sxs-lookup"><span data-stu-id="82dce-105">Alert notifications are sent when alerts are triggered for common activities, such as when users:</span></span>

- <span data-ttu-id="82dce-106">创建转发电子邮件的收件箱规则。</span><span class="sxs-lookup"><span data-stu-id="82dce-106">Create inbox rules that forward email.</span></span>
- <span data-ttu-id="82dce-107">为其邮箱分配权限。</span><span class="sxs-lookup"><span data-stu-id="82dce-107">Assign permissions their mailbox.</span></span>
- <span data-ttu-id="82dce-108">在 SharePoint 文件共享中共享或删除大量文件。</span><span class="sxs-lookup"><span data-stu-id="82dce-108">Share or delete a large number of files in SharePoint file sharing.</span></span>
- <span data-ttu-id="82dce-109">创建电子数据展示搜索和导出搜索结果。</span><span class="sxs-lookup"><span data-stu-id="82dce-109">Create eDiscovery searches and export search results.</span></span>

<span data-ttu-id="82dce-110">查看警报并对其执行操作:</span><span class="sxs-lookup"><span data-stu-id="82dce-110">To review and act on an alert:</span></span>

1. <span data-ttu-id="82dce-111">转到[安全 & 合规性中心](https://protection.office.com)并登录。</span><span class="sxs-lookup"><span data-stu-id="82dce-111">Go to the [Security & Compliance center](https://protection.office.com) and sign in.</span></span>
2. <span data-ttu-id="82dce-112">单击 "**警报** > **查看警报**"。</span><span class="sxs-lookup"><span data-stu-id="82dce-112">Click **Alerts** > **View alerts**.</span></span>
3. <span data-ttu-id="82dce-113">单击某个通知可显示包含有关该警报的信息的飞出页面。</span><span class="sxs-lookup"><span data-stu-id="82dce-113">Click an alert to display a flyout page with information about the alert.</span></span>

<span data-ttu-id="82dce-114">您可以对通知执行操作, 例如[删除可疑的收件箱规则](https://docs.microsoft.com/office365/securitycompliance/responding-to-a-compromised-email-account)。</span><span class="sxs-lookup"><span data-stu-id="82dce-114">You can take action on an alert, such as [removing a suspicious inbox rule](https://docs.microsoft.com/office365/securitycompliance/responding-to-a-compromised-email-account).</span></span> <span data-ttu-id="82dce-115">或者, 可以通过单击 "通知弹出窗口" 页上的 "**解决**" 直接关闭该警报。</span><span class="sxs-lookup"><span data-stu-id="82dce-115">Or you can simply close the alert by clicking **Resolve** on the alert flyout page.</span></span>

<span data-ttu-id="82dce-116">有关配置和管理通知策略的详细信息, 请参阅[本文](https://docs.microsoft.com/office365/securitycompliance/alert-policies)。</span><span class="sxs-lookup"><span data-stu-id="82dce-116">For more information about configuring and managing alert policies, see  [this article](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span></span>

<span data-ttu-id="82dce-117">**重要说明**: 通知来自 Microsoft 的电子邮件通知决不会要求您执行以下操作:</span><span class="sxs-lookup"><span data-stu-id="82dce-117">**Important**: Alert email notifications from Microsoft will never ask you to do the following:</span></span>

- <span data-ttu-id="82dce-118">提供密码</span><span class="sxs-lookup"><span data-stu-id="82dce-118">Provide a password</span></span>
- <span data-ttu-id="82dce-119">验证帐户的安全详细信息</span><span class="sxs-lookup"><span data-stu-id="82dce-119">Verify the security details of your account</span></span>
- <span data-ttu-id="82dce-120">重新对自己进行身份验证</span><span class="sxs-lookup"><span data-stu-id="82dce-120">Re-authenticate yourself</span></span>

<span data-ttu-id="82dce-121">如果您收到这样的电子邮件, 则它不是由 Microsoft 发送的, 应被视为仿冒欺诈。</span><span class="sxs-lookup"><span data-stu-id="82dce-121">If you receive an email message like this, it was not sent by Microsoft and should be considered a phishing scam.</span></span> <span data-ttu-id="82dce-122">如果发生这种情况, 请[将其报告给 Microsoft](https://docs.microsoft.com/office365/SecurityCompliance/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop)。</span><span class="sxs-lookup"><span data-stu-id="82dce-122">If that happens, please [report it to Microsoft](https://docs.microsoft.com/office365/SecurityCompliance/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).</span></span>