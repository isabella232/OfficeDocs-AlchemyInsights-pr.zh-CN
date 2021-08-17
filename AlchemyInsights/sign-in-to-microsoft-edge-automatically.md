---
title: 自动登录Microsoft Edge登录
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 4e069a1c75caabf3bef7387140edd5650cf966856b888b5c6b5618a603986d6d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050684"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>自动登录Microsoft Edge登录

Microsoft Edge使用操作系统默认帐户根据用户设备的配置方式自动登录用户。 

下面介绍了每种类型的设备配置及其从属用户登录过程的方案：

- **设备为混合/AAD-J：** 此选项适用于Windows 10、低级别Windows和相应的服务器版本。 用户将自动使用其 AD Azure Active Directory (AD) 登录。
- **设备已加入域**：此选项适用于 Windows 10、低Windows版本和相应的服务器版本。 默认情况下，具有域帐户的用户不会自动登录;若要为用户启用自动登录，请使用 **ConfigureOnPremisesAccountAutoSignIn** 策略。 若要为拥有 Azure AD 帐户的用户启用自动登录，请考虑混合加入其设备。
- 操作系统的默认帐户是 **Microsoft** 帐户：此选项适用于 Windows 10 RS3 (版本 1709 内部版本 10.0.16299) 及更高版本。 方案不太可能在企业设备上发生。 但是，如果操作系统默认帐户是 Microsoft 帐户，Microsoft Edge将自动使用 Microsoft 帐户登录用户。
 
 
