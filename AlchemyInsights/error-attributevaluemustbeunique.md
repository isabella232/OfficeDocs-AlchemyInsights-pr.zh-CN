---
title: 错误 AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 5ac56fa78c66cf3b246bc0cc01f040e27310d629
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36526963"
---
# <a name="error-attributevaluemustbeunique"></a>错误: AttributeValueMustBeUnique

AttributeValueMustBeUnique 错误最常见的原因是具有不同的 SourceAnchor (immutableId) 的两个对象具有相同的 ProxyAddresses 和/或 UserPrincipalName 属性值。 若要修复 AttributeValueMustBeUnique 错误, 请执行以下操作:
  
1. 标识复制的 proxyAddresses、userPrincipalName 或其他导致错误的属性值。 此外, 还应确定冲突中涉及的两个或多个对象。 Azure AD Connect Health 生成的报告可帮助您识别这两个对象。
    
2. 确定哪个对象应继续具有重复的值以及哪个对象不应出现的情况。
    
3. 从不应具有该值的对象中移除重复的值。 请注意, 应在来源于对象的目录中进行更改。 在某些情况下, 您可能需要删除发生冲突的对象之一。
    
4. 如果您在本地 AD 中进行了更改, 则允许 Azure AD Connect 同步错误的更改以进行修复。
    

