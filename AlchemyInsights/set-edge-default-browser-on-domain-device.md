---
title: 将 Microsoft Edge 设置为加入域的设备上的默认浏览器
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426776"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="dc8d6-102">将 Microsoft Edge 设置为加入域的设备上的默认浏览器</span><span class="sxs-lookup"><span data-stu-id="dc8d6-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="dc8d6-103">将 Microsoft Edge 设置为默认浏览器：</span><span class="sxs-lookup"><span data-stu-id="dc8d6-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="dc8d6-104">[创建默认关联配置文件](https://go.microsoft.com/fwlink/?linkid=2132437)并将其存储在本地或网络共享上。</span><span class="sxs-lookup"><span data-stu-id="dc8d6-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="dc8d6-105">打开组策略编辑器，然后转到“**计算机配置**” > “**管理模板**” > “**Windows 组件**” > “**文件资源管理器**”。</span><span class="sxs-lookup"><span data-stu-id="dc8d6-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="dc8d6-106">选择“**设置默认关联配置文件**”。</span><span class="sxs-lookup"><span data-stu-id="dc8d6-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="dc8d6-107">选择“**策略设置**”，然后选择“**启用**”。</span><span class="sxs-lookup"><span data-stu-id="dc8d6-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="dc8d6-108">在“**选项**”下，输入默认关联配置文件的位置，然后选择“**确定**”。</span><span class="sxs-lookup"><span data-stu-id="dc8d6-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
