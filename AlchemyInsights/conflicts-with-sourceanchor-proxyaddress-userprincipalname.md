---
title: 与 SourceAnchor、ProxyAddress 或 UserPrincipalName 存在冲突
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1699"
- "1300022"
ms.openlocfilehash: 2d58078fcabb416c418b67a2f2ce2eba679a18c6ecf3846c534bde74188d7827
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033052"
---
# <a name="conflicts-with-sourceanchor-proxyaddress-userprincipalname"></a>与 SourceAnchor、ProxyAddress 或 UserPrincipalName 存在冲突

如果你在同步期间收到诸如“你的目录中存在已同步且 ProxyAddress 或 UserPrincipalName 相同的对象”的错误，请参阅[诊断和修正“重复属性同步”错误](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors)。

此外，还需考虑启用重复属性复原。 有关详细信息，请参阅[标识同步和重复属性复原](https://aka.ms/duplicateattributeresiliency)。