---
title: 使用身份验证库
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897428"
---
# <a name="working-with-authentication-libraries"></a>使用身份验证库

如果要解决 Microsoft 身份验证库 (MSAL) 问题，请执行以下建议步骤:

1. **使用 MSAL**: [Microsoft 标识平台身份验证库](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - 本文介绍了 Microsoft.认证库对几种应用类型的支持。 它包括指向库源代码的链接、从哪里获取应用项目的程序包、以及库是否支持用户登录(身份验证)、访问受保护的 Web API (授权)，或者两者都支持。

2. **Troubleshoot Authentication**: MSAL 支持多种身份验证流程，用于不同的应用场景。 根据客户应用程序的构建方式，MSAL 可以使用 Microsoft 标识平台支持的一种或多种认证流。 这些流程可以产生几种类型的令牌和授权码，并需要不同的令牌来使其发挥作用。

3. **访问令牌**: [Microsoft 身份平台访问令牌](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - 了解 API 如何验证和使用访问令牌中的声明。 本文中除记录外的所有文档都仅适用于已注册的 API 所发布的令牌。 此令牌不适用于为 Microsoft 拥有的 API 发布的令牌，也不能用这些令牌来验证 Microsoft 标识平台将如何为所创建的 API 发布令牌。

**结束对 Azure Active Directory 身份验证库 (ADAL) 的支持**

- **自 2020 年 6 月 30 日起，** 我们将不再为 ADAL 和 Azure AD Graph 添加任何新功能。 我们将继续提供技术支持和安全更新，但不再提供功能更新。
- **自 2022 年 6 月 30 日起，** 我们将终止对 Azure AD Graph 的支持，并且将不再提供技术支持或安全更新。
- 此时间之后，在现有 OS 版本上使用 ADAL 的应用将继续工作，但将不会 *获得任何技术支持或安全更新*。
- 此后，使用 Azure AD Graph 的应用可能不再接收来自 Azure AD Graph 端点的响应。

**ADAL 迁移**

- 我们建议更新到 MSAL，其具有最新的功能和安全更新。
- 如果使用 Microsoft 应用，请了解 Microsoft 正在支持在结束最后期限之前将其应用程序迁移到 MSAL，以确保它们将受益于 MSAL 持续的安全性和功能改进。

1. [请阅读 ADAL 常见问题解答](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)。
2. [了解如何在不同平台上迁移应用](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance)。
3. 如果在阅读完应用平台的指南后还有其他问题，可以在 [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html)上以 [azure-ad-adal-deprecation] 为标签发帖，或者在库的 GitHub 储存库中开一个问题。 请参阅 **MSAL 概述** 文章中的[语言和框架](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks)部分，以获取每个库的报告链接。
4. **如果需要帮助了解哪些应用程序使用 ADAL**，我们建议查看所有应用程序的源代码。 如果适用，请联系任何独立软件供应程序 (ISV) 或应用程序供应程序。 Microsoft 支持部门也可提供租户内所有非 Microsoft ADAL 应用的列表。







