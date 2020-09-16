---
title: 解决未经许可的产品错误
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: bd2e8cb204edd7135fc34ef0d42ac8259434d37d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737943"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>解决 "未经许可的产品" 错误的建议

若要解决有关 "未经许可的产品" 的错误，请尝试以下操作：

- 检查以查看您的订阅状态是否已过期。
- 确保您具有允许客户端许可证（如 Microsoft 365 应用程序商业版或商业高级版）的订阅，并 [确保用户已分配许可证](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)。 
- 确保用户使用与已分配许可证的相同帐户登录 Office。
- 检查 " [服务运行状况" 页](https://docs.microsoft.com/office365/enterprise/view-service-health) 以查看该服务是否存在任何已知问题。
- 检查你的防火墙、防病毒软件和代理设置，以确认他们不会阻止 Microsoft 365 应用访问 Internet。 请参阅 [url 和 IP 地址范围](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)。

您也可以尝试以下故障排除操作： 

- 打开 Office [应用并注销](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) 任何现有的用户帐户。 [删除](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) 并 [重新分配](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) office 许可证，然后使用受影响的用户帐户 [登录 office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) 。
- 运行 [激活疑难解答](https://aka.ms/SARA-OfficeActivation-Alchemy)。
- [重置 Office 激活状态](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)。 
- [执行 Office 的联机修复](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b)。

有关其他故障排除解决方案，请参阅： 

- [Office 中未经授权产品和激活错误](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [激活 Office 时出现错误“很抱歉，无法连接到你的帐户。请稍后重试”](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)