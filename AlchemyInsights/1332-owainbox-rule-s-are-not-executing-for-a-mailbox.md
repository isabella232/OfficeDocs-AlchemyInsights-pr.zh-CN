---
title: 1332 OWA-收件箱规则不执行的邮箱
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 0d3b7ce3d6b32d94a012eb3767c0747eed80f6e5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29915794"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>收件箱规则没有按预期工作

验证以下设置：
  
- 可以重定向一条消息，转发或答复以自动基于收件箱规则仅一次。（收件箱规则或邮件流规则，也称为传输规则） 的重定向规则可以将最多个十个转接收件人添加到一条消息。有关详细信息，请参阅[日记、 传输和收件箱规则限制](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)。
    
- 收件箱规则对备用日记邮箱不起作用。有关备用日记邮箱的详细信息，请参阅[备用日记邮箱](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)。
    
若要解决这些问题，请参阅[KB 2829319](https://support.microsoft.com/kb/2829319)。
  
如果没有应用上述问题，先升级到 Microsoft 支持问题运行的收件箱规则诊断报告：
  
1. 在 web 上的 Outlook 中打开邮箱并单击**设置** \> **选项** \> **组织电子邮件** \> **收件箱规则**。
    
2. 在页面的底部，单击**如果规则未正常运行单击此处以生成诊断报告**。
    

