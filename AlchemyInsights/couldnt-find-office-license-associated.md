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
ms.openlocfilehash: 1820cdb83a1adf36b4e7d0898ecdf8097eb6f0f3
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627908"
---
# <a name="fixing-the-office-apps-couldnt-find-office-licenses-associated-message"></a>修复 Office 应用程序 "找不到与 office 许可证关联的信息" 消息

如果您收到此消息，请尝试以下操作：

1. 检查防火墙、防病毒软件和代理设置以确认他们不会阻止对 Office 应用程序的 Internet 访问。 请参阅[Office 365 url 和 IP 地址范围](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)。
2. 删除并重新分配受影响的用户[的 Office 许可证](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users)。 
3. 打开 Office[应用并注销](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)任何现有的用户帐户。
4. 转到 Windows 设置 >**帐户** > **电子邮件 & 帐户**，并删除除受影响帐户之外的所有工作帐户。
5. 转到 Windows 设置 >**帐户** > **访问工作或学校**，并断开除受影响帐户之外的所有工作帐户。
6. 重置 Office 激活状态。 [了解如何](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)操作。
7. 使用受影响的用户帐户[登录](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)。

有关其他故障排除解决方案，请参阅[Office 中的无许可证产品和激活错误](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)。