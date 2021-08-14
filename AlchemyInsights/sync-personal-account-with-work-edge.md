---
title: 使用户能够将个人帐户与 Microsoft Edge 中的工作帐户同步
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: da435b37b689e97ca51ce5cf94eb7e7d71eb972060526989239310fac1460628
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54009046"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>使用户能够将个人帐户与 Microsoft Edge 中的工作帐户同步

确保满足以下条件：

- 在 Azure Active Directory 管理中心启用企业状态漫游，需要订阅 Azure Active Directory Premium 或企业移动性 + 安全性 （EMS）。有关详细信息，请参阅[在 Azure Active Directory 中启用企业状态漫游](/azure/active-directory/devices/enterprise-state-roaming-enable)。
- 满足以下一个或两个条件：
    - 已为租户启用 Azure 信息保护服务。 有关详细信息，请参阅 [ 从 Microsoft 365 管理中心激活 Azure Rights Management 保护](/azure/information-protection/activate-office365)。
    - 已为任何用户或租户启用 Azure Active Directory 企业状态漫游（ESR）功能。 有关详细信息，请参阅 [ 什么是企业状态漫游？](/azure/active-directory/devices/enterprise-state-roaming-overview)。

如果 AIP 和 ESR 均被禁用，则会出现一条错误消息，告知用户其帐户无法同步。
