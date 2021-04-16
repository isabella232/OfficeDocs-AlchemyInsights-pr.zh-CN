---
title: 解决未授权的产品错误
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
- "3412"
- "9001428"
ms.openlocfilehash: eebfb7cea7ae97921bf3c3667818400a17b5e52e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786839"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a><span data-ttu-id="99733-102">解决"未授权产品"错误的建议</span><span class="sxs-lookup"><span data-stu-id="99733-102">Suggestions for solving "Unlicensed Product" errors</span></span>

<span data-ttu-id="99733-103">若要解决有关"未授权产品"的错误，请尝试以下操作：</span><span class="sxs-lookup"><span data-stu-id="99733-103">To solve errors about an "Unlicensed Product," try the following:</span></span>

- <span data-ttu-id="99733-104">检查订阅状态是否已过期。</span><span class="sxs-lookup"><span data-stu-id="99733-104">Check to see if your subscription status has expired.</span></span>
- <span data-ttu-id="99733-105">请确保你拥有允许客户端许可证的订阅，例如 Microsoft 365 商业应用版或商业高级版，并确保用户 [分配有许可证](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)。</span><span class="sxs-lookup"><span data-stu-id="99733-105">Make sure you have a subscription that allows client licenses, such as Microsoft 365 Apps for business or Business Premium, and [ensure that the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> 
- <span data-ttu-id="99733-106">确保用户使用分配有许可证的相同帐户登录 Office。</span><span class="sxs-lookup"><span data-stu-id="99733-106">Make sure the user is signing in to Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="99733-107">检查 ["服务运行状况"](https://docs.microsoft.com/office365/enterprise/view-service-health) 页以查看服务是否存在任何已知问题。</span><span class="sxs-lookup"><span data-stu-id="99733-107">Check the [Service health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="99733-108">检查防火墙、防病毒软件和代理设置，确认它们不会阻止 Microsoft 365 应用访问 Internet。</span><span class="sxs-lookup"><span data-stu-id="99733-108">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the Internet.</span></span> <span data-ttu-id="99733-109">请参阅 [URL 和 IP 地址范围](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)。</span><span class="sxs-lookup"><span data-stu-id="99733-109">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

<span data-ttu-id="99733-110">您还可以尝试以下疑难解答操作：</span><span class="sxs-lookup"><span data-stu-id="99733-110">You may also try the following troubleshooting actions:</span></span> 

- <span data-ttu-id="99733-111">打开 Office 应用 [并注销](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) 任何现有用户帐户。</span><span class="sxs-lookup"><span data-stu-id="99733-111">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="99733-112">[删除](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users)[并重新分配](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)Office 许可证，然后使用受影响的用户帐户登录[Office。](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)</span><span class="sxs-lookup"><span data-stu-id="99733-112">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) the Office license, and then [sign in to Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="99733-113">运行 [激活疑难解答程序](https://aka.ms/SARA-OfficeActivation-Alchemy)。</span><span class="sxs-lookup"><span data-stu-id="99733-113">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy).</span></span>
- <span data-ttu-id="99733-114">[重置 Office 激活状态](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)。</span><span class="sxs-lookup"><span data-stu-id="99733-114">[Reset the Office activation state](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span> 
- <span data-ttu-id="99733-115">[执行 Office 的联机修复](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b)。</span><span class="sxs-lookup"><span data-stu-id="99733-115">[Perform an Online Repair of Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span></span>

<span data-ttu-id="99733-116">有关其他故障排除解决方案，请参阅：</span><span class="sxs-lookup"><span data-stu-id="99733-116">For additional troubleshooting solutions, see:</span></span> 

- [<span data-ttu-id="99733-117">Office 中未经授权产品和激活错误</span><span class="sxs-lookup"><span data-stu-id="99733-117">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [<span data-ttu-id="99733-118">激活 Office 时出现错误“很抱歉，无法连接到你的帐户。请稍后重试”</span><span class="sxs-lookup"><span data-stu-id="99733-118">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)