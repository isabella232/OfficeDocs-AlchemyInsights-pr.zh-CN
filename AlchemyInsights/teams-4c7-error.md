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
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786659"
---
# <a name="4c7-error-in-microsoft-teams"></a>Microsoft Teams 中的 4c7 错误

发生此错误是因为 Microsoft Teams 需要表单身份验证。 在将 Active Directory 联合身份验证服务 (AD FS) 时，默认情况下不会为 Intranet 启用表单身份验证。 如果 Windows 集成身份验证失败，系统将提示你使用表单身份验证登录。

若要解决此问题，请通过使用本地 Active Directory 副本的计算机上 AD FS Microsoft 管理控制台 (MMC) 管理单元启用表单身份验证。 为此，请按照下列步骤操作： 

1. 在导航窗格中，浏览到"**身份验证策略"。**
2. 在 **详细信息窗格中** 的"操作"下，选择 **"编辑全局主身份验证"。**
3. 在 **"Intranet"选项卡** 上，选择"**表单身份验证"。**
4. 选择 **"确定** ("或 **"应用**) "。