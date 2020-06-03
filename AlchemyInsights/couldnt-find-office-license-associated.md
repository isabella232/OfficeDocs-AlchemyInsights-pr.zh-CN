---
title: 修复 Office 应用程序找不到 office 许可证关联的邮件
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 887be4bee2bd1562bdc3b29783e9deafe47d8d57
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505857"
---
# <a name="fixing-the-office-apps-couldnt-find-office-licenses-associated-message"></a>修复 Office 应用程序 "找不到与 office 许可证关联的信息" 消息

如果您收到此消息，请尝试以下操作：

1. 检查防火墙、防病毒软件和代理设置以确认他们不会阻止对 Office 应用程序的 Internet 访问。 请参阅[Microsoft 365 url 和 IP 地址范围](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)。
2. 删除并重新分配受影响的用户[的 Office 许可证](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)。 
3. 打开 Office[应用并注销](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)任何现有的用户帐户。
4. 转到 Windows 设置 >**帐户**  >  **电子邮件 & 帐户**，并删除除受影响帐户之外的所有工作帐户。
5. 转到 Windows 设置 >**帐户**  >  **访问工作或学校**，并断开除受影响帐户之外的所有工作帐户。
6. 重置 Office 激活状态。 [了解如何](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)操作。
7. 使用受影响的用户帐户[登录](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)。

有关其他故障排除解决方案，请参阅[Office 中的无许可证产品和激活错误](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)。