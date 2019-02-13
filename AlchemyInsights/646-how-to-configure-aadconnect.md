---
title: 646 如何配置 AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: dd6d6986b23c8adcc98fe713bacf32fb5bf8b4b6
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29915552"
---
# <a name="configure-sync-features"></a>配置同步功能

Azure AD 连接提供了众多功能的默认情况下，启用或更高版本可以启用。某些功能需要特定环境中的其他配置。
  
- [筛选](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering)限制对象同步到 Azure AD。默认情况下，所有用户、 联系人、 组和 Windows 10 都同步计算机帐户。您可以包括或排除基于域、 Ou、 或其他属性的对象。 
    
- [密码哈希同步](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization)同步从内部部署 Active Directory 密码哈希与 Azure AD。这将允许密码管理在一个位置，但相同密码中同时使用内部部署和云环境。由于 Active Directory 的权威源，您可以使用您自己的密码策略。 
    
- [自助服务密码重置 (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr)允许用户仍将应用您的本地密码策略时重置云中自己的密码。 
    
- [设备写回](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback)允许 Azure AD 以便它们可用于条件的访问，重新写入到内部部署 Active Directory 中注册的设备。 
    
- [防止意外删除](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes)默认情况下启用为了帮助防止太多同时对象删除 （每个同步多于 500 个对象）。您可以更改此设置以满足组织的需求。 
    
- 对于 express 安装默认情况下启用[自动升级](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)并有助于确保您的 Azure AD 连接版本始终是最新。 
    

