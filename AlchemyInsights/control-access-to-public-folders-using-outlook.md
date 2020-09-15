---
title: 使用Outlook控制对公共文件夹的访问
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 4ef62fe8c9cc438c48ed8897a8b3385b15669cdc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680482"
---
# <a name="control-access-to-public-folders-using-outlook"></a>使用Outlook控制对公共文件夹的访问

使用 Outlook 控制哪些用户可以访问公用文件夹，请执行以下操作：

1. 使用 `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true：允许用户在 Outlook 中访问公用文件夹  
$false：防止用户在Outlook 中访问公用文件夹。 此值为默认值。  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

注意：此过程仅可控制与 Windows 客户端的 Outlook 桌面版的连接。 用户可以使用 OWA 或 Outlook for Mac 继续访问公用文件夹。

如需了解更多信息，请参阅 [ Outlook 中对公用文件夹的受控连接](https://aka.ms/controlpf)。
