---
title: 配置 LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49876537"
---
# <a name="configure-ldap"></a><span data-ttu-id="aee0d-102">配置 LDAP</span><span class="sxs-lookup"><span data-stu-id="aee0d-102">Configure LDAP</span></span>

<span data-ttu-id="aee0d-103">若要配置 LDAP，请执行下列操作：</span><span class="sxs-lookup"><span data-stu-id="aee0d-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="aee0d-104">在 Azure 门户上检查域 [的运行状况](https://aka.ms/aadds-health)。</span><span class="sxs-lookup"><span data-stu-id="aee0d-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="aee0d-105">确保有效的 Azure AD 订阅可用，并且已启用 Azure AD 域服务。</span><span class="sxs-lookup"><span data-stu-id="aee0d-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="aee0d-106">启用安全 LDAP 所需的证书必须从受信任的公共证书颁发机构获取，或者是自签名证书。</span><span class="sxs-lookup"><span data-stu-id="aee0d-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="aee0d-107">确保证书遵循所需的 [准则](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)。</span><span class="sxs-lookup"><span data-stu-id="aee0d-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="aee0d-108">**证书无效**</span><span class="sxs-lookup"><span data-stu-id="aee0d-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="aee0d-109">若要续订证书，请按照步骤创建新证书并重新加载：[配置 LDAP。](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="aee0d-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="aee0d-110">若要解决 Azure Active directory 域服务中安全 LDAP 警报的已知问题，请参阅["解决 LDAP 警报"。](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="aee0d-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
