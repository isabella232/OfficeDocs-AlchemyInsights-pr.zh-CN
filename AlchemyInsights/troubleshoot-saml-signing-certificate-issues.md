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
ms.openlocfilehash: fb043122edf5f99325f0403810eb0dc119d254e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314410"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>SAML 签名证书问题疑难解答

要解决 SAML 签名证书问题，请执行以下建议步骤：

1. 添加支持 SSO 的企业应用程序时，Azure 将生成称为 [SAML 签名证书](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications)。 此证书的到期日期为 3 年。 若要更改证书的到期日期，请参阅 [自定义联合证书的到期日期，并回退到新的证书](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)。
2. Azure 将使用此证书来签名应用程序请求的 SAML 令牌，并将其发送给应用程序，获得成功的 SSO。 为完成此操作，请从 Azure 门户下载证书并将其发送给应用程序供应商，以完成 SSO 过程。

完成此过程后，应用程序将信任此证书，应用程序将接受由该证书签名的所有 SAML 令牌。

3. 如果此证书过期，请创建新证书，更新到应用程序供应商，然后使其在 Azure 侧处于活动状态。 有关详细信息，请参阅 [即将到期的证书](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)。

**注意**：如果证书过期，用户将不会受阻。

4. [添加电子邮件地址](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration)以在当前证书到期之前接收通知。

**注意**：步骤 4 是可选的。

5. 更改应用程序的 SAML 证书签名选项和证书签名算法。 有关详细信息，请参阅 [签名选项和签名算法](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)。

