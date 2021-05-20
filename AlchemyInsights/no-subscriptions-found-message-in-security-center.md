---
title: 安全中心未找到订阅消息
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544098"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="606ef-102">安全中心未找到订阅消息</span><span class="sxs-lookup"><span data-stu-id="606ef-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="606ef-103">如果在访问 Microsoft Defender 安全中心时收到“未找到订阅”的消息，那么说明用户用来登录到门户的 Azure Active Directory (AAD) 没有Microsoft Defender ATP 许可证。</span><span class="sxs-lookup"><span data-stu-id="606ef-103">If while accessing Microsoft Defender Security Center you get a "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="606ef-104">Windows E5 和 Office E5 许可证是分开的。</span><span class="sxs-lookup"><span data-stu-id="606ef-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="606ef-p101">如果购买了许可证但是未配置到此 AAD 实例，请发起技术支持案例。以下的一项适用于你：</span><span class="sxs-lookup"><span data-stu-id="606ef-p101">Open a support case if the license was purchased but not provisioned to this AAD instance. Either you have:</span></span> <br/>
-   <span data-ttu-id="606ef-107">可能存在许可证配置问题。</span><span class="sxs-lookup"><span data-stu-id="606ef-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="606ef-108">你无意间将许可证配置到了用来验证此服务之外的 Microsoft AAD。</span><span class="sxs-lookup"><span data-stu-id="606ef-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>