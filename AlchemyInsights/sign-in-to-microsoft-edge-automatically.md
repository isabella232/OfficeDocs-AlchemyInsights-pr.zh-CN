---
title: 自动登录到 Microsoft Edge
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
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599443"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>自动登录到 Microsoft Edge

Microsoft Edge 根据用户设备的配置方式，使用 OS 的默认帐户自动登录用户。 

以下介绍每种类型的设备配置及其相关用户登录进程的方案：

1. **设备是混合型/AAD-J**：此选项在 windows 10、下层 windows 和相应的服务器版本上可用。 将使用 Azure Active Directory (AD) 帐户自动登录用户。
2. **设备已加入域**：此选项在 windows 10、下层 windows 和相应的服务器版本上可用。 默认情况下，不会自动登录具有域帐户的用户;若要为其启用自动登录，请使用 **ConfigureOnPremisesAccountAutoSignIn** 策略。 若要为使用 Azure AD 帐户的用户启用自动登录，请考虑混合加入其设备。
3. **OS 的默认帐户是 Microsoft 帐户**：在 WINDOWS 10 RS3 上提供此选项。 (版本1709，构建 10.0.16299) 及更高版本。 企业设备上可能不会发生这种情况。 但是，如果 OS 的默认帐户是 Microsoft 帐户，则 Microsoft Edge 将使用 Microsoft 帐户自动登录用户。
 
 
