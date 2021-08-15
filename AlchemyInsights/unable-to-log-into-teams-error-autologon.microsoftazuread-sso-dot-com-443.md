---
title: 错误 autologon.microsoftazuread-sso.com:443 导致无法登录到 Teams
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 6671a63d97f24fadc9b34907d75600a3c0ad1c9990a4a8f8d32034c11e8a952e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038390"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>错误 autologon.microsoftazuread-sso.com:443 导致无法登录到 Teams

若启用无缝 SSO 作为 O365 身份验证方式，可能需要将 URL“autologon.microsoftazuread-sso.com”添加到“Intranet 站点”。  若过去曾将它添加到“受信任的站点”中，并且正在使用无缝 SSO，应将其从“受信任的站点”中删除。

请查看[无缝 SSO 故障排除清单](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist)。

请按照以下步骤将 URL 添加到“Intranet 站点”列表：

1. 单击“开始”按钮，以打开 Internet Explorer。 在搜索框中输入 Internet Explorer，然后从结果列表中单击“Internet Explorer”。
2. 单击“工具”，然后单击“Internet 选项”。
3. 单击“安全”选项卡。
4. 现在单击“本地 Intranet 站点”，然后依次单击“站点”按钮和“高级”按钮。
5. 输入网站 URL，然后单击“添加”。
6. 完成后，单击“关闭”。

有关详细信息，请参阅[关于为 O365 部署无缝 SSO 的文档](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start)（包括步骤 3 中用于将 URL 添加到“Intranet 站点”的基于策略的过程）。
