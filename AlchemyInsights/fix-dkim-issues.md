---
title: 修复 DKIM 设置问题
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
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945921"
---
# <a name="fix-dkim-setup-issues"></a>修复 DKIM 设置问题

如果你在为自定义域启用 DKIM 时遇到问题，请使用以下步骤：

- 大多数 DKIM 设置问题与错误的 DNS 记录有关。 验证 DKIM CNAME 记录 (不是TXT 记录) 格式是否正确。 有关详细信息，[请参阅本主题。](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

- 在 DNS 托管服务处为域创建或更新 DKIM DNS 记录 (，域注册机构) ，等待 DNS 记录传播。

- 如果无法通过管理中心创建 DKIM DNS 记录，可以将 替换为自定义域 (例如，contoso.com) 在 \<CustomDomain\> [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)中运行此命令： `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` 。
