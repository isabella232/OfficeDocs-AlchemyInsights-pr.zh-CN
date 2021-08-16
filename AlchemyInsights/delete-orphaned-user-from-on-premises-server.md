---
title: 从本地服务器中删除孤立用户
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: a6af617fa4235868f0754ff4c06f4cc73b1700ef14ea449dd1886ab100ddd384
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102231"
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