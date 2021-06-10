---
title: 无法激活 Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798670"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="93fa4-102">无法激活 Office</span><span class="sxs-lookup"><span data-stu-id="93fa4-102">Unable to activate Office</span></span>

<span data-ttu-id="93fa4-103">**注意**：如果正在使用较早版本的 Windows（例如 Windows 7），请确保启用 TLS 1.2 为默认值。</span><span class="sxs-lookup"><span data-stu-id="93fa4-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="93fa4-104">有关详细信息，请参阅 [更新以在 Windows 的 WinHTTP 中启用 TLS 1.1 和 TLS 1.2 作为默认安全协议](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)。</span><span class="sxs-lookup"><span data-stu-id="93fa4-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="93fa4-105">检查你的订阅状态是否已过期。</span><span class="sxs-lookup"><span data-stu-id="93fa4-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="93fa4-106">请确保你拥有允许客户端许可证的订阅（如 Office 365 商业版或商业高级版），并[确保该用户分配有许可证](/microsoft-365/admin/manage/assign-licenses-to-users)。</span><span class="sxs-lookup"><span data-stu-id="93fa4-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="93fa4-107">确保用户使用分配有许可证的同一帐户登录到 Office。</span><span class="sxs-lookup"><span data-stu-id="93fa4-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="93fa4-108">查看 [Office 365 服务运行状况页面](/office365/enterprise/view-service-health)，检查是否存在任何已知的服务问题。</span><span class="sxs-lookup"><span data-stu-id="93fa4-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="93fa4-p102">检查防火墙、防病毒软件和代理设置，确认它们并未阻止 Microsoft 365 应用访问 Internet。请参阅 [Office 365 URL 和 IP 地址范围](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URL 和 IP 地址范围")。</span><span class="sxs-lookup"><span data-stu-id="93fa4-p102">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet. Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="93fa4-111">**提示** 在 Windows 计算机上，我们可以为你诊断并自动修复若干常见的 Office 登录问题。</span><span class="sxs-lookup"><span data-stu-id="93fa4-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="93fa4-112">下载并运行 **[Microsoft 支持和恢复助手](https://aka.ms/SaRA-OfficeSignInScenario)** 以使用我们的自动化工具。</span><span class="sxs-lookup"><span data-stu-id="93fa4-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="93fa4-113">采取下列故障排除操作：</span><span class="sxs-lookup"><span data-stu-id="93fa4-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="93fa4-114">打开 Office 应用，然后[注销](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)任何现有用户帐户。</span><span class="sxs-lookup"><span data-stu-id="93fa4-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="93fa4-115">[移除](/microsoft-365/admin/manage/remove-licenses-from-users)并[重新分配](/microsoft-365/admin/manage/assign-licenses-to-users) Office 许可证，然后使用受影响的用户帐户[登录 Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)。</span><span class="sxs-lookup"><span data-stu-id="93fa4-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="93fa4-116">运行[激活故障排除程序](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="93fa4-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="93fa4-117">重置 Office 激活状态</span><span class="sxs-lookup"><span data-stu-id="93fa4-117">Reset Office activation state</span></span>](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "重置 Office 激活状态")
- [<span data-ttu-id="93fa4-118">执行 Office 的联机修复</span><span class="sxs-lookup"><span data-stu-id="93fa4-118">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="93fa4-119">有关其他故障排除解决方案，请参阅：</span><span class="sxs-lookup"><span data-stu-id="93fa4-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="93fa4-120">Office 中未经授权产品和激活错误</span><span class="sxs-lookup"><span data-stu-id="93fa4-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="93fa4-121">激活 Office 时出现错误“很抱歉，无法连接到你的帐户。请稍后重试”</span><span class="sxs-lookup"><span data-stu-id="93fa4-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)