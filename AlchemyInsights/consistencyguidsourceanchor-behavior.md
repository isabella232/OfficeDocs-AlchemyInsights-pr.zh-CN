---
title: ConsistencyGuid/sourceAnchor 行为
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 8527e7c2404742a999041f85ed12d78c48cc0d8c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705723"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="ee255-102">ConsistencyGuid/sourceAnchor 行为</span><span class="sxs-lookup"><span data-stu-id="ee255-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="ee255-103">Azure AD Connect （版本1.1.524.0 和之后）现在有利于将 ConsistencyGuid 用作 sourceAnchor 属性。</span><span class="sxs-lookup"><span data-stu-id="ee255-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="ee255-104">使用此功能时，Azure AD Connect 会自动将同步规则配置为：</span><span class="sxs-lookup"><span data-stu-id="ee255-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="ee255-105">使用 ConsistencyGuid 作为 User 对象的 sourceAnchor 属性。</span><span class="sxs-lookup"><span data-stu-id="ee255-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="ee255-106">ObjectGUID 用于其他对象类型。</span><span class="sxs-lookup"><span data-stu-id="ee255-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="ee255-107">对于任何给定的本地 AD 用户对象，其 ConsistencyGuid 属性未填充，Azure AD Connect 将其 objectGUID 值写入本地 Active Directory 中的 ConsistencyGuid 属性。</span><span class="sxs-lookup"><span data-stu-id="ee255-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="ee255-108">在填充 ConsistencyGuid 属性后，Azure AD Connect 然后将该对象导出到 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="ee255-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="ee255-109">**注意：** 将本地 AD 对象导入到 Azure AD Connect （即，导入到 AD 连接器空间并投影到元节）后，将无法再更改它的 sourceAnchor 值。</span><span class="sxs-lookup"><span data-stu-id="ee255-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="ee255-110">若要指定给定内部部署 AD 对象的 sourceAnchor 值，请先配置其 ConsistencyGuid 属性，然后再将其导入到 Azure AD Connect。</span><span class="sxs-lookup"><span data-stu-id="ee255-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="ee255-111">有关 SourceAnchor 和 ConsistencyGuid 的详细信息，请参阅以下内容： [AZURE AD Connect：设计概念](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="ee255-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

