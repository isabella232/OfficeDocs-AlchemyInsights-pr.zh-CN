---
title: 在 EXO 中以启用邮件方式发送公用文件夹
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 22aa3e8f46c2ff4f62cb520b9498041dffb9d3a3eb607d788cc97b10bf32dbb5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052556"
---
# <a name="sendas-mail-enabled-public-folder"></a>SendAs 启用邮件的公用文件夹

以下示例将启用邮件的公用文件夹 NewPF1 的"发送方式"权限分配给用户为用户为用户。。

Add-RecipientPermission -Identity 'NewPF1' -Trustee "Trustee" -AccessRights 'SendAs'

有关语法和参数的详细信息，请参阅为已启用邮件的公用文件夹分配"代理发送"或" [代表发送"权限](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs)。

