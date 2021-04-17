---
title: 修复 Microsoft 365 应用 找不到 Office 许可证关联消息
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
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816478"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>修复 Microsoft 365 应用"找不到关联的 Office 许可证"消息

如果收到此消息，请尝试执行以下操作：

1. 请检查防火墙、防病毒软件和代理设置，确认它们不会阻止 Internet 访问 Microsoft 365 应用。 请参阅 [Microsoft 365 URL 和 IP 地址范围](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)。
2. 删除 [并重新分配受影响的用户的 Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) 许可证。 
3. 打开 Office 应用 [并注销](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) 任何现有用户帐户。
4. 转到 Windows 设置>帐户  >  **电子邮件&帐户，** 并删除所有工作帐户（受影响帐户除外）。
5. 转到 Windows 设置>**访问** 工作或学校帐户，并断开所有工作  >  帐户（受影响帐户除外）。
6. 重置 Office 激活状态。 [了解如何。](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)
7. [使用受影响的](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) 用户帐户登录。

有关其他疑难解答解决方案，请参阅 Office 中的未授权产品和 [激活错误](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)。