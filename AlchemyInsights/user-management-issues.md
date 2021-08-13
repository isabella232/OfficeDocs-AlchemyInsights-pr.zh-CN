---
title: 用户管理问题
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 70f8def2a0f3419a9aa6325e376ba52fc35ec48b61f39ede99d7e58cd6c6c464
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971438"
---
# <a name="user-management-issues"></a>用户管理问题

**如果禁用属性"需要用户分配"（将此属性设置为 No），则当前已分配至应用程序的用户会发生什么情况？**

禁用 **需要用户分配** 不会影响当前已分配的用户。 禁用此属性将仅允许所有用户访问该应用程序。 列出的所有用户和应用程序中分配给组的用户仍然有效。

- 若要将应用限制到特定的一组用户，请参阅 [将Azure AD 应用限制为一组用户 - Microsoft 标识平台|Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.)。
- 若要从 Azure 门户内使用 PowerShell 将用户和组分配给 Azure Active Directory （Azure AD） 中的企业应用程序，请参阅 [在 Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)中管理应用的用户分配。
- 若要代理应用程序创建和管理权限，请参阅 [代理应用程序管理管理员权限 - Azure AD |Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles)。
- **向用户隐藏特定企业应用程序** - 按照以下步骤操作，从 **我的应用** 面板中隐藏所有 Microsoft 365 应用程序。 这些应用仍在 Office 365 门户中可见。

 1. 以目录的全局管理员登身份登录到 Azure 门户。 
 2. 选择 **Azure Active Directory**。 
 3. 选择 **用户**。 
 4. 选择 **用户设置**。 
 5. 在 **企业应用程序** 中，点击 **"管理最终用户启动和查看其应用程序**。 
 6. 对于 **用户只能在 Office 365 门户中看到 Office 365 应用程序**，请单击" **是**。 
 7. 单击 **保存**。 
 8. 有关详细信息，请参阅 [Azure AD 设备中的用户体验中隐藏企业应用程序|Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- 如果向许多组织提供软件即服务 （SaaS） 应用程序，可以将应用程序配置为接受来自任何 Azure Active Directory （Azure AD） 租户的登录。 此配置称为"使应用程序成为多租户"。 任何 Azure AD 租户中的用户在同意通过你的应用程序用其账号后，将能够登录到你的应用程序。 有关详细信息，请参阅 [构建登录 Azure AD 用户的应用程序 - Microsoft 标识平台|Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant)。

- **最终用户分配到应用程序后如何访问该应用程序？**

企业应用程序模版中的每一个应用程序都有一个链接，供最终用户访问。 用户还可通过 **我的应用** 门户轻松访问该应用。

- **希望了解用户正在使用哪些应用程序和应用程序类型？**

可以从 **portal.azure.com >Azure Active Directory>Signins> 下载** 中，下载过去 30 天的登录报告。

- 了解如何 [许可授予租户范围的管理员](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) 并 [许可配置最终用户对应用程序](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent)。

- 了解 [许可的工作原理](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 以及 [管理对应用程序的许可](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests)。


