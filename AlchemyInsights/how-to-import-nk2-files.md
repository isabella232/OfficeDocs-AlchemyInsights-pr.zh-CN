---
title: 操作方法-nk2-文件
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 6a823f6e0c4c46de64dd7b70fb40c76255d78ec1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780049"
---
# <a name="how-to-import-nk2-files"></a><span data-ttu-id="09eec-102">如何导入 nk2 文件</span><span class="sxs-lookup"><span data-stu-id="09eec-102">How to import .nk2 files</span></span> 

<span data-ttu-id="09eec-103">当您首次启动 Microsoft Outlook 2013、Outlook 2016、Outlook 2019 或 Outlook for Microsoft 365 时，您的昵称缓存 (存储在 *profilename*文件中) 将导入到默认邮件存储区中的隐藏邮件中。</span><span class="sxs-lookup"><span data-stu-id="09eec-103">When you start Microsoft Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365 for the first time, your nickname cache (stored in the *profilename*.nk2 file) is imported into a hidden message in your default message store.</span></span>

<span data-ttu-id="09eec-104">若要将 nk2 文件导入到 Outlook 2013、Outlook 2016、Outlook 2019 或 Outlook for Microsoft 365 中，请确保. nk2 文件位于以下文件夹中：%appdata%\Microsoft\Outlook</span><span class="sxs-lookup"><span data-stu-id="09eec-104">To import .nk2 files into Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365, make sure that the .nk2 file is in the following folder: %appdata%\Microsoft\Outlook</span></span>

<span data-ttu-id="09eec-105">**注意**： nk2 文件必须具有与当前 Outlook 2013 或 outlook 2016 配置文件相同的名称。</span><span class="sxs-lookup"><span data-stu-id="09eec-105">**Note**: The .nk2 file must have the same name as your current Outlook 2013 or Outlook 2016 profile.</span></span> <span data-ttu-id="09eec-106">默认情况下，配置文件名称为 "Outlook"。</span><span class="sxs-lookup"><span data-stu-id="09eec-106">By default, the profile name is "Outlook."</span></span> <span data-ttu-id="09eec-107">若要检查配置文件名称，请按照以下步骤操作：</span><span class="sxs-lookup"><span data-stu-id="09eec-107">To check the profile name, follow these steps:</span></span> 
1. <span data-ttu-id="09eec-108">单击“开始”\*\*\*\*，然后单击“控制面板”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="09eec-108">Click **Start**, and then click **Control Panel**.</span></span>
2. <span data-ttu-id="09eec-109">双击 " **邮件**"。</span><span class="sxs-lookup"><span data-stu-id="09eec-109">Double-click **Mail**.</span></span>
3. <span data-ttu-id="09eec-110">在 "邮件设置" 对话框中，选择 " **显示配置文件**"。</span><span class="sxs-lookup"><span data-stu-id="09eec-110">In the Mail Setup dialog box, select **Show Profiles**.</span></span>
4. <span data-ttu-id="09eec-111">选择 "**开始**  >  **运行**"。</span><span class="sxs-lookup"><span data-stu-id="09eec-111">Select **Start** > **Run**.</span></span>
5. <span data-ttu-id="09eec-112">在 " **打开** " 框中，键入 *outlook.exe/importnk2*"，然后选择 **" 确定 "**。</span><span class="sxs-lookup"><span data-stu-id="09eec-112">In the **Open** box, type *outlook.exe /importnk2*, and then select **OK**.</span></span> 

<span data-ttu-id="09eec-113">导入 nk2 文件后，该文件的内容将合并到存储在邮箱中的现有昵称缓存中。</span><span class="sxs-lookup"><span data-stu-id="09eec-113">After you import the .nk2 file, the contents of the file are merged into the existing nickname cache stored in your mailbox.</span></span>

<span data-ttu-id="09eec-114">**注意**：在下一次启动 outlook 2013、outlook 2016、outlook 2019 或 Outlook for Microsoft 365 时，将使用 .old 文件扩展名将. nk2 文件重命名。</span><span class="sxs-lookup"><span data-stu-id="09eec-114">**Note**: The .nk2 file is renamed with a .old file name extension the next time you start Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365.</span></span> <span data-ttu-id="09eec-115">如果要重新导入 nk2 文件，请首先删除 .old 文件扩展名。</span><span class="sxs-lookup"><span data-stu-id="09eec-115">If want to re-import the .nk2 file, remove the .old file name extension first.</span></span>

<span data-ttu-id="09eec-116">有关详细信息，请参阅将 [自动完成列表导入或复制到另一台计算机](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%)。</span><span class="sxs-lookup"><span data-stu-id="09eec-116">For more information, see [Import or copy the Auto-Complete List to another computer](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).</span></span>