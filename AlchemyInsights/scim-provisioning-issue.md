---
title: SCIM 预配问题
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
- "7854"
- "9004348"
ms.openlocfilehash: aa5b4cbb99cb1a5a323b39101766bea55fd49064
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/22/2021
ms.locfileid: "49935352"
---
# <a name="scim-provisioning-issue"></a><span data-ttu-id="d39d6-102">SCIM 预配问题</span><span class="sxs-lookup"><span data-stu-id="d39d6-102">SCIM provisioning issue</span></span>

<span data-ttu-id="d39d6-103">自动预配是指在用户需要访问的云应用程序中创建用户标识和角色。</span><span class="sxs-lookup"><span data-stu-id="d39d6-103">Automatic provisioning refers to creating user identities and roles in the cloud applications that users need access to.</span></span> <span data-ttu-id="d39d6-104">除了创建用户标识外，自动设置还包括随着状态或角色更改而维护并删除用户标识。</span><span class="sxs-lookup"><span data-stu-id="d39d6-104">In addition to creating user identities, automatic provisioning includes the maintenance and removal of user identities as status or roles change.</span></span> <span data-ttu-id="d39d6-105">开始部署之前，可查看 [预配的工作原理](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works)，以了解 Azure Active Directory (AD) 预配如何工作，并获取配置建议。</span><span class="sxs-lookup"><span data-stu-id="d39d6-105">Before you start a deployment, you can review [How provisioning works](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) to learn how Azure Active Directory (AD) provision works, and get configuration recommendations.</span></span>

<span data-ttu-id="d39d6-106">作为应用程序开发人员，可以使用跨域身份管理 (SCIM) 用户管理 API 系统，以在应用程序和 Azure AD 之间自动预配用户和组。</span><span class="sxs-lookup"><span data-stu-id="d39d6-106">As an application developer, you can use the System for Cross-Domain Identity Management (SCIM) user management API to enable automatic provisioning of users and groups between your application and Azure AD.</span></span> <span data-ttu-id="d39d6-107">[使用 Azure AD 构建 SCIM 终结点和配置用户预配](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) 一文介绍了如何构建 SCIM 终结点，并将其与 Azure AD 预配服务集成。</span><span class="sxs-lookup"><span data-stu-id="d39d6-107">The [Build a SCIM endpoint and configure user provisioning with Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) article describes how to build an SCIM endpoint and integrate it with the Azure AD provisioning service.</span></span>



