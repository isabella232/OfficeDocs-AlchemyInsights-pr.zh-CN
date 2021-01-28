---
title: 删除或还原应用程序
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
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013931"
---
# <a name="delete-or-restore-applications"></a><span data-ttu-id="035cd-102">删除或还原应用程序</span><span class="sxs-lookup"><span data-stu-id="035cd-102">Delete or restore applications</span></span>

<span data-ttu-id="035cd-103">**若要从 Azure AD 租户中删除应用程序**，</span><span class="sxs-lookup"><span data-stu-id="035cd-103">**To delete an application from your Azure AD tenant**:</span></span>

1. <span data-ttu-id="035cd-104">在 **Azure AD 门户中，** 选择 **企业应用程序**。</span><span class="sxs-lookup"><span data-stu-id="035cd-104">In the **Azure AD portal**, select **Enterprise applications**.</span></span> <span data-ttu-id="035cd-105">然后查找并选择要删除的应用程序。</span><span class="sxs-lookup"><span data-stu-id="035cd-105">Then find and select the application you want to delete.</span></span>
2. <span data-ttu-id="035cd-106">在左 **窗格中** 的"管理"部分，选择"**属性"。**</span><span class="sxs-lookup"><span data-stu-id="035cd-106">In the **Manage** section in the left pane, select **Properties**.</span></span>
3. <span data-ttu-id="035cd-107">选择 **"** 删除"，然后选择" **是** "以确认想要从 Azure AD 租户中删除应用。</span><span class="sxs-lookup"><span data-stu-id="035cd-107">Select **Delete**, and then select **Yes** to confirm you want to delete the app from your Azure AD tenant.</span></span>

<span data-ttu-id="035cd-108">若要详细了解如何删除应用，请参阅快速入门：从 [Azure AD 租户的 Azure Active Directory (中删除) 应用程序](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)。</span><span class="sxs-lookup"><span data-stu-id="035cd-108">For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span></span>

<span data-ttu-id="035cd-109">在 PowerShell 中 [，Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet 从 Azure Active Directory 中的特定应用程序中删除应用程序代理配置，并可以完全删除应用程序（如果已指定）。</span><span class="sxs-lookup"><span data-stu-id="035cd-109">In PowerShell, the [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet removes Application Proxy configurations from a specific application in Azure Active Directory, and can delete the application completely if specified.</span></span>

<span data-ttu-id="035cd-110">可以使用 **PowerShell 还原** 已删除的应用程序。</span><span class="sxs-lookup"><span data-stu-id="035cd-110">You can **restore a deleted application** using PowerShell.</span></span> <span data-ttu-id="035cd-111">确定要还原的应用程序后，可以使用 [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)还原它。</span><span class="sxs-lookup"><span data-stu-id="035cd-111">Once the application you want to restore has been identified, you can restore it using [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>
