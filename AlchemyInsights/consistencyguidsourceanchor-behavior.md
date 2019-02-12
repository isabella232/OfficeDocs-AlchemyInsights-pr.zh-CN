---
title: ConsistencyGuid / sourceAnchor 行为
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: e1ffa9cf2b59570cb6ea3517efad7a55fd9489a8
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29927617"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor 行为

Azure AD 连接 (版本 1.1.524.0 和之后) 现在方便了 msDS ConsistencyGuid 用作 sourceAnchor 属性。使用此功能时，Azure AD 连接将自动配置同步规则：
  
- MsDS ConsistencyGuid 用作用户对象的 sourceAnchor 属性。ObjectGUID 用于其他对象类型。
    
- 为任何给定的本地 AD 用户其 msDS ConsistencyGuid 属性不填充、 Azure AD 连接写入其 objectGUID 值回内部部署 Active Directory 中的 msDS ConsistencyGuid 属性的对象。已填充 msDS ConsistencyGuid 属性后，Azure AD 连接然后将该对象导出到 Azure AD。
    
 **注意：** 一次内部部署 AD 对象导入到 Azure AD 连接 （即，导入到 AD 连接器空间和 Metaverse 到计划），不能再更改其 sourceAnchor 值。若要指定的 sourceAnchor 值指定内部部署 AD 对象，请配置其 msDS ConsistencyGuid 属性，然后导入到 Azure AD 连接。 
  
有关 SourceAnchor 和 ConsistencyGuid 的详细信息，请参阅以下： [Azure AD 连接： 设计概念](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

