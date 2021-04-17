---
title: 使用Outlook控制对公共文件夹的访问
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816730"
---
# <a name="control-access-to-public-folders-using-outlook"></a>使用Outlook控制对公共文件夹的访问

使用 Outlook 控制哪些用户可以访问公用文件夹，请执行以下操作：

1. 使用 `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true：允许用户在 Outlook 中访问公用文件夹  
$false：防止用户在Outlook 中访问公用文件夹。 此值为默认值。  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

注意：此过程仅可控制与 Windows 客户端的 Outlook 桌面版的连接。 用户可以使用 OWA 或 Outlook for Mac 继续访问公用文件夹。

如需了解更多信息，请参阅 [ Outlook 中对公用文件夹的受控连接](https://aka.ms/controlpf)。
