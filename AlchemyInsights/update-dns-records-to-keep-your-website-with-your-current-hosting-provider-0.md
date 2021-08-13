---
title: 更新 DNS 记录以便利用当前的托管提供商继续托管网站
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: f868ce25d68f61da30d2db4de88aa83675c97857b3c1371cf2039e0b03895a64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007672"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>更新 DNS 记录以便利用当前的托管提供商继续托管网站

1. 在Microsoft 365 管理中心中，转到"设置域"页面，在域列表中，选择用于  >  [](https://admin.microsoft.com/Adminportal#/Domains)网站的域。

2. 选择" **+ 新增自定义记录** "，然后输入以下信息：

  - 对于" **DNS 类型** "，请输入： **A (地址)**

  - 对于" **主机名或别名** "，请键入： **@**

  - 对于" **IP 地址** "，请键入网站当前托管位置的静态 IP 地址（例如 172.16.140.1）。

    必须是该网站的 *静态*  IP 地址，不能是  *动态*  IP 地址。 请与您的网站的托管网站核实，确保可以获得您的公共网站的静态 IP 地址。

3. 选择" **保存** "。

此外，您可以创建 CNAME 记录以帮助客户找到您的网站。
  
1. 选择" **+ 新增自定义记录** "，然后输入以下信息：

  - 对于" **DNS 类型** "，请输入： **CNAME (别名)**

  - 对于" **主机名或别名** "，请键入： **www**

  - 对于" **指向地址** "，请键入网站的完全限定域名 (FQDN)，例如 contoso.com。

2. 选择“保存”。
