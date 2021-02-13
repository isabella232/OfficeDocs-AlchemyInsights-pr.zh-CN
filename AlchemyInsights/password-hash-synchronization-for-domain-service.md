---
title: 域服务的密码哈希同步
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162915"
---
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="a2b48-102">域服务的密码哈希同步</span><span class="sxs-lookup"><span data-stu-id="a2b48-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="a2b48-103">**如果 Azure AD DS 实例提示启用密码哈希同步**</span><span class="sxs-lookup"><span data-stu-id="a2b48-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="a2b48-104">所遇到的场景是，你正在运行一个混合环境，用户从预置的 Azure Active Directory 域服务 (AD DS) 环境中进行同步。</span><span class="sxs-lookup"><span data-stu-id="a2b48-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="a2b48-105">尽管已将密码散列同步从预置 AD DS 到 Azure AD 租户，但仍会遇到这种情况。</span><span class="sxs-lookup"><span data-stu-id="a2b48-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="a2b48-106">**原因**</span><span class="sxs-lookup"><span data-stu-id="a2b48-106">**Cause**</span></span>

<span data-ttu-id="a2b48-107">出现这种情况的原因是，Azure AD Connect 默认情况下没有同步 Azure AD DS 所需的传统新技术 LAN Manager (NTLM) 和 Kerberos 密码哈希。</span><span class="sxs-lookup"><span data-stu-id="a2b48-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="a2b48-108">**解决方法**</span><span class="sxs-lookup"><span data-stu-id="a2b48-108">**Workaround**</span></span> 

<span data-ttu-id="a2b48-109">需要配置 Azure AD Connect 来同步 NTLM 和 Kerberos 身份验证所需的这些密码哈希。</span><span class="sxs-lookup"><span data-stu-id="a2b48-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="a2b48-110">配置 Azure AD Connect 后，预置账户创建或密码更改事件也会随即将传统密码哈希同步到 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="a2b48-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="a2b48-111">有关这方面的更多信息以及有关如何在 Azure AD DS 混合环境中启用密码同步的指导，请参见[此处](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync)。</span><span class="sxs-lookup"><span data-stu-id="a2b48-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>