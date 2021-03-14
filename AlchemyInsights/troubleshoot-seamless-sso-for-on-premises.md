---
title: 本地无缝单一登录 (SSO) 疑难解答
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9370"
- "9004357"
ms.openlocfilehash: a8d14b12bfb3b02da0468eee70af26344465a2a2
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50753385"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-for-on-premises"></a><span data-ttu-id="95eaf-102">本地无缝单一登录 (SSO) 疑难解答</span><span class="sxs-lookup"><span data-stu-id="95eaf-102">Troubleshoot Seamless Single Sign-on (SSO) for on-premises</span></span>

<span data-ttu-id="95eaf-103">要解决无缝单一登录 (SSO) 问题，请执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="95eaf-103">To resolve Seamless Single Sign-on (SSO) issues, perform the following steps:</span></span>

<span data-ttu-id="95eaf-104">**如何滚动更新 AZUREADSSO 计算机帐户的 Kerberos 解密密钥？**</span><span class="sxs-lookup"><span data-stu-id="95eaf-104">**How can I roll over the Kerberos decryption key of the AZUREADSSO computer account?**</span></span>

<span data-ttu-id="95eaf-105">我们强烈建议至少每 30 天滚动更新一次 Kerberos 解密密钥。</span><span class="sxs-lookup"><span data-stu-id="95eaf-105">We highly recommend that you roll over the Kerberos decryption key at least every 30 days.</span></span> <span data-ttu-id="95eaf-106">要手动完成此操作，请参阅 [如何滚动更新 Kerberos 解密密钥](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#)。</span><span class="sxs-lookup"><span data-stu-id="95eaf-106">To do this manually, see [How to roll over Kerberos decryption keys](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span></span>

<span data-ttu-id="95eaf-107">**配置无缝 SSO**</span><span class="sxs-lookup"><span data-stu-id="95eaf-107">**Configure Seamless SSO**</span></span>

<span data-ttu-id="95eaf-108">要部署无缝 SSO，请执行 [Azure Active Directory 无缝单一登录：快速启动](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys) 中的步骤。</span><span class="sxs-lookup"><span data-stu-id="95eaf-108">To deploy Seamless SSO, follow the steps in [Azure Active Directory Seamless Single Sign-On: Quickstart](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span></span>

<span data-ttu-id="95eaf-109">**公告**</span><span class="sxs-lookup"><span data-stu-id="95eaf-109">**Advisory**</span></span>

- <span data-ttu-id="95eaf-110">[Azure Active Directory 无缝单一登录：常见问题解答](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) - 在此篇文章中，我们处理了有关 Azure Active Directory 无缝单一登录 （无缝 SSO） 的常见问题。</span><span class="sxs-lookup"><span data-stu-id="95eaf-110">[Azure Active Directory Seamless Single Sign-On: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) - In this article, we address frequently asked questions about Azure Active Directory Seamless Single Sign-On (Seamless SSO).</span></span> <span data-ttu-id="95eaf-111">请继续检查新的内容。</span><span class="sxs-lookup"><span data-stu-id="95eaf-111">Keep checking back for new content.</span></span>
- <span data-ttu-id="95eaf-112">[Microsoft 问答](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - 本文提供有关如何就无缝 SSO 提出功能请求或技术问题的信息。</span><span class="sxs-lookup"><span data-stu-id="95eaf-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - This article provides information on how to make feature requests or ask technical questions about Seamless SSO.</span></span>

<span data-ttu-id="95eaf-113">**疑难解答**</span><span class="sxs-lookup"><span data-stu-id="95eaf-113">**Troubleshoot**</span></span>

<span data-ttu-id="95eaf-114">[Azure Active Directory 无缝单一登录疑难解答](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) - 本文帮助你查找有关 Azure Active Directory (Azure AD) 无缝单一登录（无缝 SSO）常见问题的疑难解答信息。</span><span class="sxs-lookup"><span data-stu-id="95eaf-114">[Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) - This article helps you find troubleshooting information about common problems regarding Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO).</span></span>







