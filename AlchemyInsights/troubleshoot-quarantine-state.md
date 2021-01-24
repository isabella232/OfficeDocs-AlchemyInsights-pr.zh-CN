---
title: 隔离状态疑难解答
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7853"
- "9004348"
ms.openlocfilehash: 3ee932b7788f4aff3c8bc762c5c917124edfe065
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/22/2021
ms.locfileid: "49935341"
---
# <a name="troubleshoot-quarantine-state"></a><span data-ttu-id="8793f-102">隔离状态疑难解答</span><span class="sxs-lookup"><span data-stu-id="8793f-102">Troubleshoot quarantine state</span></span>

<span data-ttu-id="8793f-103">Azure Active Directory (AD) 预配服务监视配置的运行状况。</span><span class="sxs-lookup"><span data-stu-id="8793f-103">The Azure Active Directory (AD) provisioning service monitors the health of your configuration.</span></span> <span data-ttu-id="8793f-104">它还可以将不正常的应用置于 **隔离** 状态。</span><span class="sxs-lookup"><span data-stu-id="8793f-104">It also places unhealthy apps in a **quarantine** state.</span></span> <span data-ttu-id="8793f-105">如果对目标系统进行的大多数或者所有呼叫始终失败，则预配作业将标记为 **隔离**。</span><span class="sxs-lookup"><span data-stu-id="8793f-105">If most, or all, of the calls made against the target system consistently fail, then the provisioning job is marked as **in quarantine**.</span></span> <span data-ttu-id="8793f-106">失败的实例有 **因为管理员凭据无效而收到错误**。</span><span class="sxs-lookup"><span data-stu-id="8793f-106">An example of a failure is **an error received because of invalid admin credentials**.</span></span> <span data-ttu-id="8793f-107">有关详细信息，请参阅 [隔离状态中的应用程序预配](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-quarantine-status)。</span><span class="sxs-lookup"><span data-stu-id="8793f-107">For more information, see [Application provisioning in quarantine status](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-quarantine-status).</span></span>

<span data-ttu-id="8793f-108">若要解决云同步问题，请参阅 [预配隔离的问题](https://docs.microsoft.com/azure/active-directory/cloud-sync/how-to-troubleshoot#provisioning-quarantined-problems)。</span><span class="sxs-lookup"><span data-stu-id="8793f-108">To troubleshoot cloud sync, see [Provisioning quarantined problems](https://docs.microsoft.com/azure/active-directory/cloud-sync/how-to-troubleshoot#provisioning-quarantined-problems).</span></span> 
