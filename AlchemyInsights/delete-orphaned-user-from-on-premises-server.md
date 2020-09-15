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
ms.openlocfilehash: 537ae7edebfa5a4ab71c2141d549d732ed4f883f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680125"
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