---
title: 配置 MIM 同步服务
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430713"
---
# <a name="configure-mim-sync-service"></a><span data-ttu-id="327c9-102">配置 MIM 同步服务</span><span class="sxs-lookup"><span data-stu-id="327c9-102">Configure MIM Sync service</span></span>

<span data-ttu-id="327c9-103">Microsoft Identity Manager （MIM） 同步服务是 MIM 的一个组件。</span><span class="sxs-lookup"><span data-stu-id="327c9-103">Microsoft Identity Manager (MIM) Synchronization Service is a component of MIM.</span></span> <span data-ttu-id="327c9-104">它是一种集中式本地服务，为具有多个本地目录和数据库的组织存储和集成信息。</span><span class="sxs-lookup"><span data-stu-id="327c9-104">It is a centralized on-premises service that stores and integrates information for organizations that have multiple on-premises directories and databases.</span></span> <span data-ttu-id="327c9-105">如果在 MIM 的最近更新中解决了你的问题，或者该问题是在下节中所提及的其他问题之一，则可能在 MIM 同步后解决你的问题。</span><span class="sxs-lookup"><span data-stu-id="327c9-105">You may be able to resolve your problem with MIM Sync if the issue was addressed in a recent update to MIM or is one of the other issues mentioned in the below section.</span></span>

<span data-ttu-id="327c9-106">**建议的步骤**</span><span class="sxs-lookup"><span data-stu-id="327c9-106">**Recommended steps**</span></span>

1. <span data-ttu-id="327c9-107">确保使用的是 MIM 同步的最新更新，并检查 [MIM 同步发行说明](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) 以确定该问题是否已在更新中得到解决。</span><span class="sxs-lookup"><span data-stu-id="327c9-107">Ensure that you are using a recent update of MIM Sync and check the [MIM Sync release notes](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) to determine if the issue has been resolved in an update.</span></span>
2. <span data-ttu-id="327c9-108">如果问题出现在 Generic LDAP、Generic SQL、Lotus Domino 或 Web Services 连接器上，请确保使用的是最新更新的 [通用连接器](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)。</span><span class="sxs-lookup"><span data-stu-id="327c9-108">If the problem is with the Generic LDAP, Generic SQL, Lotus Domino or Web Services connector, ensure that you are using a recent update of the [generic connectors](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span></span>
3. <span data-ttu-id="327c9-109">如果 MIM 同步运行因错误而停止，请参阅 [运行错误代码](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) 表以确认潜在原因。</span><span class="sxs-lookup"><span data-stu-id="327c9-109">If an MIM Sync-run stops with an error, consult the table of [run error codes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) to determine the potential causes.</span></span>
4. <span data-ttu-id="327c9-110">如果运行停止时出现 **“extension-dll-exception”**，请单击这些字样打开 **“连接器空格对象属性”** 窗口，然后单击 **“堆叠跟踪...”** 更多关于根本原因的信息，如 [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx)中所述。</span><span class="sxs-lookup"><span data-stu-id="327c9-110">If the run stops with **extension-dll-exception**, then click on those words to open the **Connector Space Object properties** window, and click on **Stack Trace...** to see more information on the underlying cause, as described in [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span></span>
5. <span data-ttu-id="327c9-111">如果密码更改通知服务 (PCNS) 组件在密码同步期间事件日志中报告 **错误 6025** ，请查看 [PCNS 报告错误 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx) 的故障排除指南。</span><span class="sxs-lookup"><span data-stu-id="327c9-111">If the Password Change Notification Service (PCNS) component reports **error 6025** in the event log during password synchronization, check the guide for troubleshooting [PCNS reporting error 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span></span>
6. <span data-ttu-id="327c9-112">如果与 FIM 服务管理代理完全同步速度较慢，请检查TempDB 的 **自动增加** 设置，如 [解决完全同步速度慢或挂起故障](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx)中所述。</span><span class="sxs-lookup"><span data-stu-id="327c9-112">If full synchronization with the FIM Service Management Agent is slow, check the **auto grow** setting for TempDB, as described in [Troubleshooting slow or hanging full synchronization](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span></span>
7. <span data-ttu-id="327c9-113">如果在使用 FIM 服务管理代理时遇到停用服务器的错误，并出现 failed-creation-via-web-services，请参阅 [支持信息: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services)以了解原因概述。</span><span class="sxs-lookup"><span data-stu-id="327c9-113">If you are encountering an error of stopped-server with failed-creation-via-web-services using the FIM Service Management Agent, see [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for an overview of causes.</span></span>

