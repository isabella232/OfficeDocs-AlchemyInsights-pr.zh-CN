---
title: 使用 AIP 客户端自动分类行为异常
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
- "4373"
ms.openlocfilehash: d7a2246d78cbd6c4ab40c2a4e5a21807933b619a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715191"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>使用 AIP 客户端自动分类行为异常

自动分类行为异常时，使用下列推荐的指南：

1. 如果使用自动标记时遇到问题，请参阅[如何为 Azure 信息保护配置自动分类和推荐分类条件](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)和[敏感信息类型查找的内容](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)。
2. 检查是否使用了配置不正确的作用域内策略：[如何通过使用作用域内策略为特定用户配置 Azure 信息保护策略](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)。
3. 如果附加标记文档时，Outlook 无法使用自动标记，验证未按下列说明定义 `DRMEncryptProperty`：[针对安全的 IRM 注册表设置](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)。
4. 如果将[内置信息类型](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b)用于 Azure 信息保护策略，请验证内容是否与预期格式匹配。
5. 验证标签是否已针对**自动**或**推荐**进行了相应配置。 （**自动**标记可用于所有 Microsoft 365 应用程序，而**推荐**可用于除 Outlook 之外的所有 Microsoft 365 应用程序。）
6. 不可对之前已手动标记或者之前已自动标记有更高级分类的文档和电子邮件使用自动分类。  有关详细信息，请参阅：[如何应用自动标签或建议标签](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied)。
7. 如果仍遇到问题，请收集 Azure 信息保护客户端日志，并将导出的日志附加到支持票证。 导出 Azure 信息保护日志：
    - 在 Outlook 中打开 Office 文档或新建电子邮件。
    - 单击“**保护/敏感度**” > “**帮助和反馈**。
    - 单击“**导出日志**”。
    - 将日志保存到选定位置，并将其附加到服务请求中。

有关详细信息，请参阅：

- [如何为 Azure 信息保护配置自动分类和推荐分类条件](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [有关使用 Azure 信息保护常见方案的操作指南](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [查阅 Azure 信息保护文档](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [查阅 Azure 信息保护订阅和功能](https://azure.microsoft.com/pricing/details/information-protection)
- [Azure 信息保护要求](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Azure 信息保护快速入门教程](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [下载 Azure 信息保护客户端](https://www.microsoft.com/download/details.aspx?id=53018)
