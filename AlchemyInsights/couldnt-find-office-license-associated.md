---
title: 修复 Microsoft 365 应用 找不到 Office 许可证关联消息
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816478"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="47e82-102">修复 Microsoft 365 应用"找不到关联的 Office 许可证"消息</span><span class="sxs-lookup"><span data-stu-id="47e82-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="47e82-103">如果收到此消息，请尝试执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="47e82-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="47e82-104">请检查防火墙、防病毒软件和代理设置，确认它们不会阻止 Internet 访问 Microsoft 365 应用。</span><span class="sxs-lookup"><span data-stu-id="47e82-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="47e82-105">请参阅 [Microsoft 365 URL 和 IP 地址范围](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)。</span><span class="sxs-lookup"><span data-stu-id="47e82-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="47e82-106">删除 [并重新分配受影响的用户的 Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) 许可证。</span><span class="sxs-lookup"><span data-stu-id="47e82-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="47e82-107">打开 Office 应用 [并注销](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) 任何现有用户帐户。</span><span class="sxs-lookup"><span data-stu-id="47e82-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="47e82-108">转到 Windows 设置>帐户  >  **电子邮件&帐户，** 并删除所有工作帐户（受影响帐户除外）。</span><span class="sxs-lookup"><span data-stu-id="47e82-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="47e82-109">转到 Windows 设置>**访问** 工作或学校帐户，并断开所有工作  >  帐户（受影响帐户除外）。</span><span class="sxs-lookup"><span data-stu-id="47e82-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="47e82-110">重置 Office 激活状态。</span><span class="sxs-lookup"><span data-stu-id="47e82-110">Reset the Office activation state.</span></span> <span data-ttu-id="47e82-111">[了解如何。](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)</span><span class="sxs-lookup"><span data-stu-id="47e82-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="47e82-112">[使用受影响的](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) 用户帐户登录。</span><span class="sxs-lookup"><span data-stu-id="47e82-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="47e82-113">有关其他疑难解答解决方案，请参阅 Office 中的未授权产品和 [激活错误](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)。</span><span class="sxs-lookup"><span data-stu-id="47e82-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>