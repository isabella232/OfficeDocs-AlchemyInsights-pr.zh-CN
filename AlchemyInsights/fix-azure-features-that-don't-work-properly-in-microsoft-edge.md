---
title: 如果 Azure 功能在 Microsoft Edge 中无法正常工作，应执行的操作
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
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576367"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="0ee6e-102">如果 Azure 功能在 Microsoft Edge 中无法正常工作，应执行的操作</span><span class="sxs-lookup"><span data-stu-id="0ee6e-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="0ee6e-103">Microsoft Edge 具有与安全区域相关的 [已知问题](https://go.microsoft.com/fwlink/?linkid=2140608) ，可能会影响 Azure 用户登录到 Windows 管理中心的方式。</span><span class="sxs-lookup"><span data-stu-id="0ee6e-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="0ee6e-104">如果在 Microsoft Edge 中使用 Azure 功能时遇到问题，请尝试以下步骤：</span><span class="sxs-lookup"><span data-stu-id="0ee6e-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="0ee6e-105">在 " **开始** " 菜单中，搜索 " **Internet 选项** " 并选择它。</span><span class="sxs-lookup"><span data-stu-id="0ee6e-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="0ee6e-106">在 " **Internet 属性** " 对话框中，转到 " **安全性** " 选项卡。</span><span class="sxs-lookup"><span data-stu-id="0ee6e-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="0ee6e-107">选择 " **受信任的站点** " 区域，然后选择 " **网站** " 按钮。</span><span class="sxs-lookup"><span data-stu-id="0ee6e-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="0ee6e-108">在 " **受信任的站点** " 对话框中，添加您的网关 URL 以及 [https://login.microsoftonline.com](https://login.microsoftonline.com) 和 [https://login.live.com](https://login.live.com) ，然后选择 " **关闭**"。</span><span class="sxs-lookup"><span data-stu-id="0ee6e-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="0ee6e-109">在 " **Internet 属性** " 对话框中，转到 " **隐私** " 选项卡。</span><span class="sxs-lookup"><span data-stu-id="0ee6e-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="0ee6e-110">在 " **弹出窗口阻止** " 部分中，选择 " **设置**"。</span><span class="sxs-lookup"><span data-stu-id="0ee6e-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="0ee6e-111">在打开的对话框中，添加您的网关 URL 以及 [https://login.microsoftonline.com](https://login.microsoftonline.com) 和 [https://login.live.com](https://login.live.com) ，然后选择 " **关闭**"。</span><span class="sxs-lookup"><span data-stu-id="0ee6e-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
