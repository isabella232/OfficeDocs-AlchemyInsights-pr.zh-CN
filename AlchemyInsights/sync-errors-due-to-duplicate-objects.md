---
title: 902 (由于重复的对象而产生的同步错误)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: ce7eeb07cfde16e6d6856a9369c042dcf4f05b63
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/13/2019
ms.locfileid: "31859094"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>由于复制对象导致的同步错误

目录同步完成时, 您可能会收到以下错误消息之一:

- 无法更新 Microsoft Online Services 中的此对象, 因为与此对象相关联的以下属性的值可能已与本地目录中的另一个对象相关联。

- 您的 Microsoft Online Services 目录中已存在具有相同代理地址的同步对象。

- 无法更新此对象, 因为与此对象相关联的以下属性的值可能已经与本地目录服务中的另一个对象相关联: UserPrincipalName。

若要确定并解决问题, 请下载并运行[IdFix DirSync 错误修正工具](https://www.microsoft.com/download/details.aspx?id=36832)。

有关详细信息, 请参阅[KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)。
