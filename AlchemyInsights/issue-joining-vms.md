---
title: 加入虚拟机的问题
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884557"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="19a31-102">加入虚拟机的问题</span><span class="sxs-lookup"><span data-stu-id="19a31-102">Issue joining VMs</span></span>

<span data-ttu-id="19a31-103">要解决加入虚拟机时出现的问题，请执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="19a31-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="19a31-104">试试使用 **UPN** 格式（例如，“joeuser@contoso.com”）来代替 **SAMAccountName** 格式 ('CONTOSO\joeuser')。</span><span class="sxs-lookup"><span data-stu-id="19a31-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="19a31-105">确保你已经按照 *入门* 中所列步骤启用了密码同步。</span><span class="sxs-lookup"><span data-stu-id="19a31-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="19a31-106">确保受影响的用户账户不是 Azure AD 租户中的外部账户。</span><span class="sxs-lookup"><span data-stu-id="19a31-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="19a31-107">外部用户无法登陆到托管的域，因为 Azure AD 域服务没有此类用户账户的凭据。</span><span class="sxs-lookup"><span data-stu-id="19a31-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="19a31-108">如果受影响的用户账户是仅使用云的用户账户，请在启用 Azure AD 域服务后确保用户已经更改了他们的密码。</span><span class="sxs-lookup"><span data-stu-id="19a31-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="19a31-109">此步骤后，Azure AD 域服务所需的凭据哈希值将会生成。</span><span class="sxs-lookup"><span data-stu-id="19a31-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="19a31-110">如果从本地目录中同步了受影响的用户，请确认推荐的 Azure AD Connect 版本已经进行过配置，以便进行完整的同步。</span><span class="sxs-lookup"><span data-stu-id="19a31-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="19a31-111">如果在确认步骤 4 后问题仍然发生，请在你的同步机器上执行下列命令：</span><span class="sxs-lookup"><span data-stu-id="19a31-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="19a31-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="19a31-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>