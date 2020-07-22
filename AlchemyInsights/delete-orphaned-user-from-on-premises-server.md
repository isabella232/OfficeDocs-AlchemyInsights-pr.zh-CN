---
title: 从本地服务器中删除孤立用户
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/20/2020
ms.locfileid: "45186096"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>从本地服务器中删除孤立用户

若要删除孤立用户，请按照下列步骤操作：

1. 按照[什么是使用 Azure Active Directory 的混合标识？](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories)中的说明强制实施目录同步。

2. 若要验证目录同步，请参阅[什么是使用 Azure Active Directory 的混合标识？](https://technet.microsoft.com/library/jj151797.aspx)。

3. 如果同步正常进行，但 Active Directory 对象删除没有传播到 Azure AD，则请对 Windows PowerShell cmdlet 使用以下 Azure Active Directory 模块之一，手动删除孤立对象：

    Remove-MsolContact  
    Remove-MsolGroup  
    Remove-MsolUser

    例如，若要删除孤立用户 ID john.smith@contoso.com（它最初是通过目录同步创建的），请运行 cmdlet：

    Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com