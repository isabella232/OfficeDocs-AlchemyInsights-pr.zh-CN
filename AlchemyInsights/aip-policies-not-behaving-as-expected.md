---
title: AIP：策略未按预期运行
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
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663179"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP：策略未按预期运行

Azure 信息保护：策略未按预期运行，有关各种策略问题的建议准则，请参阅以下内容：

1. 如果你在视觉标记方面遇到问题，请查看[应用视觉标记时](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)。
2. 如果使用自动标记时遇到问题，请查看[如何为 Azure 信息保护配置自动分类和推荐分类条件](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)和[敏感信息类型查找的内容](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)。
3. 如果你在本机/配置文件保护方面遇到问题，请查看[文件 API 配置](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)。
4. 检查是否使用了配置不正确的作用域内策略：[如何通过使用作用域内策略为特定用户配置 Azure 信息保护策略](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)。
5. 如果附加标记文档时，Outlook 无法使用自动标记，验证是否未按下列说明定义 DRMEncryptProperty：[针对安全的 IRM 注册表设置](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)。

如果仍遇到问题，请收集 Azure 信息保护客户端日志，并将导出的日志附加到此票证。

1. 在 Outlook 中打开 Office 文档或新建电子邮件。
2. 单击“**保护/敏感度**” > “**帮助和反馈**。
3. 单击“**导出日志**”。
4. 将日志保存到选定位置，并将其附加到此服务请求中。

其他资源：

- [如何为 Azure 信息保护配置用于视觉标记的标签](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [查阅 Azure 信息保护文档](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [在 Microsoft 365 应用中使用敏感度标签](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

