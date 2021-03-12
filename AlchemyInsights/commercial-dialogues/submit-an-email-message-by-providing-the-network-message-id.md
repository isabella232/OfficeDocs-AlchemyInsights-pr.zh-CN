---
title: 通过提供网络邮件 ID 提交电子邮件
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
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735549"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="8bbe4-102">通过提供网络邮件 ID 提交电子邮件</span><span class="sxs-lookup"><span data-stu-id="8bbe4-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="8bbe4-103">在"**新建提交"** 飞出内容中，选择 **"电子邮件** 和网络 **消息 ID"。**</span><span class="sxs-lookup"><span data-stu-id="8bbe4-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="8bbe4-104">按照以下步骤在 Outlook 中查找电子邮件的邮件 ID：</span><span class="sxs-lookup"><span data-stu-id="8bbe4-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="8bbe4-105">双击电子邮件以打开它。</span><span class="sxs-lookup"><span data-stu-id="8bbe4-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="8bbe4-106">选择 **"文件**  >  **属性"。**</span><span class="sxs-lookup"><span data-stu-id="8bbe4-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="8bbe4-107">打开记事本或空白 Word 文档，然后将 **"Internet** 标题"框中的内容复制并粘贴到打开的文档中，以更好地查看。</span><span class="sxs-lookup"><span data-stu-id="8bbe4-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="8bbe4-108">找到 **"X-MS-Exchange-Organization-Network-Message-Id"** 字段。</span><span class="sxs-lookup"><span data-stu-id="8bbe4-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="8bbe4-109">后的值 **是** 提交所需的 ID。</span><span class="sxs-lookup"><span data-stu-id="8bbe4-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="8bbe4-110">在 **"收件人"** 下，如果电子邮件已登陆到此电子邮件所有收件人的垃圾邮件文件夹，请选择"**全选"。**</span><span class="sxs-lookup"><span data-stu-id="8bbe4-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="8bbe4-111">如果没有，则仅选择报告问题的用户。</span><span class="sxs-lookup"><span data-stu-id="8bbe4-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="8bbe4-112">在 **"提交原因"** 下，如果选择 **"应** 已被阻止"，请指定邮件应被阻止为"垃圾邮件"、"网络钓鱼"还是"恶意软件"，然后选择"提交 **"。** </span><span class="sxs-lookup"><span data-stu-id="8bbe4-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="8bbe4-113">若要了解更多信息，请参阅如何将可疑的垃圾邮件、网络钓鱼、URL 和文件提交给 [Microsoft 进行扫描](https://go.microsoft.com/fwlink/?linkid=2101479)。</span><span class="sxs-lookup"><span data-stu-id="8bbe4-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
