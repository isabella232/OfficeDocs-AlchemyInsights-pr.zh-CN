---
title: 将域名称服务器更新为指向 Microsoft
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: d9d66e366db14840a86b681deba78b89ddff5e068a3b931c88e493d2ec791b10
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54073590"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a>将域名称服务器更新为指向 Microsoft

注意：名称服务器更改有时候需要长达 48 小时才能进行传播。
  
若要使用 Microsoft 设置域，需要更新注册机构中的名称服务器。 创建或编辑域注册机构中的名称服务器记录。
  
1. 转到域注册机构的网站，查找可在其中编辑名称服务器的区域。

2. 创建或编辑两个名称服务器记录，匹配以下值：

  - ns1.bdm.microsoftonline.com

  - ns2.bdm.microsoftonline.com

3. 保存更改。

您还可以找到本文中的详细说明：[更改名称服务器以设置Microsoft 365注册机构的名称](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)
  