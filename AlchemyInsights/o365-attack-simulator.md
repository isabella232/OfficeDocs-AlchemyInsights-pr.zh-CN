---
title: Office 365 中的2681攻击模拟器
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305322"
---
# <a name="attack-simulator-in-office-365"></a><span data-ttu-id="7e200-102">Office 365 中的攻击模拟器</span><span class="sxs-lookup"><span data-stu-id="7e200-102">Attack Simulator in Office 365</span></span>

- <span data-ttu-id="7e200-103">是否缺少攻击模拟器？</span><span class="sxs-lookup"><span data-stu-id="7e200-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="7e200-104">攻击模拟器需要**Office 365 高级威胁防护计划2（ATP 计划2）** 或**Office 365 企业版 E5**。</span><span class="sxs-lookup"><span data-stu-id="7e200-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="7e200-105">在 Office 365 高级威胁防护计划1（ATP 计划1）、Office 365 企业版 E3 或任何 Office 365 商业版订阅中**不**包含攻击模拟器。</span><span class="sxs-lookup"><span data-stu-id="7e200-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Office 365 Business subscriptions.</span></span>

- <span data-ttu-id="7e200-106">用于启动模拟攻击的帐户需要全局管理员或安全管理员权限以及多重身份验证（MFA）。</span><span class="sxs-lookup"><span data-stu-id="7e200-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="7e200-107">有关攻击模拟器要求的详细信息，请参阅[本主题](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin)。</span><span class="sxs-lookup"><span data-stu-id="7e200-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="7e200-108">有关**强力密码**攻击模拟的重要须知：</span><span class="sxs-lookup"><span data-stu-id="7e200-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="7e200-109">如果目标帐户已启用 MFA 且密码被正确猜出，则该帐户不会显示为 "已损坏" （第二身份验证因素将不完整）。</span><span class="sxs-lookup"><span data-stu-id="7e200-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="7e200-110">密码文件不能大于 10 MB。</span><span class="sxs-lookup"><span data-stu-id="7e200-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="7e200-111">每行使用一个密码，并在列表中的最后一个密码后包含一个空行（回车）。</span><span class="sxs-lookup"><span data-stu-id="7e200-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="7e200-112">了解有关**Spear 的网络钓鱼**附加模拟的重要事项：</span><span class="sxs-lookup"><span data-stu-id="7e200-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="7e200-113">根据设计，不能为**网络钓鱼登录服务器 URL**提供自定义值。</span><span class="sxs-lookup"><span data-stu-id="7e200-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="7e200-114">如果收件人使用 "[启用报告邮件" 加载项](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in)将邮件报告为网络钓鱼，则您可能不会收到有关邮件的通知（因为这是一种模拟攻击）。</span><span class="sxs-lookup"><span data-stu-id="7e200-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="7e200-115">报告：在模拟的攻击完成之后，您可以单击 "**攻击详细信息**" 来查看报告。</span><span class="sxs-lookup"><span data-stu-id="7e200-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="7e200-116">有关攻击模拟器的详细说明和新功能，请参阅[Office 365 中的攻击模拟器](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)。</span><span class="sxs-lookup"><span data-stu-id="7e200-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
