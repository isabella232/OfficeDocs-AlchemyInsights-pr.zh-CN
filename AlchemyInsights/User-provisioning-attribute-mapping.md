---
title: 用户预配的属性映射
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
- "7851"
- "9004348"
ms.openlocfilehash: 73da476cc5913a16911839a59b80959d3c99a8bc22471febe421b022ce2c49ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918133"
---
# <a name="user-provisioning-attribute-mapping"></a>用户预配的属性映射

1. 若要解决已知属性映射问题，请参阅 [属性映射](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings)。 
2. Microsoft Azure Active Directory (AD) 支持将用户预配到第三方 SaaS 应用程序，例如 Salesforce、G Suite 和其他应用程序。 如果为第三方 SaaS 应用程序启用了用户设置，则 Azure 门户通过属性映射控制其属性值。 若要了解如何自定义默认属性映射，请参阅 [在 Azure Active Directory 中自定义 SaaS 应用程序的用户预配属性映射](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes)。
    - 若要详细了解 SaaS 应用的用户设置，请参阅 [什么是 Azure AD 中自动 SaaS 应用用户设置？](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning) 
3. 为用户预配自定义属性映射时，可能会发现想要映射的属性不会显示在源属性列表中。 本文，即 [将属性从本地 Active Directory 同步到 Azure AD，以将其预配到应用程序](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping)，说明了如何通过将缺少的属性从本地 AD 同步到 Azure AD 来添加这一属性。
