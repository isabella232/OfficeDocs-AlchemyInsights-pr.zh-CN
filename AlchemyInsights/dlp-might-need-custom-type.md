---
title: DLP 可能需要自定义类型
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932648"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP 可能需要自定义类型

**重要说明**：许多 SharePoint Online 和 OneDrive 客户对在后台运行的服务运行关键业务应用程序。 其中包括内容迁移、数据丢失防护（DLP）和备份解决方案。 在这些前所未有的时间内，我们将采取措施，以确保在远程工作方案中，SharePoint Online 和 OneDrive 服务对依赖于该服务的用户保持高可用性和可靠性。

为支持此目标，我们已在工作日白天营业时对后台应用（迁移、DLP 和备份解决方案）实施了更严格的限制限制。 在这些情况中，您应认为这些应用程序的吞吐量非常有限。 但是，在夜间和周末的时间内，服务将准备好处理来自后台应用程序的较大数量的请求。

**DLP 可能需要自定义信息类型**

使用数据丢失防护（DLP）策略，可以识别和保护组织中的敏感数据。 在某些情况下，您可能需要创建自己的**自定义**敏感信息类型来保护组织的数据。

例如，您的组织可能需要以特定于您的组织的某种格式标识和保护员工 Id 或其他数据。如果是这样，请参阅以下文章以了解详细信息。
  
 **自定义内置敏感信息类型**
  
如果内置的敏感信息类型只满足几次调整，就能满足您的需求，则可以[自定义内置的敏感信息类型](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type)。 例如，您可以添加或删除关键字，或者添加或删除支持的证据，如日期或地址。
  
 **创建自定义敏感信息类型**
  
但是，如果您需要完全标识和保护不同类型的敏感信息，则可以在安全 & 合规性中心的 UI 中[创建自定义敏感信息类型](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)。
  
**使用安全与合规中心 PowerShell 创建自定义敏感信息类型**

最后，如果 UI 不提供您所需的所有选项，则可以[在 Security & 合规性中心 PowerShell 中创建自定义敏感信息类型](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell)。 从 XML 文件开始，可以使用每个可用的选项。
