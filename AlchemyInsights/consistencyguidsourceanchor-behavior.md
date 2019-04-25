---
title: ConsistencyGuid/sourceAnchor 行为
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: cb1b50792b07a1b3b69607bf2f6824141a15922f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32408098"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor 行为

Azure AD Connect (版本1.1.524.0 和之后) 现在有利于将 ConsistencyGuid 用作 sourceAnchor 属性。 使用此功能时, Azure AD Connect 会自动将同步规则配置为:
  
- 使用 ConsistencyGuid 作为 User 对象的 sourceAnchor 属性。 ObjectGUID 用于其他对象类型。
    
- 对于任何给定的本地 AD 用户对象, 其 ConsistencyGuid 属性未填充, Azure AD Connect 将其 objectGUID 值写入本地 Active Directory 中的 ConsistencyGuid 属性。 在填充 ConsistencyGuid 属性后, Azure ad Connect 然后将该对象导出到 Azure ad。
    
 **注意:** 将本地 AD 对象导入到 Azure AD Connect (即, 导入到 AD 连接器空间并投影到元节) 后, 将无法再更改它的 sourceAnchor 值。 若要指定给定内部部署 AD 对象的 sourceAnchor 值, 请先配置其 ConsistencyGuid 属性, 然后再将其导入到 Azure AD Connect。 
  
有关 SourceAnchor 和 ConsistencyGuid 的详细信息, 请参阅以下内容: [Azure AD Connect: 设计概念](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

