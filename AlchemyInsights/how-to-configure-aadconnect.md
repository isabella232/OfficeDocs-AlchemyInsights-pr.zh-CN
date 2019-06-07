---
title: 646如何配置 AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 2dc4ae7d6809c24ce599ac128570e9354c9f2b30
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752551"
---
# <a name="configure-sync-features"></a>配置同步功能

Azure AD Connect 包括在默认情况下启用的几项功能, 或者您可以稍后启用的功能。 某些功能需要在特定环境中进行额外配置。

- [筛选](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering)限制将对象同步到 Azure AD。 默认情况下, 将同步所有用户、联系人、组和 Windows 10 计算机帐户。 您可以基于域、Ou 或其他属性包含或排除对象。

- [密码哈希同步](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization)将密码哈希从本地 Active Directory 同步到 Azure AD。 这将允许在一个位置进行密码管理, 但在本地和云环境中使用相同的密码。 由于 Active Directory 是权威源, 因此您可以使用自己的密码策略。

- [自助密码重置 (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr)允许用户在应用本地密码策略的同时在云中重置自己的密码。

- [设备写回](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback)允许 Azure AD 中的注册设备被写回本地 Active Directory, 以便它们可用于条件访问。

- 默认情况下, 将启用[意外删除](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes)以帮助防止同时删除的对象过多 (每个同步有500个以上的对象)。 您可以更改此设置以满足组织的需求。

- 默认情况下会为 express 安装启用[自动升级](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade), 并有助于确保你的 Azure AD Connect 版本始终是最新的。
