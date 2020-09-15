---
title: 错误 AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709141"
---
# <a name="error-attributevaluemustbeunique"></a>错误： AttributeValueMustBeUnique

AttributeValueMustBeUnique 错误的最常见原因是两个对象具有不同的 SourceAnchor (immutableId) 具有相同的 ProxyAddresses 和/或 UserPrincipalName 属性值。 若要修复 AttributeValueMustBeUnique 错误，请执行以下操作：
  
1. 标识复制的 proxyAddresses、userPrincipalName 或其他导致错误的属性值。 此外，还应确定冲突中涉及的两个 (或多个) 对象。 Azure AD Connect Health 生成的报告可帮助您识别这两个对象。
    
2. 确定哪个对象应继续具有重复的值以及哪个对象不应出现的情况。
    
3. 从不应具有该值的对象中移除重复的值。 请注意，应在来源于对象的目录中进行更改。 在某些情况下，您可能需要删除发生冲突的对象之一。
    
4. 如果您在本地 AD 中进行了更改，则允许 Azure AD Connect 同步错误的更改以进行修复。
    

