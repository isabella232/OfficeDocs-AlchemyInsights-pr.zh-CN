---
title: 在门户中复制设备记录
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2020
ms.locfileid: "43789587"
---
# <a name="duplicate-device-record-in-the-portal"></a>在门户中复制设备记录

如果设备未正确向 Configuration Manager 网站报告共同管理状态，则可能会在门户中看到一个设备的 2 个记录。 要检查设备的共同管理状态，请查看 Configuration Manager 控制台中设备的“**共同托管**”列。 如果看不到该列，可通过右键单击任一列标题，然后从列表中选择来进行添加。

“共同托管”值必须为“**是**”。 如果该值为“**否**”，请在客户端设备上打开 Configuration Manager 客户端小程序，然后勾选“常规”选项卡中的“**共同管理**”属性。

- 如果该值为“**已启用**”，则表示与管理点的客户端通信存在问题。 请查看设备上的 **CcmMessaging.log**，调查可能存在的连接性问题。

- 如果该值为“**已禁用**”且设备已在 Intune 中注册，请查看设备上的 **CoManagementHandler.log**，确保设备已收到共同管理策略。