---
title: 部署 AD FS
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1300012"
- "7420"
ms.openlocfilehash: a304504f7483036884878639dfa6ebfc3cdfcac8
ms.sourcegitcommit: 05a9dd3121c21322dc9ddec4c2eec548cafd5a43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50165245"
---
# <a name="deploy-ad-fs"></a><span data-ttu-id="f5767-102">部署 AD FS</span><span class="sxs-lookup"><span data-stu-id="f5767-102">Deploy AD FS</span></span>

<span data-ttu-id="f5767-103">AD FS (Active Directory 联合身份验证) 使用本地基础结构对用户进行身份验证，以验证 Office 365 服务。</span><span class="sxs-lookup"><span data-stu-id="f5767-103">An Active Directory Federation Services (AD FS) deployment uses your on-premises infrastructure to authenticate users for ‎Office 365 services.</span></span> <span data-ttu-id="f5767-104">通过联合登录，用户可以登录到与 Azure Active Directory (Azure AD) 集成的 Office 365 服务和软件即服务 (SAAS) 应用程序。</span><span class="sxs-lookup"><span data-stu-id="f5767-104">With federated sign-in, you can enable users to sign in to Office 365 services and Software as a Service (SAAS) applications that are integrated with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="f5767-105">联合登录通过 AD FS 针对本地 Active Directory 对用户进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="f5767-105">Federated sign-in authenticates users against your on-premises Active Directory via AD FS.</span></span> <span data-ttu-id="f5767-106">此外，在企业网络中，用户无需重新输入其密码。</span><span class="sxs-lookup"><span data-stu-id="f5767-106">Also, while on the corporate network, users won't be required to reenter their passwords.</span></span>

<span data-ttu-id="f5767-107">[AD FS 部署](https://go.microsoft.com/fwlink/?linkid=2071178)顾问提供有关部署本地 AD FS 基础结构的分步指南，该基础结构会验证 Microsoft 365 和 Office 365 服务的用户身份。</span><span class="sxs-lookup"><span data-stu-id="f5767-107">The [AD FS deployment advisor](https://go.microsoft.com/fwlink/?linkid=2071178) provides you with step-by-step guidance on deploying an on-premises AD FS infrastructure that authenticates users for Microsoft 365 and Office 365 services.</span></span> <span data-ttu-id="f5767-108">借助本指南，贵组织可以审阅 AD FS 组件和要求、获取和安装部署所需的 SSL 证书，以及安装所需的 Web 应用程序代理服务器。</span><span class="sxs-lookup"><span data-stu-id="f5767-108">With this guide, your organization can review AD FS components and requirements, acquire and install SSL certificates that are necessary for deployment, and install a required web application proxy server.</span></span>
