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
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>如果 Azure 功能在 Microsoft Edge 中无法正常工作，应执行的操作

Microsoft Edge 具有与安全区域相关的 [已知问题](https://go.microsoft.com/fwlink/?linkid=2140608) ，可能会影响 Azure 用户登录到 Windows 管理中心的方式。 如果在 Microsoft Edge 中使用 Azure 功能时遇到问题，请尝试以下步骤：

1. 在 " **开始** " 菜单中，搜索 " **Internet 选项** " 并选择它。
2. 在 " **Internet 属性** " 对话框中，转到 " **安全性** " 选项卡。
3. 选择 " **受信任的站点** " 区域，然后选择 " **网站** " 按钮。
4. 在 " **受信任的站点** " 对话框中，添加您的网关 URL 以及 [https://login.microsoftonline.com](https://login.microsoftonline.com) 和 [https://login.live.com](https://login.live.com) ，然后选择 " **关闭**"。
5. 在 " **Internet 属性** " 对话框中，转到 " **隐私** " 选项卡。
6. 在 " **弹出窗口阻止** " 部分中，选择 " **设置**"。 在打开的对话框中，添加您的网关 URL 以及 [https://login.microsoftonline.com](https://login.microsoftonline.com) 和 [https://login.live.com](https://login.live.com) ，然后选择 " **关闭**"。
