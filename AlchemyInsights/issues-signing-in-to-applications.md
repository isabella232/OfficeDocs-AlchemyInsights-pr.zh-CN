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
# <a name="issues-signing-in-to-applications"></a><span data-ttu-id="37252-102">登陆应用的问题</span><span class="sxs-lookup"><span data-stu-id="37252-102">Issues signing in to applications</span></span>

<span data-ttu-id="37252-103">要检测和用户登录问题有关的原因或诊断，请执行下列步骤：</span><span class="sxs-lookup"><span data-stu-id="37252-103">To detect the cause or diagnose problems related to user sign-in, perform the following steps:</span></span>

1. <span data-ttu-id="37252-104">启动[登陆诊断](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)。</span><span class="sxs-lookup"><span data-stu-id="37252-104">Launch the [Sign-in Diagnostic](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
2. <span data-ttu-id="37252-105">通过输入你具有的关于用户、应用、登陆时间、请求 ID 或相关 ID 的详细信息，来找到要分析的事件。</span><span class="sxs-lookup"><span data-stu-id="37252-105">Find the event to analyze by entering the details you have about the user, application, time of sign in, request Id, or correlation Id.</span></span>
3. <span data-ttu-id="37252-106">查看诊断结果，它会详细显示发生的问题以及可以采取的措施，如果需要措施的话。</span><span class="sxs-lookup"><span data-stu-id="37252-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="37252-107">下列是一些关于登陆应用常见的问题：</span><span class="sxs-lookup"><span data-stu-id="37252-107">The following are some common issues you may experience when signing in to applications:</span></span>

1. <span data-ttu-id="37252-108">你或用户 **已经完成 Azure AD 登陆，但是看到了意外的提示** - 阅读文章[登陆到应用时出现意外的同意提示](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)和[为应用执行同意时出现意外的错误](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)。</span><span class="sxs-lookup"><span data-stu-id="37252-108">You or the user **has complete an Azure AD sign in, but are seeing an unexpected prompt** - See the articles [Unexpected consent prompt when signing in to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) and [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>
2. <span data-ttu-id="37252-109">你或用户 **已经直接登陆应用，但是无法通过自定义门户的深层链接或访问面板登陆**：请参阅[从 Azure AD 我的应用登陆到应用的相关问题疑难解答](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)。</span><span class="sxs-lookup"><span data-stu-id="37252-109">You or a user **has signed in to an application directly, but can't sign in to it from a deeplink on the custom portal or the access panel**: See [Troubleshoot problems signing in to an application from Azure AD My Apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).</span></span>
3. <span data-ttu-id="37252-110">你或用户 **已经完成 Azure AD 登陆，但是应用显示了错误消息且用户无法完成登陆登陆流程**：问题的原因是应用不接受 Azure AD 发送的响应。</span><span class="sxs-lookup"><span data-stu-id="37252-110">You or a user **has completed an Azure AD sign in, but the application displays an error message and doesn't let the user finish the sign-in flow**: The problem is that the app didn't accept the response that Azure AD issued.</span></span> <span data-ttu-id="37252-111">按照[以下步骤](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error)开始故障排除。</span><span class="sxs-lookup"><span data-stu-id="37252-111">Follow [these steps](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) to troubleshoot.</span></span>
4. <span data-ttu-id="37252-112">你或用户 **无法登陆以密码单一登陆配置的非库应用**：按照[以下步骤](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)的指引进行故障排除。</span><span class="sxs-lookup"><span data-stu-id="37252-112">You or a user **can’t sign in to a non-gallery application configured for password single sign-on**: Follow the guidance in [these steps](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) to troubleshoot.</span></span>
5. <span data-ttu-id="37252-113">你或用户 **无法登陆以密码单一登陆配置的 Azure AD 库应用**：按照[以下步骤](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)的指引进行故障排除。</span><span class="sxs-lookup"><span data-stu-id="37252-113">You or a user **can’t sign in to an Azure AD Gallery application configured for password single sign-on**: Follow [these steps](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) to troubleshoot.</span></span>
6. <span data-ttu-id="37252-114">你或用户 **无法登陆到 Microsoft 应用**：按照[这些步骤](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)进行故障排除。</span><span class="sxs-lookup"><span data-stu-id="37252-114">You or a user **can't sign in to a Microsoft application**: Follow [these steps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) to troubleshoot.</span></span>
7. <span data-ttu-id="37252-115">你或用户 **无法登陆以联合单一登陆配置的非库应用**：按照[以下步骤](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery)的指引进行故障排除。</span><span class="sxs-lookup"><span data-stu-id="37252-115">You or a user **can't sign in to a non-gallery application configured for federated single sign-on**: Follow [these steps](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) to troubleshoot.</span></span>
8. <span data-ttu-id="37252-116">你或用户 **无法登陆以联合密码单一登陆配置的 Azure AD 库应用**：按照[以下步骤](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)的指引进行故障排除。</span><span class="sxs-lookup"><span data-stu-id="37252-116">You or a user **can't sign in to an Azure AD Gallery application configured for federated single sign-on**: Follow [these steps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) to troubleshoot.</span></span>
9. <span data-ttu-id="37252-117">你或用户 **无法登陆到自定义开发的应用**：按照[这些步骤](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)进行故障排除。</span><span class="sxs-lookup"><span data-stu-id="37252-117">You or a user **can't sign in to a custom-developed application**: Follow [these steps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) to troubleshoot.</span></span>
10. <span data-ttu-id="37252-118">你或用户 **无法登陆到使用 Azure AD 应用程序代理的本地应用**：按照[这些步骤](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy)进行故障排除。</span><span class="sxs-lookup"><span data-stu-id="37252-118">You or a user **can't sign in to an on-premises application using the Azure AD application proxy**: Follow [these steps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) to troubleshoot.</span></span>

