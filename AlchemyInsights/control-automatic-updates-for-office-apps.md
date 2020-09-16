---
title: 控制 Office 应用的自动更新
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: ab3d6e60bc1b67220adbdf7ba61599a6b7aa663a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747766"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="d9aea-102">控制 Office 应用的自动更新</span><span class="sxs-lookup"><span data-stu-id="d9aea-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="d9aea-103">默认情况下，Office 应用的更新会自动下载并在后台应用，无需任何用户干预。</span><span class="sxs-lookup"><span data-stu-id="d9aea-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="d9aea-104">但是，管理员可以使用 Office Update 设置控制更新的应用方式。</span><span class="sxs-lookup"><span data-stu-id="d9aea-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="d9aea-105">更新设置允许管理员启用或禁用自动更新、显示或隐藏 Office 中的“**立即更新**”按钮、设置更新截止日期等。</span><span class="sxs-lookup"><span data-stu-id="d9aea-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="d9aea-106">有关详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="d9aea-106">For detailed information, see:</span></span>

- [<span data-ttu-id="d9aea-107">配置 Office 的更新设置</span><span class="sxs-lookup"><span data-stu-id="d9aea-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="d9aea-108">Office 的自动更新未启用</span><span class="sxs-lookup"><span data-stu-id="d9aea-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="d9aea-109">定义 Office 安装后的更新方式</span><span class="sxs-lookup"><span data-stu-id="d9aea-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="d9aea-110">若要查看应用于客户端计算机的现有更新设置，请按照以下步骤进行操作：</span><span class="sxs-lookup"><span data-stu-id="d9aea-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="d9aea-111">转到“**开始**” > “**运行**” > “**regedit**”，打开注册表编辑器。</span><span class="sxs-lookup"><span data-stu-id="d9aea-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="d9aea-112">切换到以下位置并查看 Office Update 设置：</span><span class="sxs-lookup"><span data-stu-id="d9aea-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="d9aea-113">a.</span><span class="sxs-lookup"><span data-stu-id="d9aea-113">a.</span></span> <span data-ttu-id="d9aea-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="d9aea-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="d9aea-115">b.</span><span class="sxs-lookup"><span data-stu-id="d9aea-115">b.</span></span> <span data-ttu-id="d9aea-116">ClickToRun\Configuration</span><span class="sxs-lookup"><span data-stu-id="d9aea-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="d9aea-117">**注意** 如果设置了OfficeMgmtCOM 注册表项，则可能会在“**Office**” > “**帐户**” > “**Office Updates**”中看到“更新由系统管理员管理”消息。</span><span class="sxs-lookup"><span data-stu-id="d9aea-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="d9aea-118">有关详细信息，请参阅[使用 Microsoft Endpoint Configuration Manager 管理 Microsoft 365 应用版更新](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager)。</span><span class="sxs-lookup"><span data-stu-id="d9aea-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  