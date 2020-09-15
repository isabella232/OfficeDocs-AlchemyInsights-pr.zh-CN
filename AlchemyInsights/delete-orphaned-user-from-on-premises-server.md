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
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="83fb6-102">从本地服务器中删除孤立用户</span><span class="sxs-lookup"><span data-stu-id="83fb6-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="83fb6-103">若要删除孤立用户，请按照下列步骤操作：</span><span class="sxs-lookup"><span data-stu-id="83fb6-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="83fb6-104">按照[什么是使用 Azure Active Directory 的混合标识？](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories)中的说明强制实施目录同步。</span><span class="sxs-lookup"><span data-stu-id="83fb6-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="83fb6-105">若要验证目录同步，请参阅[什么是使用 Azure Active Directory 的混合标识？](https://technet.microsoft.com/library/jj151797.aspx)。</span><span class="sxs-lookup"><span data-stu-id="83fb6-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="83fb6-106">如果同步正常进行，但 Active Directory 对象删除没有传播到 Azure AD，则请对 Windows PowerShell cmdlet 使用以下 Azure Active Directory 模块之一，手动删除孤立对象：</span><span class="sxs-lookup"><span data-stu-id="83fb6-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="83fb6-107">Remove-MsolContact</span><span class="sxs-lookup"><span data-stu-id="83fb6-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="83fb6-108">Remove-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="83fb6-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="83fb6-109">Remove-MsolUser</span><span class="sxs-lookup"><span data-stu-id="83fb6-109">Remove-MsolUser</span></span>

    <span data-ttu-id="83fb6-110">例如，若要删除孤立用户 ID john.smith@contoso.com（它最初是通过目录同步创建的），请运行 cmdlet：</span><span class="sxs-lookup"><span data-stu-id="83fb6-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="83fb6-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="83fb6-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>