---
title: 如何禁用外部组
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 95e60599b5298090db23bf887cb860350280964f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35384815"
---
# <a name="how-to-disable-external-groups"></a>如何禁用外部组

Yammer 外部邮件应用 Exchange 传输规则 (Etr), 这是一组用于防止公司信息被共享的主动控制。 为了限制用户创建外部组, 您需要配置 Exchange 传输规则 (ETR), 然后将 Yammer 配置为使用 Exchange 传输规则来阻止外部邮件。
  
在 Exchange Online 管理中心中创建规则后, 请按照以下步骤设置 ETR 以在 Yammer 中应用:
  
- 以经验证的管理员身份登录到 Yammer, 并在**Yammer 管理中心**中, 转到 "C **Content And \> security security Settings"。**

- 在 "**外部邮件**" 下, 选择 "在**Yammer 中强制实施 Exchange Online exchange 传输规则 (etr)"。**

- 选择“保存”****。

有关详细信息, 请参阅在[具有 Exchange 传输规则的 Yammer 网络中控制外部消息](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)
  