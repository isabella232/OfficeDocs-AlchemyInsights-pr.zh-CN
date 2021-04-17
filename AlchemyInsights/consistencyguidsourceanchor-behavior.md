---
title: ConsistencyGuid / sourceAnchor 行为
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816982"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor 行为

Azure AD Connect (1.1.524.0 版) 现在便于将 msDS-ConsistencyGuid 用作 sourceAnchor 属性。 使用此功能时，Azure AD Connect 会自动将同步规则配置为：
  
- 使用 msDS-ConsistencyGuid 作为 User 对象的 sourceAnchor 属性。 ObjectGUID 用于其他对象类型。
    
- 对于未填充其 msDS-ConsistencyGuid 属性的任何给定本地 AD User 对象，Azure AD Connect 将其 objectGUID 值写回本地 Active Directory 中的 msDS-ConsistencyGuid 属性。 填充 msDS-ConsistencyGuid 属性后，Azure AD Connect 再将该对象导出到 Azure AD。
    
 **注意：** 将本地 AD 对象导入 Azure AD Connect (即导入 AD 连接器空间并预测到 Metaverse) 后，你不能再更改其 sourceAnchor 值。 若要指定给定本地 AD 对象的 sourceAnchor 值，请配置其 msDS-ConsistencyGuid 属性，然后再将其导入 Azure AD Connect。 
  
有关 SourceAnchor 和 ConsistencyGuid 的信息，请参阅以下内容 [：Azure AD Connect：设计概念](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

