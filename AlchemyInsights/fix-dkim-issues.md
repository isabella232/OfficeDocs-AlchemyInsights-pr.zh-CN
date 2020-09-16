---
title: 修复 DKIM 安装问题
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744940"
---
# <a name="fix-dkim-setup-issues"></a>修复 DKIM 安装问题

如果您在为您的自定义域启用 DKIM 时遇到问题，请使用以下步骤：

- 大多数 DKIM 安装问题与不正确的 DNS 记录有关。 验证 DKIM CNAME 记录 (**不** 是 TXT 记录，) 格式是否正确。 有关详细信息，请参阅本 [主题](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)。

- 在您的域的 DNS 托管服务上创建或更新 DKIM DNS 记录之后 (通常情况下，您的域注册机构) ，等待 DNS 记录传播。

- 如果无法在管理中心创建 DKIM DNS 记录，则可以 \<CustomDomain\> 将其替换为自定义域 (例如，contoso.com) 并在 [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)中运行此命令： `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` 。
