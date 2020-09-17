---
title: 如何启用无缝 SSO
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: f3581549823e1ec650a3717780bc07e9944d4c1c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780517"
---
# <a name="how-to-enable-seamless-sso"></a>如何启用无缝 SSO

通过 [AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect)启用无缝 SSO。
  
如果要执行 Azure AD Connect 的全新安装，请选择 " [自定义安装路径](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom)"。 在 " **用户登录** " 页上，选择 " **启用单一登录"** 选项。
  
若要验证是否正确启用了无缝 SSO，请执行以下操作：
  
1. 以全局管理员身份登录到 [Azure Active Directory 管理中心](https://aad.portal.azure.com) 。

2. 在左窗格中选择 " **Azure Active Directory** "。

3. 验证是否 **启用了**无缝单一登录。

若要了解详细信息，请参阅 [Azure Active Directory 无缝单一登录：快速入门](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start)。
  