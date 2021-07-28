---
title: 如果 Azure 功能在 Microsoft Edge 中无法正常工作，该怎么办
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8315"
- "9004429"
ms.openlocfilehash: aa89cbd58875f418a0a7a9db4b5eb4f0e4c1223a
ms.sourcegitcommit: e9fcd72e64d35f5ba14dfa0fbde39eae20d86cfe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/27/2021
ms.locfileid: "53603238"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>如果 Azure 功能在 Microsoft Edge 中无法正常工作，该怎么办

Microsoft Edge 存在与安全区域相关的已知问题，这些问题可能会影响 Azure 用户登录 Windows 管理中心的方式。 有关详细信息，请参阅 [ Edge ](https://go.microsoft.com/fwlink/?linkid=2140608)上的已知问题。 如果在 Microsoft Edge 中使用 Azure 功能时遇到问题，请尝试以下操作：

1. 在“开始”菜单上，在 **搜索** 栏中，键入 **Internet 选项**，然后选择它。
1. 在 **Internet 属性** 中，选择"**安全**"选项卡。
1. 选择 **受信任的站点**，然后选择 **站点**。
1. 添加网关 URL，以及 <https://login.microsoftonline.com> 和 <https://login.live.com>，然后选择 **关闭**。
1. 在 **Internet 属性** 中，选择"**隐私**"选项卡。
1. 在弹出窗口阻止程序部分中，选择 **设置**。 添加网关 URL，以及 <https://login.microsoftonline.com> 和 <https://login.live.com>，然后选择 **关闭**。