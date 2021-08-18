---
title: 终结点 DLP 未部署到用户的设备
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: fa0e2766e1526d8e81cb247029e7c0fd98630b96
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316808"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>终结点 DLP 未部署到用户的设备

如果终结点数据丢失防护 (DLP) 设置尚未应用于用户的设备，请确认你满足以下要求：

- Windows 10 x64 内部版本 1809 或更高版本已安装在设备上。
- 反恶意软件客户端版本 4.18.2009.7 或更高版本已安装。
- 设备满足以下条件 **之一**：
    
    - 已建立 Azure Active Directory (Azure AD) 联接
    - 已建立混合 Azure AD 联接
    - 已完成 AAD 注册

- 若要执行策略操作，请确保终结点设备上已安装 Microsoft Chromium Edge 浏览器。

有关部署终结点 DLP 的其他要求，请参阅[终结点数据丢失防护入门](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)。