---
title: 应用注册所有者问题
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: cd7533f09ed8361e134b81979532cdebbf49971c54553a0172c7527f30e319bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951123"
---
# <a name="app-registration-owner-issues"></a>应用注册所有者问题

以下是将主体添加为应用注册所有者的可用方法：

- 使用 Azure AD PowerShell 模块 -

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    参考 [：Add-AzureADApplicationOwner (AzureAD) ](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- 使用 Azure CLI - `az ad app owner add`

    参考 [：az 广告应用所有者](https://docs.microsoft.com/cli/azure/ad/app/owner)
- 使用 MS Graph -

    参考：[添加所有者 - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- 使用 Azure AD 门户 - 导航 [到](https://portal.azure.com/) portal.azure.com> Azure Active directory >应用注册>选择应用程序>所有者>添加所有者"

**即使你是该应用程序的所有者，也无法在"应用注册"边栏选项卡上查看应用程序？**

应用的所有者不是管理角色。 如果启用 ["限制对 Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) 管理门户的访问"设置，则只有管理员才能在应用注册门户上查看应用程序。 若要使所有者能够查看应用程序，请禁用此设置 (将其设置为 NO) 或仅为特定应用程序向所有者分配管理员角色。 但是，为此，你需要一个Azure AD Premium P2[许可证，并](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)启用Privileged Identity Management。
