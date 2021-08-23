---
title: 是否向 Microsoft 报告垃圾邮件误报？
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "975"
- "666"
- "3100019"
ms.openlocfilehash: d3897f24ce9a967b08a3fd15a2fdedbb3fe2a22d
ms.sourcegitcommit: f05d4caa0e657ee74d6b6e9abc88488f17d740fe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396605"
---
# <a name="do-you-have-legitimate-messages-being-marked-as-spam"></a>是否有正当邮件被标记为垃圾邮件？

当合法电子邮件最终在"垃圾邮件"文件夹或"隔离"中时，这很令人沮丧。 请考虑以下最常见的误报原因：

**租户替代 (最常见的)** 这完全在你的控制范围内进行修正。

将邮件提交到Microsoft 365 Defender策略和规则进行分析;在数分钟内即可获得重新扫描详细信息。
查看或修改策略或规则（如果适用）。 

**最终用户替代 (常见)** 这完全在你的控制范围内进行修正。 

将邮件提交到Microsoft 365 Defender策略和规则进行分析;在数分钟内即可获得重新扫描详细信息。 

如果邮件因从用户的阻止发件人列表中的地址发送而被阻止，则邮件头包括垃圾邮件筛选裁定"SFV：BLK"。

**发件人的电子邮件身份验证** 这部分位于要修正的控件内。

提交邮件以分析发件人在传递时的电子邮件身份验证失败情况;结果在一天内可用。 

如果你拥有发送基础结构，请查看如何将其与 SPF、DKIM 和 DMARC 保持一致，以确保目标电子邮件系统信任从你的域发送的邮件。 或者，与发件人联系以处理其 DNS 配置。

**Microsoft 筛选裁定** 这部分位于要修正的控件内。

提交邮件，将邮件报告为安全邮件;在一天内提供重新扫描结果。 如果你对特定情况下的筛选裁定有意见不一致，请使用租户允许/阻止列表。 但是，不应永久绕过 Microsoft 筛选裁定。 

有关详细信息，请参阅：

- 使最终用户能够向 Microsoft 提交邮件。 Microsoft 使用这些提交来提高电子邮件保护技术的有效性，它们会显示在提交报告中，供你用作更新策略的指示。 

- 若要观看有关提交邮件进行分析的简短视频，请参阅 [提交邮件进行分析](https://go.microsoft.com/fwlink/?linkid=2166435)。

- [使用“管理员提交”将可疑的垃圾邮件、网络钓鱼诈骗、URL和文件提交给 Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)

- [管理租户允许/阻止列表](https://docs.microsoft.com/microsoft-365/security/office-365-security/tenant-allow-block-list)

- [Microsoft 365 中的反垃圾邮件标题](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)

- [EOP 中的出站垃圾邮件保护](https://docs.microsoft.com/microsoft-365/security/office-365-security/outbound-spam-controls)