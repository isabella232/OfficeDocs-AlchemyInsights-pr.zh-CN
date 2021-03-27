---
title: 获取企业应用程序列表
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
- "9004342"
- "9837"
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/26/2021
ms.locfileid: "51379801"
---
# <a name="get-a-list-of-enterprise-applications"></a>获取企业应用程序列表

1. 若要获取企业应用程序 **列表 (所有** 应用程序，或者通过 Powershell 命令按显示名称、ID、标识符 URI 等 ) 进行筛选，请参阅 [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)。
2. 若要从所有对象 (或按 ID) Powershell 命令筛选的服务主体对象列表，请参阅 [Get-AzureADServicePrincipal (AzureAD) ](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)。
3. 如果你想要获取 SAML 配置的应用列表，以下 **PowerShell 脚本** 可以帮助你：

    每个应用程序（无论是 OAuth 应用还是 SAML 应用 (库应用和非库应用) 注册时，它们都会在 AAD 中创建两个对象。 一个称为 Application 对象，另一个称为服务主体对象。 使用 PowerShell 转储服务主体对象的属性时，会发现每个应用程序都有一定数量的与其关联的标记，如下所示：

    - OAuth 应用将具有名为"**WindowsAzureActiveDirectoryIntegratedApp**" 的标记
    - Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"
    - 非库 SAML 应用将具有名为"**WindowsAzureActiveDirectoryCustomSingleSignOnApplication "** 的标记

    因此，可以使用这些标记并找出它是什么类型的应用。 标记 **"WindowsAzureActiveDirectoryIntegratedApp"** 通用于所有类型的应用。 可以使用以下代码段列出库和非库 (的所有 SAML) ：

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    有关详细信息，请参阅在 [Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)中标识支持 SAML 的应用。

4. **仅查找和列出 Web 应用程序**：使用以下命令获取应用程序类型为"Web app/API"的所有 Azure AD 应用程序

    Get-AzureADApplication -All：$true |Where-Object { $_.PublicClient -ne $true } |FT
5. **单独查找和列出本机应用程序**：运行以下命令，获取桌面/移动设备 (应用程序的所有) 客户端。

    Get-AzureADApplication -All：$true |Where-Object { $_.PublicClient -eq $true } |FT
6. **将所有注册的 Azure AD 应用程序详细信息导出到 CSV：** 以下命令将包含所需详细信息的所有 Azure AD 应用导出到 csv 文件：

    - Get-AzureADApplication -All：$true |Select-Object DisplayName、AppID、PublicClient、AvailableToOtherTenants、HomePage、LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8

7. **需要导出未使用的 Azure 应用列表** – 审核报告

    如果你拥有 Azure AD Premium 许可证，Azure AD 最多只能显示 30 天的应用程序日志。
    有两个选项可以保留数据超过 30 天。 可以使用 Azure [AD 报告 API](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) 以编程方式检索数据，并存储到数据库中。 或者，你可以将审核日志集成到第三方 SIEM 系统中。

    还可以下载 Azure Active directory 下的所有应用程序和拥有的应用程序的应用列表>应用注册>下载>所有应用程序/拥有的应用程序。

    若要通过 MS Graph 获取应用程序列表，请参阅[列出应用程序 - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list)和应用程序资源类型[- Microsoft Graph v1.0。](https://docs.microsoft.com/graph/api/resources/application)
