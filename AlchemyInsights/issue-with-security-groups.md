---
title: 安全组问题
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
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162916"
---
# <a name="issue-with-security-groups"></a><span data-ttu-id="136a1-102">安全组问题</span><span class="sxs-lookup"><span data-stu-id="136a1-102">Issue with security groups</span></span>

<span data-ttu-id="136a1-103">**如果收到网络错误 AADDS104**</span><span class="sxs-lookup"><span data-stu-id="136a1-103">**If you are getting Network Error AADDS104**</span></span>

<span data-ttu-id="136a1-104">无效网络安全组规则是Azure Active Directory Domain Services（AD DS）出现网络错误的最常见原因。</span><span class="sxs-lookup"><span data-stu-id="136a1-104">Invalid network security group rules are the most common cause of network errors for Azure Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="136a1-105">虚拟网络的网络安全组必须允许访问特定的端口和协议。</span><span class="sxs-lookup"><span data-stu-id="136a1-105">The network security group for the virtual network must allow access to specific ports and protocols.</span></span> <span data-ttu-id="136a1-106">如果这些端口受阻，Azure 平台就无法监控或更新托管域。</span><span class="sxs-lookup"><span data-stu-id="136a1-106">If these ports are blocked, the Azure platform can't monitor or update the managed domain.</span></span> <span data-ttu-id="136a1-107">Azure AD 和 Azure AD DS 之间的同步也会受到影响。</span><span class="sxs-lookup"><span data-stu-id="136a1-107">The synchronization between the Azure AD and Azure AD DS is also impacted.</span></span> <span data-ttu-id="136a1-108">请确保保持默认端口的开放，以避免服务中断。</span><span class="sxs-lookup"><span data-stu-id="136a1-108">Ensure you keep the default ports open to avoid interruption in service.</span></span>

<span data-ttu-id="136a1-109">若要了解并解决网络安全组配置问题的常见警报，请参阅 [添加并验证安全组](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules)。</span><span class="sxs-lookup"><span data-stu-id="136a1-109">To understand and to resolve common alerts for network security group configuration issues, see [Add and Verify Security Groups](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span></span>
