---
title: Single-Sign设备Azure Active Directory打开
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: 365225926296677feb7853481651a634792fd8bfa9abd9dc9359ffaae50b60eb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050000"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>已加入Azure Active Directory的单一登录

如果你有本地 Active Directory (AD) 环境，并且你想要将加入 AD 域的计算机加入 Azure AD，则可以通过执行混合 Azure AD 加入来实现此目的。 [How To： Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.

[为本地部署配置加入 Azure AD Single-Sign使用 Windows Hello for Business](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**PRT (主要刷新) 问题** PRT (主刷新令牌) 是 Windows 10、Windows Server 2016 和更高版本、iOS 和 Android 设备上 Azure AD 身份验证的关键项目。 它是一个 JSON Web 令牌 (JWT) ，专门颁发给 Microsoft 第一方令牌代理，以在这些设备上使用的应用程序之间启用单一登录 (SSO) 。 [在什么是主刷新令牌？](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)中，我们将详细介绍如何在设备上颁发、使用和保护 PRT Windows 10保护。

**WamDefaultSet：YES 和 AzureADPrt：YES** 这些字段指示用户登录设备时是否已成功通过 Azure AD 身份验证。 如果值为 **NO，** 则可能是由于：

- 注册时与设备关联的 TPM 中的存储密钥 (在运行提升的设备时检查 KeySignTest) 。
- 备用登录 ID
- 找不到 HTTP 代理

使用 dsregcmd 命令对设备进行故障排除 - [SSO 状态](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
