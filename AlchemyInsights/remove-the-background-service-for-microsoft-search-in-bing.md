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
ms.openlocfilehash: 07d24290fc3b13cce7a931c4cff15176c080b4413489ba1935b6886939ea3874
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53982363"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>删除必应中的 Microsoft 搜索的背景服务

要删除必应中的 Microsoft 搜索的背景服务，可以尝试以下补救措施：

1. 要还原到原始搜索引擎设置，请执行下列操作：

    a. 将 **“使用必应作为默认搜索引擎”[切换开关](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)设为“关”**。

    b. [转到 Microsoft 365 管理中心](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed)并清除影响你组织中所有用户的设置。

2. 要从单个设备中删除背景服务，请执行下列任务：

    a. 选择 **“控制面板”>“程序”>“程序和功能”**。

    b. 右键单击已安装程序列表下的“**必应中的 Microsoft 搜索**”，然后单击“**卸载**”。

3. 要从组织中多个设备删除背景服务，请以管理员角色登录，然后在脚本中运行以下命令： 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
