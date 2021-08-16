---
title: DLP 可能需要自定义类型
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1b0beb89eaf8a4105659a1faa7cc723174a73940ef46bd2355bdddfee7b94adb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030784"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP 可能需要自定义类型

**重要信息：** 在这段前所未有的时期，我们正在采取措施确保 SharePoint Online 和 OneDrive 服务高度可用，请访问 [SharePoint Online 临时功能调整](https://aka.ms/ODSPAdjustments)，获取详细信息。

**DLP 可能需要自定义信息类型**

借助 DLP 策略 (数据丢失) ，您可以识别和保护您组织的敏感数据。 在某些情况下，可能需要创建自己的自定义敏感信息类型来保护组织的数据。 

例如，您的组织可能需要以特定于组织的某种格式标识和保护员工标识或其他数据。如果是，请参阅以下文章了解详细信息。
  
 **自定义内置敏感信息类型**
  
如果只需做一些调整，内置敏感信息类型就可以满足您的需求，可以自定义 [内置敏感信息类型](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)。 例如，可以添加或删除关键字，也可以添加或删除支持性证据，如日期或地址。
  
 **创建自定义敏感信息类型**
  
但是，如果需要完全标识和保护不同类型的敏感信息，可以在安全与合规中心的 UI 中创建自定义[](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)&类型。
  
**使用安全与合规中心 PowerShell 创建自定义敏感信息类型**

最后，如果 UI 未提供所需的全部选项，可以在安全与合规中心 [PowerShell &敏感信息类型](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)。 从 XML 文件开始，可以使用每个可用的选项。
