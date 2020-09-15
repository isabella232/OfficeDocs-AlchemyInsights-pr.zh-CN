---
title: 如何禁用外部组
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704118"
---
# <a name="how-to-disable-external-groups"></a>如何禁用外部组

Yammer external 消息类将 Exchange 传输规则应用 (Etr) ，这是一组用于防止公司信息被共享的主动控制。 为了限制用户创建外部组，您需要将 Exchange 传输规则配置 (ETR) ，然后将 Yammer 配置为使用 Exchange 传输规则来阻止外部邮件。
  
在 Exchange Online 管理中心中创建规则后，请按照以下步骤设置 ETR 以在 Yammer 中应用：
  
- 以经验证的管理员身份登录到 Yammer，并在 **Yammer 管理中心**中，转到 "C **Content And security \> security Settings"。**

- 在 " **外部邮件**" 下，选择 "在 **Yammer 中 (Etr) 强制实施 Exchange Online exchange 传输规则"。**

- 选择“**保存**”。

有关详细信息，请参阅在 [Yammer 网络中禁用外部消息](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)。
  