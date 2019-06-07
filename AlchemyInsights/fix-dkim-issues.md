---
title: 修复 DKIM 安装问题
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764867"
---
# <a name="fix-dkim-setup-issues"></a>修复 DKIM 安装问题

如果您在为您的自定义域启用 DKIM 时遇到问题, 请使用以下步骤:

- 大多数 DKIM 安装问题与不正确的 DNS 记录有关。 验证 DKIM CNAME 记录 (**而不**是 TXT 记录) 的格式是否正确。 有关详细信息, 请参阅本[主题](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)。

- 在您的域的 DNS 托管服务 (通常是您的域注册机构) 中创建或更新 DKIM DNS 记录后, 请等待 DNS 记录传播。

- 如果无法在管理中心创建 DKIM DNS 记录, 则可以\<将 CustomDomain\>替换为自定义域 (例如, contoso.com), 并在[Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)中运行此命令:。 `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`
