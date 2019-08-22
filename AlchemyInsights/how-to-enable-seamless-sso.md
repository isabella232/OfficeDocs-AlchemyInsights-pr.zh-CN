---
title: 如何启用无缝 SSO
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: 249d388564294f65e759f84b7fcb09278e05cc12
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36540675"
---
# <a name="how-to-enable-seamless-sso"></a>如何启用无缝 SSO

通过[AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect)启用无缝 SSO。
  
如果要执行 Azure AD Connect 的全新安装, 请选择 "[自定义安装路径](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom)"。 在 "**用户登录**" 页上, 选择 "**启用单一登录"** 选项。
  
若要验证是否正确启用了无缝 SSO, 请执行以下操作:
  
1. 以全局管理员身份登录到[Azure Active Directory 管理中心](https://aad.portal.azure.com)。

2. 在左窗格中选择 " **Azure Active Directory** "。

3. 验证是否**启用了**无缝单一登录。

若要了解详细信息, 请参阅[Azure Active Directory 无缝单一登录: 快速入门](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start)。
  