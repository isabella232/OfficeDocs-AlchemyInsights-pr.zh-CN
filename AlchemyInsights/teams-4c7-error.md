---
title: Teams 4c7 错误
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049298"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7 错误Microsoft Teams

发生此错误的原因是Microsoft Teams表单身份验证。 在将 Active Directory 联合身份验证服务 (AD FS) 时，默认情况下不会为 Intranet 启用表单身份验证。 如果Windows身份验证失败，系统将提示你使用表单身份验证登录。

若要解决此问题，请通过使用本地 Active Directory 副本的计算机上 AD FS Microsoft 管理控制台 (MMC) 管理单元启用表单身份验证。 为此，请按照下列步骤操作： 

1. 在导航窗格中，浏览到"**身份验证策略"。**
2. 在 **详细信息窗格中** 的"操作"下，选择 **"编辑全局主身份验证"。**
3. 在 **"Intranet"选项卡** 上，选择"**表单身份验证"。**
4. 选择 **"确定** ("或 **"应用**) "。