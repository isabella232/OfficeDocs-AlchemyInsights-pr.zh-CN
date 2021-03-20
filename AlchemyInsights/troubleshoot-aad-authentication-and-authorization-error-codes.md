---
title: Azure AD 身份验证和授权 （AADSTS） 错误代码疑难解答
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897595"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>Azure AD 身份验证和授权 （AADSTS） 错误代码疑难解答

要解决 AAD 身份验证和授权错误代码 （AADSTS），请执行以下建议步骤：

1. **处理应用程序中的错误代码**

- **OAuth2.0 规范**， https://tools.ietf.org/html/rfc6749#section-5.2 提供了有关如何使用错误响应的错误部分来处理身份验证过程中的错误的指南。

    - **错误**：错误代码字符串，可用于对发生的错误类型进行分类，应将其用于对错误做出反应。
    - 当前 **错误** 字段有几个可能的值 - 查看协议文档链接和 OAuth 2.0 规范，了解有关特定错误及如何响应这些错误的更多信息。

- 以下是错误响应示例：
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **查找当前错误代码信息**

- 错误代码和消息可能会有变化。 有关最新信息，请参阅 https://login.microsoftonline.com/error 页面，查找 AADSTS 错误说明、修补程序和一些建议的解决方法。
- 还可搜索和解决文章[身份验证和授权错误代码](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application)中列出的 [AADSTS错误代码](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes)。

3. **获取帮助**

- [开发人员支持与帮助](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - 如果需要一个问题的答案或帮助解决我们的文档中没有涉及的问题，可能需要与专家联系以寻求帮助。 本文提供有关在开发与 Microsoft 身份平台集成的应用时获取问题的答案的一些建议。








