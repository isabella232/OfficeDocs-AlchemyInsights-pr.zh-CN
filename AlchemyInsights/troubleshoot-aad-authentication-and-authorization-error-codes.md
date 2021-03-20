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
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a><span data-ttu-id="bb832-102">Azure AD 身份验证和授权 （AADSTS） 错误代码疑难解答</span><span class="sxs-lookup"><span data-stu-id="bb832-102">Troubleshoot Azure AD Authentication and Authorization (AADSTS) error codes</span></span>

<span data-ttu-id="bb832-103">要解决 AAD 身份验证和授权错误代码 （AADSTS），请执行以下建议步骤：</span><span class="sxs-lookup"><span data-stu-id="bb832-103">To resolve AAD authentication and authorization error codes (AADSTS), perform the following recommended steps:</span></span>

1. <span data-ttu-id="bb832-104">**处理应用程序中的错误代码**</span><span class="sxs-lookup"><span data-stu-id="bb832-104">**Handling error codes in your application**</span></span>

- <span data-ttu-id="bb832-105">**OAuth2.0 规范**， https://tools.ietf.org/html/rfc6749#section-5.2 提供了有关如何使用错误响应的错误部分来处理身份验证过程中的错误的指南。</span><span class="sxs-lookup"><span data-stu-id="bb832-105">The **OAuth2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2, provides guidance on how to handle errors during authentication using the error portion of the error response.</span></span>

    - <span data-ttu-id="bb832-106">**错误**：错误代码字符串，可用于对发生的错误类型进行分类，应将其用于对错误做出反应。</span><span class="sxs-lookup"><span data-stu-id="bb832-106">**error**: An error code string that can be used to classify types of errors that occur, and should be used to react to errors.</span></span>
    - <span data-ttu-id="bb832-107">当前 **错误** 字段有几个可能的值 - 查看协议文档链接和 OAuth 2.0 规范，了解有关特定错误及如何响应这些错误的更多信息。</span><span class="sxs-lookup"><span data-stu-id="bb832-107">The **error** field has several possible values - review the protocol documentation links and OAuth 2.0 specs for more information about specific errors and how to react to them.</span></span>

- <span data-ttu-id="bb832-108">以下是错误响应示例：</span><span class="sxs-lookup"><span data-stu-id="bb832-108">Here is a sample error response:</span></span>
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
2. <span data-ttu-id="bb832-109">**查找当前错误代码信息**</span><span class="sxs-lookup"><span data-stu-id="bb832-109">**Lookup current error code information**</span></span>

- <span data-ttu-id="bb832-110">错误代码和消息可能会有变化。</span><span class="sxs-lookup"><span data-stu-id="bb832-110">Error codes and messages are subject to change.</span></span> <span data-ttu-id="bb832-111">有关最新信息，请参阅 https://login.microsoftonline.com/error 页面，查找 AADSTS 错误说明、修补程序和一些建议的解决方法。</span><span class="sxs-lookup"><span data-stu-id="bb832-111">For the most current information, see the https://login.microsoftonline.com/error page to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>
- <span data-ttu-id="bb832-112">还可搜索和解决文章[身份验证和授权错误代码](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application)中列出的 [AADSTS错误代码](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes)。</span><span class="sxs-lookup"><span data-stu-id="bb832-112">You can also search for and troubleshoot [AADSTS error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listed in the article [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span></span>

3. <span data-ttu-id="bb832-113">**获取帮助**</span><span class="sxs-lookup"><span data-stu-id="bb832-113">**Get Help**</span></span>

- <span data-ttu-id="bb832-114">[开发人员支持与帮助](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - 如果需要一个问题的答案或帮助解决我们的文档中没有涉及的问题，可能需要与专家联系以寻求帮助。</span><span class="sxs-lookup"><span data-stu-id="bb832-114">[Support and help options for developers](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - If you need an answer to a question or help in solving a problem not covered in our documentation, it might be time to reach out to experts for help.</span></span> <span data-ttu-id="bb832-115">本文提供有关在开发与 Microsoft 身份平台集成的应用时获取问题的答案的一些建议。</span><span class="sxs-lookup"><span data-stu-id="bb832-115">This article provides several suggestions for getting answers to your questions as you develop apps that integrate with the Microsoft identity platform.</span></span>








