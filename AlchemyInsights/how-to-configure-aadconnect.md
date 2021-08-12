---
title: 646 如何配置 AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963633"
---
# <a name="configure-sync-features"></a>配置同步功能

Azure AD 连接包括默认启用或可在以后启用的几个功能。 某些功能需要特定环境中的其他配置。

- [对象](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) 同步到 Azure AD 的筛选限制。 默认情况下，将同步所有用户、联系人、组Windows 10计算机帐户。 可以基于域、OUS 或其他属性包含或排除对象。

- [密码哈希同步](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) 将密码哈希从本地 Active Directory 同步到 Azure AD。 这允许在一个位置管理密码，但在内部部署和云环境中使用相同的密码。 由于 Active Directory 是权威来源，因此您可以使用自己的密码策略。

- [SSPR (](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) 自助服务密码重置) 允许用户在云中重置自己的密码，同时仍应用本地密码策略。

- [设备写回](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) 允许 Azure AD 中注册的设备写回本地 Active Directory，以便它们可用于条件访问。

- [默认情况下会启用"](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) 防止意外删除"功能，以帮助防止每个同步 (对象数超过 500 个) 。 您可以更改此设置以满足组织的需要。

- [默认情况下，](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)为快速安装启用自动升级，并有助于确保 Azure AD 连接始终为当前版本。
