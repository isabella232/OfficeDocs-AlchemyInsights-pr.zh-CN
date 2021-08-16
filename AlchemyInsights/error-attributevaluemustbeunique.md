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
ms.openlocfilehash: 37d6764d19d9cfbb0899a5ab85a4b1530896568adc364122075b7d6f2a32970a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54002110"
---
# <a name="error-attributevaluemustbeunique"></a>错误：AttributeValueMustBeUnique

AttributeValueMustBeUnique 错误的最常见原因是两个对象的 SourceAnchor (immutableId) ProxyAddresses 和/或 UserPrincipalName 属性的值相同。 若要修复 AttributeValueMustBeUnique 错误：
  
1. 标识重复的 proxyAddresses、userPrincipalName 或其他导致错误的属性值。 还要确定冲突 (两) 两个或多个对象。 Azure AD 连接 Health for sync 生成的报告可以帮助你识别这两个对象。
    
2. 确定哪个对象应继续具有重复的值，以及不应包含的对象。
    
3. 从不应具有该值的对象中删除重复的值。 请注意，应在对象的来源目录中做出更改。 在某些情况下，可能需要删除其中一个发生冲突的对象。
    
4. 如果你在本地 AD 中进行了更改，请让 Azure AD 连接同步更改，以修复错误。
    

