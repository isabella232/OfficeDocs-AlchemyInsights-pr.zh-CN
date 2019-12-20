---
title: 团队4c7 错误
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/19/2019
ms.locfileid: "40795976"
---
# <a name="4c7-error-in-microsoft-teams"></a>Microsoft 团队中的4c7 错误

出现此错误的原因是 Microsoft 团队需要表单身份验证。 当您部署 Active Directory 联合身份验证服务（AD FS）时，默认情况下不会为 intranet 启用表单身份验证。 如果 Windows 集成身份验证失败，系统会提示您使用表单身份验证进行登录。

若要解决此问题，请使用具有 Active Directory 本地副本的计算机上的 AD FS Microsoft 管理控制台（MMC）管理单元启用表单身份验证。 要实现这一点，请执行下列步骤： 

1. 在导航窗格中，浏览到 "**身份验证策略**"。
2. 在 "详细信息" 窗格的 "**操作**" 下，选择 "**编辑全局主身份验证**"。
3. 在 " **Intranet** " 选项卡上，选择 "**表单身份验证**"。
4. 选择 **"确定"** （或 "**应用**"）。