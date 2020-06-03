---
title: 修复 DKIM 安装问题
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506764"
---
# <a name="fix-dkim-setup-issues"></a>修复 DKIM 安装问题

如果您在为您的自定义域启用 DKIM 时遇到问题，请使用以下步骤：

- 大多数 DKIM 安装问题与不正确的 DNS 记录有关。 验证 DKIM CNAME 记录（**而不**是 TXT 记录）的格式是否正确。 有关详细信息，请参阅本[主题](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)。

- 在您的域的 DNS 托管服务（通常是您的域注册机构）中创建或更新 DKIM DNS 记录后，请等待 DNS 记录传播。

- 如果无法在管理中心创建 DKIM DNS 记录，则可以将 \<CustomDomain\> 其替换为自定义域（例如，contoso.com），并在[Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)中运行此命令： `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` 。
