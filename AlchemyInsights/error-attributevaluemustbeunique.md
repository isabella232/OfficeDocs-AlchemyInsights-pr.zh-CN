---
title: Error AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 35eb88624a5535e136ac1d01faf8e905bf00eb45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813750"
---
# <a name="error-attributevaluemustbeunique"></a>错误：AttributeValueMustBeUnique

AttributeValueMustBeUnique 错误的最常见原因是两个对象的 SourceAnchor (immutableId) ProxyAddresses 和/或 UserPrincipalName 属性的值相同。 若要修复 AttributeValueMustBeUnique 错误：
  
1. 标识重复的 proxyAddresses、userPrincipalName 或其他导致错误的属性值。 还要确定冲突 (两) 两个或多个对象。 Azure AD Connect Health 生成的用于同步的报告可帮助你标识这两个对象。
    
2. 确定哪个对象应继续具有重复的值，以及不应包含的对象。
    
3. 从不应具有该值的对象中删除重复的值。 请注意，应在对象的来源目录中做出更改。 在某些情况下，可能需要删除其中一个发生冲突的对象。
    
4. 如果你在本地 AD 中进行了更改，请让 Azure AD Connect 同步更改，以修复错误。
    

