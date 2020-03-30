---
title: 错误 autologon.microsoftazuread-sso.com:443 导致无法登录到 Teams
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931797"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="a838b-102">错误 autologon.microsoftazuread-sso.com:443 导致无法登录到 Teams</span><span class="sxs-lookup"><span data-stu-id="a838b-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="a838b-103">若启用无缝 SSO 作为 O365 身份验证方式，可能需要将 URL“autologon.microsoftazuread-sso.com”添加到“Intranet 站点”。</span><span class="sxs-lookup"><span data-stu-id="a838b-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="a838b-104">若过去曾将它添加到“受信任的站点”中，并且正在使用无缝 SSO，应将其从“受信任的站点”中删除。</span><span class="sxs-lookup"><span data-stu-id="a838b-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="a838b-105">请查看[无缝 SSO 故障排除清单](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist)。</span><span class="sxs-lookup"><span data-stu-id="a838b-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="a838b-106">请按照以下步骤将 URL 添加到“Intranet 站点”列表：</span><span class="sxs-lookup"><span data-stu-id="a838b-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="a838b-107">单击“开始”按钮，以打开 Internet Explorer。\*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="a838b-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="a838b-108">在搜索框中输入 Internet Explorer，然后从结果列表中单击“Internet Explorer”。\*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="a838b-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="a838b-109">单击“工具”，然后单击“Internet 选项”。\*\*\*\*\*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="a838b-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="a838b-110">单击“安全”选项卡。\*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="a838b-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="a838b-111">现在单击“本地 Intranet 站点”，然后依次单击“站点”按钮和“高级”按钮。\*\*\*\*\*\*\*\*\*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="a838b-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="a838b-112">输入网站 URL，然后单击“添加”。\*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="a838b-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="a838b-113">完成后，单击“关闭”。\*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="a838b-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="a838b-114">有关详细信息，请参阅[关于为 O365 部署无缝 SSO 的文档](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start)（包括步骤 3 中用于将 URL 添加到“Intranet 站点”的基于策略的过程）。</span><span class="sxs-lookup"><span data-stu-id="a838b-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
