---
title: 错误 AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7a97d1a5ff352b55833bd457e3220a56130d7e7e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499624"
---
# <a name="error-attributevaluemustbeunique"></a>错误： AttributeValueMustBeUnique

AttributeValueMustBeUnique 错误的最常见原因是具有不同 SourceAnchor (immutableId) 的两个对象具有相同的 ProxyAddresses 和/或 UserPrincipalName 属性的值。若要修复 AttributeValueMustBeUnique 错误：
  
1. 确定重复的 proxyAddresses、 userPrincipalName 或导致错误其他属性值。同时也会指出冲突中涉及的两个 （或多个） 的对象。由 Azure AD 连接运行状况的同步生成的报告可帮助您确定两个对象。
    
2. 确定哪个对象应继续具有重复的值和不应的对象。
    
3. 从不应包含该值的对象中删除重复的值。请注意，则应其中源自对象的目录中进行的更改。在某些情况下，您可能需要删除冲突对象之一。
    
4. 如果您在本地 AD 中进行更改，让同步更改该错误以获取固定的 Azure AD 连接。
    

