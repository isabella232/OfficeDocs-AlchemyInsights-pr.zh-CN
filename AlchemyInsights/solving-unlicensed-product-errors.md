---
title: 解决未授权的产品错误
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
- "3412"
- "9001428"
ms.openlocfilehash: 7922a2c5306f9d16856502b5e57e585cb90f2f7c9abaad0366f72ed46de786d5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957090"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>解决"未授权产品"错误的建议

若要解决有关"未授权产品"的错误，请尝试以下操作：

- 检查订阅状态是否已过期。
- 确保你拥有允许客户端许可证的订阅，Microsoft 365 商业应用版或商业高级版，并确保用户[分配有许可证](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)。 
- 确保用户使用分配了许可证Office帐户登录登录。
- 检查 ["服务运行状况"](https://docs.microsoft.com/office365/enterprise/view-service-health) 页以查看服务是否存在任何已知问题。
- 请检查防火墙、防病毒软件和代理设置，确认它们不会阻止Microsoft 365访问 Internet。 请参阅 [URL 和 IP 地址范围](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)。

您还可以尝试以下疑难解答操作： 

- 打开Office 应用[并注销](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)任何现有用户帐户。 [删除](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users)[并重新分配](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)Office许可证，然后使用受影响的用户帐户[Office登录该](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)许可证。
- 运行 [激活疑难解答程序](https://aka.ms/SARA-OfficeActivation-Alchemy)。
- [重置 Office 激活状态](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)。 
- [执行联机修复Office。](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b)

有关其他故障排除解决方案，请参阅： 

- [Office 中未经授权产品和激活错误](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [激活 Office 时出现错误“很抱歉，无法连接到你的帐户。请稍后重试”](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)