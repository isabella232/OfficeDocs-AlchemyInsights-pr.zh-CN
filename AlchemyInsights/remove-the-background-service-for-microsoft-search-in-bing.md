---
title: 删除必应中的 Microsoft 搜索的背景服务
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50753384"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="b1efe-102">删除必应中的 Microsoft 搜索的背景服务</span><span class="sxs-lookup"><span data-stu-id="b1efe-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="b1efe-103">要删除必应中的 Microsoft 搜索的背景服务，可以尝试以下补救措施：</span><span class="sxs-lookup"><span data-stu-id="b1efe-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="b1efe-104">要还原到原始搜索引擎设置，请执行下列操作：</span><span class="sxs-lookup"><span data-stu-id="b1efe-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="b1efe-105">a.</span><span class="sxs-lookup"><span data-stu-id="b1efe-105">a.</span></span> <span data-ttu-id="b1efe-106">将 **使用必应作为默认搜索引擎[ 切换开关设为](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)关**。</span><span class="sxs-lookup"><span data-stu-id="b1efe-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="b1efe-107">b.</span><span class="sxs-lookup"><span data-stu-id="b1efe-107">b.</span></span> <span data-ttu-id="b1efe-108">[转到 Microsoft 365 管理中心](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) 并清除影响你组织中所有用户的设置。</span><span class="sxs-lookup"><span data-stu-id="b1efe-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="b1efe-109">要从单个设备中删除背景服务，请执行下列任务：</span><span class="sxs-lookup"><span data-stu-id="b1efe-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="b1efe-110">a.</span><span class="sxs-lookup"><span data-stu-id="b1efe-110">a.</span></span> <span data-ttu-id="b1efe-111">选择 **“控制面板”>“程序”>“程序和功能”**。</span><span class="sxs-lookup"><span data-stu-id="b1efe-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="b1efe-112">b.</span><span class="sxs-lookup"><span data-stu-id="b1efe-112">b.</span></span> <span data-ttu-id="b1efe-113">右键单击已安装程序列表下的“**必应中的 Microsoft 搜索**”，然后单击“**卸载**”。</span><span class="sxs-lookup"><span data-stu-id="b1efe-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="b1efe-114">要从组织中多个设备删除背景服务，请以管理员角色登录，然后在脚本中运行以下命令：</span><span class="sxs-lookup"><span data-stu-id="b1efe-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
