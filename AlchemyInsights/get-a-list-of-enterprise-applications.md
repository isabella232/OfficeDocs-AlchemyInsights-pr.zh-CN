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
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="74cf0-102">获取企业应用程序列表</span><span class="sxs-lookup"><span data-stu-id="74cf0-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="74cf0-103">若要获取企业应用程序 **列表 (所有** 应用程序，或者通过 Powershell 命令按显示名称、ID、标识符 URI 等 ) 进行筛选，请参阅 [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)。</span><span class="sxs-lookup"><span data-stu-id="74cf0-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="74cf0-104">若要从所有对象 (或按 ID) Powershell 命令筛选的服务主体对象列表，请参阅 [Get-AzureADServicePrincipal (AzureAD) ](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)。</span><span class="sxs-lookup"><span data-stu-id="74cf0-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="74cf0-105">如果你想要获取 SAML 配置的应用列表，以下 **PowerShell 脚本** 可以帮助你：</span><span class="sxs-lookup"><span data-stu-id="74cf0-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="74cf0-106">每个应用程序（无论是 OAuth 应用还是 SAML 应用 (库应用和非库应用) 注册时，它们都会在 AAD 中创建两个对象。</span><span class="sxs-lookup"><span data-stu-id="74cf0-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="74cf0-107">一个称为 Application 对象，另一个称为服务主体对象。</span><span class="sxs-lookup"><span data-stu-id="74cf0-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="74cf0-108">使用 PowerShell 转储服务主体对象的属性时，会发现每个应用程序都有一定数量的与其关联的标记，如下所示：</span><span class="sxs-lookup"><span data-stu-id="74cf0-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="74cf0-109">OAuth 应用将具有名为"**WindowsAzureActiveDirectoryIntegratedApp**" 的标记</span><span class="sxs-lookup"><span data-stu-id="74cf0-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="74cf0-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span><span class="sxs-lookup"><span data-stu-id="74cf0-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="74cf0-111">非库 SAML 应用将具有名为"**WindowsAzureActiveDirectoryCustomSingleSignOnApplication "** 的标记</span><span class="sxs-lookup"><span data-stu-id="74cf0-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="74cf0-112">因此，可以使用这些标记并找出它是什么类型的应用。</span><span class="sxs-lookup"><span data-stu-id="74cf0-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="74cf0-113">标记 **"WindowsAzureActiveDirectoryIntegratedApp"** 通用于所有类型的应用。</span><span class="sxs-lookup"><span data-stu-id="74cf0-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="74cf0-114">可以使用以下代码段列出库和非库 (的所有 SAML) ：</span><span class="sxs-lookup"><span data-stu-id="74cf0-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="74cf0-115">有关详细信息，请参阅在 [Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)中标识支持 SAML 的应用。</span><span class="sxs-lookup"><span data-stu-id="74cf0-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="74cf0-116">**仅查找和列出 Web 应用程序**：使用以下命令获取应用程序类型为"Web app/API"的所有 Azure AD 应用程序</span><span class="sxs-lookup"><span data-stu-id="74cf0-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="74cf0-117">Get-AzureADApplication -All：$true |Where-Object { $_.PublicClient -ne $true } |FT</span><span class="sxs-lookup"><span data-stu-id="74cf0-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="74cf0-118">**单独查找和列出本机应用程序**：运行以下命令，获取桌面/移动设备 (应用程序的所有) 客户端。</span><span class="sxs-lookup"><span data-stu-id="74cf0-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="74cf0-119">Get-AzureADApplication -All：$true |Where-Object { $_.PublicClient -eq $true } |FT</span><span class="sxs-lookup"><span data-stu-id="74cf0-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="74cf0-120">**将所有注册的 Azure AD 应用程序详细信息导出到 CSV：** 以下命令将包含所需详细信息的所有 Azure AD 应用导出到 csv 文件：</span><span class="sxs-lookup"><span data-stu-id="74cf0-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="74cf0-121">Get-AzureADApplication -All：$true |Select-Object DisplayName、AppID、PublicClient、AvailableToOtherTenants、HomePage、LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="74cf0-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="74cf0-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span><span class="sxs-lookup"><span data-stu-id="74cf0-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="74cf0-123">**需要导出未使用的 Azure 应用列表** – 审核报告</span><span class="sxs-lookup"><span data-stu-id="74cf0-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="74cf0-124">如果你拥有 Azure AD Premium 许可证，Azure AD 最多只能显示 30 天的应用程序日志。</span><span class="sxs-lookup"><span data-stu-id="74cf0-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="74cf0-125">有两个选项可以保留数据超过 30 天。</span><span class="sxs-lookup"><span data-stu-id="74cf0-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="74cf0-126">可以使用 Azure [AD 报告 API](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) 以编程方式检索数据，并存储到数据库中。</span><span class="sxs-lookup"><span data-stu-id="74cf0-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="74cf0-127">或者，你可以将审核日志集成到第三方 SIEM 系统中。</span><span class="sxs-lookup"><span data-stu-id="74cf0-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="74cf0-128">还可以下载 Azure Active directory 下的所有应用程序和拥有的应用程序的应用列表>应用注册>下载>所有应用程序/拥有的应用程序。</span><span class="sxs-lookup"><span data-stu-id="74cf0-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="74cf0-129">若要通过 MS Graph 获取应用程序列表，请参阅[列出应用程序 - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list)和应用程序资源类型[- Microsoft Graph v1.0。](https://docs.microsoft.com/graph/api/resources/application)</span><span class="sxs-lookup"><span data-stu-id="74cf0-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>
