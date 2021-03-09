---
title: SAML 签名证书问题疑难解答
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529162"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="5810d-102">SAML 签名证书问题疑难解答</span><span class="sxs-lookup"><span data-stu-id="5810d-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="5810d-103">要解决 SAML 签名证书问题，请执行以下建议步骤：</span><span class="sxs-lookup"><span data-stu-id="5810d-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="5810d-104">添加支持 SSO 的企业应用程序时，Azure 将生成称为 [SAML 签名证书](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications)。</span><span class="sxs-lookup"><span data-stu-id="5810d-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="5810d-105">此证书的到期日期为 3 年。</span><span class="sxs-lookup"><span data-stu-id="5810d-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="5810d-106">若要更改证书的到期日期，请参阅 [自定义联合证书的到期日期，并回退到新的证书](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)。</span><span class="sxs-lookup"><span data-stu-id="5810d-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="5810d-107">Azure 将使用此证书来签名应用程序请求的 SAML 令牌，并将其发送给应用程序，获得成功的 SSO。</span><span class="sxs-lookup"><span data-stu-id="5810d-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="5810d-108">为完成此操作，请从 Azure 门户下载证书并将其发送给应用程序供应商，以完成 SSO 过程。</span><span class="sxs-lookup"><span data-stu-id="5810d-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="5810d-109">完成此过程后，应用程序将信任此证书，应用程序将接受由该证书签名的所有 SAML 令牌。</span><span class="sxs-lookup"><span data-stu-id="5810d-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="5810d-110">如果此证书过期，请创建新证书，更新到应用程序供应商，然后使其在 Azure 侧处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="5810d-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="5810d-111">有关详细信息，请参阅 [即将到期的证书](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)。</span><span class="sxs-lookup"><span data-stu-id="5810d-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="5810d-112">如果证书过期，用户将不会受阻。</span><span class="sxs-lookup"><span data-stu-id="5810d-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="5810d-113">[为在当前证书](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) 之前接收的通知添加电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="5810d-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="5810d-114">步骤 4 是可选的。</span><span class="sxs-lookup"><span data-stu-id="5810d-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="5810d-115">更改应用程序的 SAML 证书签名选项和证书签名算法。</span><span class="sxs-lookup"><span data-stu-id="5810d-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="5810d-116">有关详细信息，请参阅 [签名选项和签名算法](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)。</span><span class="sxs-lookup"><span data-stu-id="5810d-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

