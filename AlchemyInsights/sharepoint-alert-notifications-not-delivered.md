---
title: 未传递 SharePoint 通知通知
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: f4002dc865fb7a03b07a9256709b947d6d774cb0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751233"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="eb095-102">未传递 SharePoint 通知通知</span><span class="sxs-lookup"><span data-stu-id="eb095-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="eb095-103">请检查电子邮件中的垃圾邮件文件夹，有时会出现通知。</span><span class="sxs-lookup"><span data-stu-id="eb095-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="eb095-104">确定是否 **未传递所有警报** ，或者是否未传递来自特定文件或库 **的单个警报** 。</span><span class="sxs-lookup"><span data-stu-id="eb095-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="eb095-105">**不传递单个警报**：如果未传递来自特定文件或库的单个通知，则可以尝试删除并重新创建它。</span><span class="sxs-lookup"><span data-stu-id="eb095-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="eb095-106">请参阅 [管理、查看或删除 SharePoint 警报](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) 以重新创建警报。</span><span class="sxs-lookup"><span data-stu-id="eb095-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>
- <span data-ttu-id="eb095-107">**未传递所有警报**：如果未传递来自多个文件或库的所有警报，请访问 [服务运行状况仪表板](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) ，以检查 SharePoint 或 Exchange 可能发生的任何咨询/事件。</span><span class="sxs-lookup"><span data-stu-id="eb095-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="eb095-108">问题可能与 SharePoint 通知功能或通过 Exchange 的电子邮件延迟有关。</span><span class="sxs-lookup"><span data-stu-id="eb095-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="eb095-109">此外，请务必注意是否正在传递其他电子邮件，如果没有，则可能是 Exchange 延迟问题。</span><span class="sxs-lookup"><span data-stu-id="eb095-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="eb095-110">有关警报的常见问题解答：</span><span class="sxs-lookup"><span data-stu-id="eb095-110">FAQ on alerts:</span></span>

- <span data-ttu-id="eb095-111">无法向通讯组发送通知，仅支持安全和 O365 组。</span><span class="sxs-lookup"><span data-stu-id="eb095-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="eb095-112">您不能自定义通知电子邮件模板;您需要使用 Microsoft FLOW 或 SharePoint Designer 工作流来实现这些。</span><span class="sxs-lookup"><span data-stu-id="eb095-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

## <a name="related-topics"></a><span data-ttu-id="eb095-113">相关主题</span><span class="sxs-lookup"><span data-stu-id="eb095-113">Related Topics</span></span>

<span data-ttu-id="eb095-114">想要在 SharePoint Online 中试用 Microsoft 流吗？</span><span class="sxs-lookup"><span data-stu-id="eb095-114">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="eb095-115">创建流</span><span class="sxs-lookup"><span data-stu-id="eb095-115">Create Flow</span></span>](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="eb095-116">SharePoint 和流</span><span class="sxs-lookup"><span data-stu-id="eb095-116">SharePoint and Flow</span></span>](https://flow.microsoft.com//blog/sharepoint-and-flow/)
