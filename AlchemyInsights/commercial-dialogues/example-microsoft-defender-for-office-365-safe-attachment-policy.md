---
title: Microsoft Defender for Office 365 安全附件策略示例
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735625"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="18b14-102">Microsoft Defender for Office 365 安全附件策略示例</span><span class="sxs-lookup"><span data-stu-id="18b14-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="18b14-103">这些设置启用名为 *"无延迟* "的策略，该策略可立即传递邮件，然后在扫描附件后重新附加附件：</span><span class="sxs-lookup"><span data-stu-id="18b14-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="18b14-104">**名称**：无延迟</span><span class="sxs-lookup"><span data-stu-id="18b14-104">**Name**: No delays</span></span>
- <span data-ttu-id="18b14-105">**说明**：立即传递邮件，在扫描后重新附加附件。</span><span class="sxs-lookup"><span data-stu-id="18b14-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="18b14-106">**响应**：选择 **"动态传递"** 选项。</span><span class="sxs-lookup"><span data-stu-id="18b14-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="18b14-107">有关详细信息，请参阅安全 [附件策略中的动态传递](https://go.microsoft.com/fwlink/?linkid=2092328)。</span><span class="sxs-lookup"><span data-stu-id="18b14-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="18b14-108">**重定向附件** 部分：选择" **启用** 重定向"选项，然后输入将调查恶意附件的 Microsoft 365 全局管理员、安全管理员或安全分析师的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="18b14-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="18b14-109">**"应用于** "部分： **选择"收件人域是**"，然后选择您的域。</span><span class="sxs-lookup"><span data-stu-id="18b14-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="18b14-110">选择 **"添加**"，然后选择"确定 **"。**</span><span class="sxs-lookup"><span data-stu-id="18b14-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="18b14-111">完成后，选择 **保存。**</span><span class="sxs-lookup"><span data-stu-id="18b14-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="18b14-112">若要了解更多信息，请参阅 [Microsoft Defender for Office 365 中的安全附件](https://go.microsoft.com/fwlink/?linkid=2092213)。</span><span class="sxs-lookup"><span data-stu-id="18b14-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>
