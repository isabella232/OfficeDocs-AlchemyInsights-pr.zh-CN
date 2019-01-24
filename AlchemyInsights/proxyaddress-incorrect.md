---
title: 不正确的 ProxyAddress
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
ms.assetid: c4cea778-1b26-4aea-bde8-4b7605e35886
ms.openlocfilehash: 0d7282473822a7c6bad06a1c1d93dbd6f391404b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29459138"
---
# <a name="proxyaddress-incorrect"></a><span data-ttu-id="5aace-102">不正确的 ProxyAddress</span><span class="sxs-lookup"><span data-stu-id="5aace-102">ProxyAddress incorrect</span></span>

<span data-ttu-id="5aace-p101">当到 Azure AD 同步对象时，Active Directory 中在 proxyAddresses 属性中指定的值与 Azure AD 规则进行比较，并且在 Azure AD 然后填充 proxyAddresses 属性。因此，在 Active Directory 中的对象的 proxyAddresses 属性的值可能不在 proxyAddresses 属性的值相同 Azure AD 中。</span><span class="sxs-lookup"><span data-stu-id="5aace-p101">When an object is synchronized to Azure AD, the values that are specified in the proxyAddresses attribute in Active Directory are compared with Azure AD rules, and then the proxyAddresses attribute is populated in Azure AD. Therefore, the values of the proxyAddresses attribute for the object in Active Directory may not be the same as the values of the proxyAddresses attribute in Azure AD.</span></span>
  
<span data-ttu-id="5aace-105">若要了解有关 proxyaddress 的填充方式的详细信息，请参阅[如何在 Azure AD 中填充的 proxyAddress 属性](https://support.microsoft.com/en-us/help/3190357/how-the-proxyaddresses-attribute-is-populated-in-azure-ad)。</span><span class="sxs-lookup"><span data-stu-id="5aace-105">To learn more about how the proxyaddress is populated, see [How the proxyAddress attribute is populated in Azure AD](https://support.microsoft.com/en-us/help/3190357/how-the-proxyaddresses-attribute-is-populated-in-azure-ad).</span></span>
  

