---
title: 如果 Azure 功能在 Microsoft Edge 中无法正常工作，该怎么办
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
ms.openlocfilehash: e188ecb375f3d84b45a1a7718b3c0b797c756f822ba64b3824976fe79c1e8298
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54117078"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>如果 Azure 功能在 Microsoft Edge 中无法正常工作，该怎么办

Microsoft Edge[与安全区域](https://go.microsoft.com/fwlink/?linkid=2140608)相关的已知问题，并且可能会影响 Azure 用户登录到管理中心Windows登录。 如果在将 Azure 功能与 Microsoft Edge时遇到问题，请尝试以下步骤：

1. 在" **开始"** 菜单中，搜索 **"Internet 选项** "并选择它。
2. 在 **"Internet 属性"** 对话框中，转到"安全 **"** 选项卡。
3. 选择" **受信任的站点"** 区域，然后选择"站点 **"** 按钮。
4. 在"**受信任的站点"** 对话框中，添加网关 URL 以及 [https://login.microsoftonline.com](https://login.microsoftonline.com) 和 [https://login.live.com](https://login.live.com) ，然后选择"关闭 **"。**
5. 在 **"Internet 属性** "对话框中，转到"隐私 **"** 选项卡。
6. 在"**弹出窗口阻止程序"** 部分，选择 **"设置"。** 在打开的对话框中，添加网关 URL 以及 和 [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) ，然后选择"关闭 **"。**
