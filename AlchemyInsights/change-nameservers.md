---
title: 更改名称服务器
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 572f8befd84f55cb07a3535852a46e735d3ed620
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706745"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a>将域名称服务器更新为指向 Microsoft

注意：名称服务器更改有时候需要长达 48 小时才能进行传播。
  
若要在 Microsoft 365 中设置域，需要更新注册机构处的名称服务器。创建或编辑域注册机构处的名称服务器记录。
  
1. 转到域注册机构的网站，查找可在其中编辑名称服务器的区域。
  
2. 创建或编辑两个名称服务器记录，匹配以下值：

  - ns1.bdm.microsoftonline.com

  - ns2.bdm.microsoftonline.com

3. 保存更改。

还可以在下面这篇文章中查找详细说明：[通过任意域注册机构更改名称服务器](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)
  