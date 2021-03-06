---
title: 将 ClientAccessServerEnabled 设置为 True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50509520"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="76f2c-102">将 ClientAccessServerEnabled 设置为 True</span><span class="sxs-lookup"><span data-stu-id="76f2c-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="76f2c-103">如果无法打开加密的电子邮件，而是看到 **rpmsg** 附件，请执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="76f2c-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="76f2c-104">连接到 Exchange Online PowerShell。</span><span class="sxs-lookup"><span data-stu-id="76f2c-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="76f2c-105">若要连接到 Exchange Online PowerShell，必须使用全局管理员或 Exchange 管理员帐户登录。</span><span class="sxs-lookup"><span data-stu-id="76f2c-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="76f2c-106">a.</span><span class="sxs-lookup"><span data-stu-id="76f2c-106">a.</span></span> <span data-ttu-id="76f2c-107">打开Windows PowerShell，然后运行以下命令： `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="76f2c-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="76f2c-108">b.</span><span class="sxs-lookup"><span data-stu-id="76f2c-108">b.</span></span> <span data-ttu-id="76f2c-109">在 **Windows PowerShell凭据请求** 对话框中，输入你的工作或学校帐户和密码 c。</span><span class="sxs-lookup"><span data-stu-id="76f2c-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="76f2c-110">单击“确定”。</span><span class="sxs-lookup"><span data-stu-id="76f2c-110">Click **OK**.</span></span> 

2. <span data-ttu-id="76f2c-111">运行以下命令以创建新会话：</span><span class="sxs-lookup"><span data-stu-id="76f2c-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="76f2c-112">a.</span><span class="sxs-lookup"><span data-stu-id="76f2c-112">a.</span></span> <span data-ttu-id="76f2c-113">运行以下命令：</span><span class="sxs-lookup"><span data-stu-id="76f2c-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="76f2c-114">运行 `Get-IRMConfiguration` 命令。</span><span class="sxs-lookup"><span data-stu-id="76f2c-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="76f2c-115">检查 **ClientAccessServerEnabled** 设置。</span><span class="sxs-lookup"><span data-stu-id="76f2c-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="76f2c-116">a.</span><span class="sxs-lookup"><span data-stu-id="76f2c-116">a.</span></span> <span data-ttu-id="76f2c-117">如果 **ClientAccessServerEnabled** 设置设置为 **False，** 请运行以下 cmdlet： `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="76f2c-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="76f2c-118">始终通过以下命令关闭 powershell 会话： `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="76f2c-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="76f2c-119">有关详细信息，请参阅[Exchange Online PowerShell。](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)</span><span class="sxs-lookup"><span data-stu-id="76f2c-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

