---
title: Teams 管理中心
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
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826369"
---
# <a name="teams-admin-center"></a>Teams 管理中心

了解如何通过 [Teams 管理中心](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center)管理 Teams。

如果无法访问 Teams 管理中心，请检查以下项：

- 验证是否已在任何外围设备（防火墙等）上或在本地计算机的防火墙规则中允许相应的 [Office 365 IP 地址和 URL](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service)。
- 验证用于访问 Teams 管理门户的登录名与 [Microsoft 365 管理门户](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)中列出的用户名是否匹配。

如果用户未出现在埃 Teams 管理中心，请检查以下项：

- 是否在最近 24 小时内创建了用户或分配了许可证？ 请确保在打开支持票证前等待至少 24 小时。
- 验证是否分配了适当的许可证？
- 如果你有一个本地 Active Directory，请确认 [本地 Active Directory 中 ProxyAddresses 字段中的 msRTCSIP-PrimaryUserAddress 或 SIP 地址的值是唯一的，并且格式匹配](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip：来自 [Microsoft 365 管理中心](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)中用户的 **用户名**。
- 如果你打算保留 Skype for Business Server 部署，并且让用户驻留在本地和联机：请按照 Skype for Business Server 控制面板中的“**使用 Teams 和 Skype for Business Online 设置混合**” ，并联机移动用户。
