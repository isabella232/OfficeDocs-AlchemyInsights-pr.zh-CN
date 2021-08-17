---
title: DLP 策略使用技巧无法工作
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: f93b7efebd0a619acf300120cc6ece0adbedc39675f6e782fd982dc1f988edbd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079656"
---
# <a name="dlp-policy-tip-issues"></a>DLP 策略提示问题

**重要信息：** 在这段前所未有的时期，我们正在采取措施确保 SharePoint Online 和 OneDrive 服务高度可用，请访问 [SharePoint Online 临时功能调整](https://aka.ms/ODSPAdjustments)，获取详细信息。

若要在完全强制执行模式下在安全与合规&配置 DLP 策略的策略提示，请执行下列操作：

- 确保已在 DLP **规则** 上启用策略提示。 有关步骤，请参阅 [发送电子邮件通知和显示 DLP 策略的策略提示](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)。

- 确保内容与触发敏感信息类型实体定义中概述的规则 [所需的内容匹配](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)。

- 策略提示同时显示在 OWA 和 Outlook。 但是，在使用 Outlook 2013 或更高版本时，策略提示仅在特定条件下显示。 有关特定条件列表，请参阅 Supported [conditions for Outlook for Outlook later for displaying Policy 使用技巧](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)。

有关 DLP 策略提示的信息，请参阅[DLP Policy 使用技巧 Reference](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) and Support Matrix for DLP Policy [tips](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps)。