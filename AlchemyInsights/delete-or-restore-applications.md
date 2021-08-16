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
ms.openlocfilehash: 0c7be98650ca87f36b66f0bb38fb665fc81525b7f3410da14b99fb67468c1e73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102561"
---
# <a name="delete-or-restore-applications"></a>删除或还原应用程序

**若要从 Azure AD 租户中删除应用程序**：

1. 在 **Azure AD 门户中，** 选择 **"Enterprise应用程序"。** 然后查找并选择要删除的应用程序。
2. 在左 **窗格的"** 管理"部分，选择"属性 **"。**
3. 选择 **"** 删除"，然后选择"是"以确认想要从 Azure AD 租户中删除应用。

若要详细了解如何删除应用，请参阅快速入门：从[Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)租户Azure Active Directory (应用程序) 应用程序。

在 PowerShell 中[，Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet 从 Azure Active Directory 中的特定应用程序中删除应用程序代理配置，并可以完全删除应用程序（如果已指定）。

可以使用 PowerShell **还原已删除** 的应用程序。 确定要还原的应用程序后，可以使用 [Restore-AzureADDeletedApplication 还原它](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)。
