---
title: 部署加载项Microsoft 365 应用版
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233503"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="a63e9-102">部署加载项Microsoft 365 应用版</span><span class="sxs-lookup"><span data-stu-id="a63e9-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="a63e9-103">建议使用集中部署将外接程序Office组织内部的用户和组。</span><span class="sxs-lookup"><span data-stu-id="a63e9-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="a63e9-104">若要部署外接程序，请按照以下步骤操作：</span><span class="sxs-lookup"><span data-stu-id="a63e9-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="a63e9-105">**注意：** 若要以单个用户Office加载项，请参阅在加载项程序中查看、管理和Office [加载项](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)。</span><span class="sxs-lookup"><span data-stu-id="a63e9-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="a63e9-106">此外，请确保启用单独Office应用商店加载项的购置。</span><span class="sxs-lookup"><span data-stu-id="a63e9-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> <span data-ttu-id="a63e9-107">有关详细信息，请参阅通过在所有客户端上关闭 Office [Store 阻止](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)外接程序下载 (除Outlook) 。</span><span class="sxs-lookup"><span data-stu-id="a63e9-107">For details, see [Prevent add-in downloads by turning off the Office Store across all clients (Except Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).</span></span>

1. <span data-ttu-id="a63e9-108">确保您的环境满足使用集中部署部署外接程序的要求。</span><span class="sxs-lookup"><span data-stu-id="a63e9-108">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="a63e9-109">有关详细信息，请参阅 [要求](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)。</span><span class="sxs-lookup"><span data-stu-id="a63e9-109">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="a63e9-110">转到 **设置**  >  **集成应用** 在 Microsoft 365 管理中心获取  >  应用以部署外接程序。</span><span class="sxs-lookup"><span data-stu-id="a63e9-110">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="a63e9-111">注意：</span><span class="sxs-lookup"><span data-stu-id="a63e9-111">Notes:</span></span> 

- <span data-ttu-id="a63e9-112">集成应用要求管理员具有全局管理员或Exchange管理员权限。</span><span class="sxs-lookup"><span data-stu-id="a63e9-112">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="a63e9-113">将外接程序部署到多个用户时，我们建议使用组而不是单个用户进行分配。</span><span class="sxs-lookup"><span data-stu-id="a63e9-113">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="a63e9-114">有关详细信息，请参阅 [将加载项分配给用户和组的注意事项](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)。</span><span class="sxs-lookup"><span data-stu-id="a63e9-114">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="a63e9-115">集中部署不支持嵌套组或具有父组的组的用户。</span><span class="sxs-lookup"><span data-stu-id="a63e9-115">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="a63e9-116">有关详细信息，请参阅用户 [和组分配](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)。</span><span class="sxs-lookup"><span data-stu-id="a63e9-116">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="a63e9-117">确保为用户启用 Microsoft 365 App Management Service (GUID：'0517ffae-825d-4aff-999e-3f2336b8a20a') 。</span><span class="sxs-lookup"><span data-stu-id="a63e9-117">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="a63e9-118">有关详细信息，请参阅配置 [应用属性](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)。</span><span class="sxs-lookup"><span data-stu-id="a63e9-118">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="a63e9-119">如果使用集成应用部署加载项时遇到问题，请尝试使用加载项 [进行部署](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)。</span><span class="sxs-lookup"><span data-stu-id="a63e9-119">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="a63e9-120">有关详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="a63e9-120">For more information, see:</span></span>

<span data-ttu-id="a63e9-121">[在管理中心部署外接程序](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
[在管理中心管理外接程序](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
[使用集中部署 PowerShell cmdlet 管理外接程序](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
[通过Office中心集中部署发布Microsoft 365加载项](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
[疑难解答：用户看不到外接程序](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
[排查Office加载项中的用户错误](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="a63e9-121">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>