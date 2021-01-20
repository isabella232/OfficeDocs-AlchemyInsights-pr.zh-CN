---
title: 登陆应用的问题
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886783"
---
# <a name="issues-signing-in-to-applications"></a>登陆应用的问题

要检测和用户登录问题有关的原因或诊断，请执行下列步骤：

1. 启动[登陆诊断](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)。
2. 通过输入你具有的关于用户、应用、登陆时间、请求 ID 或相关 ID 的详细信息，来找到要分析的事件。
3. 查看诊断结果，它会详细显示发生的问题以及可以采取的措施，如果需要措施的话。

下列是一些关于登陆应用常见的问题：

1. 你或用户 **已经完成 Azure AD 登陆，但是看到了意外的提示** - 阅读文章[登陆到应用时出现意外的同意提示](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)和[为应用执行同意时出现意外的错误](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)。
2. 你或用户 **已经直接登陆应用，但是无法通过自定义门户的深层链接或访问面板登陆**：请参阅[从 Azure AD 我的应用登陆到应用的相关问题疑难解答](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)。
3. 你或用户 **已经完成 Azure AD 登陆，但是应用显示了错误消息且用户无法完成登陆登陆流程**：问题的原因是应用不接受 Azure AD 发送的响应。 按照[以下步骤](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error)开始故障排除。
4. 你或用户 **无法登陆以密码单一登陆配置的非库应用**：按照[以下步骤](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)的指引进行故障排除。
5. 你或用户 **无法登陆以密码单一登陆配置的 Azure AD 库应用**：按照[以下步骤](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)的指引进行故障排除。
6. 你或用户 **无法登陆到 Microsoft 应用**：按照[这些步骤](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)进行故障排除。
7. 你或用户 **无法登陆以联合单一登陆配置的非库应用**：按照[以下步骤](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery)的指引进行故障排除。
8. 你或用户 **无法登陆以联合密码单一登陆配置的 Azure AD 库应用**：按照[以下步骤](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)的指引进行故障排除。
9. 你或用户 **无法登陆到自定义开发的应用**：按照[这些步骤](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)进行故障排除。
10. 你或用户 **无法登陆到使用 Azure AD 应用程序代理的本地应用**：按照[这些步骤](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy)进行故障排除。

