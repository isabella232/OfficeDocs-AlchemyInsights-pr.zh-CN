---
title: 修复 Microsoft 365 应用程序找不到 office 许可证关联的邮件
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747685"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="0ab7f-102">修复 Microsoft 365 应用程序 "找不到与 office 许可证关联的信息" 消息</span><span class="sxs-lookup"><span data-stu-id="0ab7f-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="0ab7f-103">如果您收到此消息，请尝试以下操作：</span><span class="sxs-lookup"><span data-stu-id="0ab7f-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="0ab7f-104">检查你的防火墙、防病毒软件和代理设置以确认他们没有阻止对 Microsoft 365 应用的 Internet 访问。</span><span class="sxs-lookup"><span data-stu-id="0ab7f-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="0ab7f-105">请参阅 [Microsoft 365 url 和 IP 地址范围](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)。</span><span class="sxs-lookup"><span data-stu-id="0ab7f-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="0ab7f-106">删除并重新分配受影响的用户 [的 Office 许可证](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) 。</span><span class="sxs-lookup"><span data-stu-id="0ab7f-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="0ab7f-107">打开 Office [应用并注销](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) 任何现有的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="0ab7f-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="0ab7f-108">转到 Windows 设置 >**帐户**  >  **电子邮件 & 帐户**，并删除除受影响帐户之外的所有工作帐户。</span><span class="sxs-lookup"><span data-stu-id="0ab7f-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="0ab7f-109">转到 Windows 设置 >**帐户**  >  **访问工作或学校**，并断开除受影响帐户之外的所有工作帐户。</span><span class="sxs-lookup"><span data-stu-id="0ab7f-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="0ab7f-110">重置 Office 激活状态。</span><span class="sxs-lookup"><span data-stu-id="0ab7f-110">Reset the Office activation state.</span></span> <span data-ttu-id="0ab7f-111">[了解如何](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)操作。</span><span class="sxs-lookup"><span data-stu-id="0ab7f-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="0ab7f-112">使用受影响的用户帐户[登录](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)。</span><span class="sxs-lookup"><span data-stu-id="0ab7f-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="0ab7f-113">有关其他故障排除解决方案，请参阅 [Office 中的无许可证产品和激活错误](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)。</span><span class="sxs-lookup"><span data-stu-id="0ab7f-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>