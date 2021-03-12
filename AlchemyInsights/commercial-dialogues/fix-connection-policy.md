---
title: 修复连接策略
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736156"
---
# <a name="fix-connection-policy"></a>修复连接策略

电子邮件被标记为安全并传递到用户收件箱，因为发送 IP 地址在连接筛选器策略中标记为安全。 若要查看策略，请执行下列操作：

1. 转到 [Office 365 安全&合规](https://go.microsoft.com/fwlink/p/?linkid=2077143)中心，然后转到"**威胁** 管理策略  >    >  [""反垃圾邮件"。](https://go.microsoft.com/fwlink/?linkid=2101518)
2. 在"**自定义"** 选项卡上，选择 **"连接筛选器策略**"，然后选择"编辑 **策略"。**
3. 查看 **IP 允许** 列表。 查看安全 **列表** 是否已启用。

    > [!NOTE]
    > Microsoft 订阅到第三方受信任发件人来源。 如果 **启用** 安全列表，这些受信任的发件人不会错误地标记为垃圾邮件。 建议选择此选项，因为这样可以减少被归类为垃圾邮件 (垃圾邮件的误报) 数量。
