---
title: Azure AD 联接设备的单一登录疑难解答
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: 872333e13bb51b3a22431154627ad561f6db88c681c9eeee523fdd09e58c0371
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039236"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Azure AD 联接设备的单一登录疑难解答

如果你有本地 Active Directory (AD) 环境，并且你想要将加入 AD 域的计算机加入 Azure AD，则可以通过执行混合 Azure AD 加入来实现此目的。 [How To： Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.

有关详细信息，请参阅[Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business。](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)

**PRT (主要刷新) 问题**

PRT (主刷新令牌) 是 Windows 10、Windows Server 2016 和更高版本、iOS 和 Android 设备上 Azure AD 身份验证的关键项目。 它是一个 JSON Web 令牌 (JWT) ，专门颁发给 Microsoft 第一方令牌代理，以在这些设备上使用的应用程序之间启用单一登录 (SSO) 。 有关在设备上颁发、使用和保护 PRT Windows 10的详细信息，请参阅什么是主[刷新令牌？。](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)

**WamDefaultSet：YES 和 AzureADPrt：YES**

这些字段指示用户登录设备时是否已成功通过 Azure AD 身份验证。 如果值为 **NO，** 则可能是由于：

- 注册时与设备关联的 TPM 中的存储密钥 (在运行提升的设备时检查 KeySignTest) 
- 备用登录 ID
- 找不到 HTTP 代理

若要使用 dsregcmd 命令对设备进行故障排除，请参阅 [SSO 状态](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)。
