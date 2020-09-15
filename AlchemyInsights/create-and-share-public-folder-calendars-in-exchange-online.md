---
title: 在 Exchange Online 中创建和共享公用文件夹日历
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "634"
- "3500007"
ms.openlocfilehash: d8b28d373db21da42b90aeef75139affd802a5d2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712640"
---
# <a name="create-and-share-public-folder-calendars-in-exchange-online"></a><span data-ttu-id="d5a85-102">在 Exchange Online 中创建和共享公用文件夹日历</span><span class="sxs-lookup"><span data-stu-id="d5a85-102">Create and share public folder calendars in Exchange Online</span></span>

<span data-ttu-id="d5a85-103">只能通过 Outlook 桌面客户端在公用文件夹中创建日历。</span><span class="sxs-lookup"><span data-stu-id="d5a85-103">You can create a calendar in the Public folder only from the Outlook desktop client.</span></span> <span data-ttu-id="d5a85-104">请按照以下步骤设置公用文件夹日历：</span><span class="sxs-lookup"><span data-stu-id="d5a85-104">Use these steps to set up public folder calendars:</span></span>

1. <span data-ttu-id="d5a85-105">确保 Exchange Online 中已部署公用文件夹。</span><span class="sxs-lookup"><span data-stu-id="d5a85-105">Ensure public folders are deployed in Exchange Online.</span></span> <span data-ttu-id="d5a85-106">有关详细信息，请参阅[创建公用文件夹邮箱](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/create-public-folder-mailbox)。</span><span class="sxs-lookup"><span data-stu-id="d5a85-106">For more info, see [Create a public folder mailbox](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/create-public-folder-mailbox).</span></span> 

2. <span data-ttu-id="d5a85-107">确保你已获得创建公用文件夹所需的访问权限。</span><span class="sxs-lookup"><span data-stu-id="d5a85-107">Ensure you're assigned necessary access permissions to create the public folder.</span></span> <span data-ttu-id="d5a85-108">有关详细信息，请参阅 [Exchange Server 的公用文件夹权限](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server)。</span><span class="sxs-lookup"><span data-stu-id="d5a85-108">For more info, see [Public folder permissions for Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span></span> 
  
3. <span data-ttu-id="d5a85-109">登录到 Outlook 桌面客户端，确保你可访问公用文件夹部署。</span><span class="sxs-lookup"><span data-stu-id="d5a85-109">Log in to the Outlook desktop client and ensure you can access your public folder deployment.</span></span>

    <span data-ttu-id="d5a85-110">如果在使用 Outlook 桌面客户端访问公用文件夹时遇到问题，请参阅 [Exchange Online 用户无法使用 Outlook 或 OWA 连接到公用文件夹](https://aka.ms/pfcte)。</span><span class="sxs-lookup"><span data-stu-id="d5a85-110">If you're having trouble accessing public folders by using the Outlook desktop client, see [Exchange Online users can't connect to public folders by using Outlook or OWA](https://aka.ms/pfcte).</span></span>

4. <span data-ttu-id="d5a85-111">创建新的公用文件夹日历类型。</span><span class="sxs-lookup"><span data-stu-id="d5a85-111">Create a new public folder calendar type.</span></span>

<span data-ttu-id="d5a85-112">公用文件夹默认共享给其他所有用户。</span><span class="sxs-lookup"><span data-stu-id="d5a85-112">The public folder is shared to all other users by default.</span></span> <span data-ttu-id="d5a85-113">公用文件夹的所有者可通过 Outlook 桌面客户端更改权限。</span><span class="sxs-lookup"><span data-stu-id="d5a85-113">Owner of the public folder can change the permissions from Outlook desktop client.</span></span> <span data-ttu-id="d5a85-114">有关详细信息，请参阅 [Exchange Server 的公用文件夹权限](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server)。</span><span class="sxs-lookup"><span data-stu-id="d5a85-114">For more info, see [Public folder permissions for Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span></span>

<span data-ttu-id="d5a85-115">**注意**：公用文件夹日历专门设计用于组织内部，无法在 Internet 上发布。</span><span class="sxs-lookup"><span data-stu-id="d5a85-115">**Note** Public folder calendars are designed to be used within the organization and can't be published on the Internet.</span></span> <span data-ttu-id="d5a85-116">如果你打算在 Internet 上发布日历，请使用共享邮箱。</span><span class="sxs-lookup"><span data-stu-id="d5a85-116">Use a shared mailbox if your intention is to publish a calendar on the  Internet.</span></span>