---
title: 更改名称服务器
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 67680a6fa514d31ccb88cc8691a199cd1f58a402
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818602"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a>将域名称服务器更新为指向 Microsoft

注意：名称服务器更改有时候需要长达 48 小时才能进行传播。
  
若要在 Microsoft 365 中设置域，需要更新注册机构处的名称服务器。创建或编辑域注册机构处的名称服务器记录。
  
1. 转到域注册机构的网站，查找可在其中编辑名称服务器的区域。
  
2. 创建或编辑两个名称服务器记录，匹配以下值：

  - ns1.bdm.microsoftonline.com

  - ns2.bdm.microsoftonline.com

3. 保存更改。

还可以在下面这篇文章中查找详细说明：[通过任意域注册机构更改名称服务器](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)
  