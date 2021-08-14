---
title: '902 (对象重复导致同步错误) '
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
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998769"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>由于对象重复导致同步错误

目录同步完成后，您可能会收到以下错误消息之一Microsoft 365：

- 无法更新此对象Microsoft Online Services因为与此对象关联的以下属性的值可能已经与本地目录中的另一个对象相关联。

- 同一代理地址的同步对象已存在于你的Microsoft Online Services目录中。

- 无法更新此对象，因为与此对象关联的以下属性具有可能已经与本地目录服务中的另一个对象关联的值：UserPrincipalName。

若要识别和修复此问题，请下载并运行 [IdFix DirSync 错误修正工具](https://github.com/Microsoft/idfix)。

有关详细信息，请参阅[KB2647098。](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)
