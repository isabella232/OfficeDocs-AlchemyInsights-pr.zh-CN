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
# <a name="delete-or-restore-applications"></a>删除或还原应用程序

**若要从 Azure AD 租户中删除应用程序**，

1. 在 **Azure AD 门户中，** 选择 **企业应用程序**。 然后查找并选择要删除的应用程序。
2. 在左 **窗格中** 的"管理"部分，选择"**属性"。**
3. 选择 **"** 删除"，然后选择" **是** "以确认想要从 Azure AD 租户中删除应用。

若要详细了解如何删除应用，请参阅快速入门：从 [Azure AD 租户的 Azure Active Directory (中删除) 应用程序](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)。

在 PowerShell 中 [，Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet 从 Azure Active Directory 中的特定应用程序中删除应用程序代理配置，并可以完全删除应用程序（如果已指定）。

可以使用 **PowerShell 还原** 已删除的应用程序。 确定要还原的应用程序后，可以使用 [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)还原它。
