---
title: 修复Microsoft 365应用程序找不到 Office 许可证关联消息
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
ms.openlocfilehash: a65610dc5f88eeb4195e48131f08940758d0dfac0710502e0e15ab5f661c5719
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069594"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>修复Microsoft 365"找不到关联的 Office 许可证"的消息

如果收到此消息，请尝试执行以下操作：

1. 请检查防火墙、防病毒软件和代理设置，以确认它们不会阻止 Internet 访问 Microsoft 365应用。 请参阅[Microsoft 365 URL 和 IP 地址范围](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)。
2. 删除[并重新分配Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)的用户的许可证。 
3. 打开Office 应用[并注销](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)任何现有用户帐户。
4. 转到"Windows 设置 >**帐户**  >  **""电子邮件&帐户"，** 并删除所有工作帐户（受影响帐户除外）。
5. 转到"Windows 设置 >访问  >  **工作或学校** 帐户"，断开所有工作帐户（受影响帐户除外）。
6. 重置 Office 激活状态。 [了解如何。](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)
7. [使用受影响的](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) 用户帐户登录。

有关其他疑难解答解决方案，请参阅未授权的产品和[激活错误Office。](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)