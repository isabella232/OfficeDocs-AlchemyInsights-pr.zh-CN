---
title: Sharepoint Online PowerShell
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 8c270748fc75f929371fbb2856daad3ae61a1540
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764251"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="4334b-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="4334b-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="4334b-103">在 Sharepoint Online 中使用 PowerShell 或脚本？</span><span class="sxs-lookup"><span data-stu-id="4334b-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="4334b-104">有关详细信息，请访问下面的链接。</span><span class="sxs-lookup"><span data-stu-id="4334b-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="4334b-105">SharePoint Online 命令行管理程序入门</span><span class="sxs-lookup"><span data-stu-id="4334b-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="4334b-106">使用多重身份验证（MFA）连接到 SPO PowerShell</span><span class="sxs-lookup"><span data-stu-id="4334b-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="4334b-107">[SharePoint 模式和做法（PnP）](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps)包含一个 PowerShell 命令库，使您可以对 SPO 执行复杂的管理操作。</span><span class="sxs-lookup"><span data-stu-id="4334b-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="4334b-108">如果您在使用 SPO 命令行管理程序进行连接时遇到问题，请确保已更新到最新版本，并尝试使用 *"import-Module Microsoft. PowerShell"* [重新导入该模块](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module)。</span><span class="sxs-lookup"><span data-stu-id="4334b-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="4334b-109">如果您尝试运行客户端对象模型脚本，则需要将[Sharepoint Online 客户端组件 SDK](https://www.microsoft.com/download/details.aspx?id=42038)安装在本地计算机上。</span><span class="sxs-lookup"><span data-stu-id="4334b-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="4334b-110">如果您在从 PowerShell 运行脚本时遇到问题，您可能需要考虑以管理员身份运行 PowerShell，并更改[执行策略](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)。</span><span class="sxs-lookup"><span data-stu-id="4334b-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>