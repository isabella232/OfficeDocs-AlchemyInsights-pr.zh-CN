---
title: '902 (由于复制对象而产生的同步错误) '
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737331"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>由于复制对象导致的同步错误

在 Microsoft 365 中的目录同步完成时，您可能会收到以下错误消息之一：

- 无法更新 Microsoft Online Services 中的此对象，因为与此对象相关联的以下属性的值可能已与本地目录中的另一个对象相关联。

- 您的 Microsoft Online Services 目录中已存在具有相同代理地址的同步对象。

- 无法更新此对象，因为与此对象相关联的以下属性的值可能已经与本地目录服务中的另一个对象相关联： UserPrincipalName。

若要确定并解决问题，请下载并运行 [IdFix DirSync 错误修正工具](https://www.microsoft.com/download/details.aspx?id=36832)。

有关详细信息，请参阅 [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)。
