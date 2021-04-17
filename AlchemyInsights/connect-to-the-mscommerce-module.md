---
title: 连接到 MSCommerce 模块
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3528"
ms.openlocfilehash: e77c6a329ac99a4cea4f143dcb3c661b6a518e35
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817018"
---
# <a name="connect-to-the-mscommerce-module"></a><span data-ttu-id="28ec7-102">连接到 MSCommerce 模块</span><span class="sxs-lookup"><span data-stu-id="28ec7-102">Connect to the MSCommerce module</span></span>

<span data-ttu-id="28ec7-103">必须先连接到 MSCommerce 模块，然后才能查看或设置 AllowSelfServicePurchase 策略。</span><span class="sxs-lookup"><span data-stu-id="28ec7-103">You must be connected to the MSCommerce module before you can view or set the AllowSelfServicePurchase policy.</span></span>  

<span data-ttu-id="28ec7-104">若要连接到 MSCommerce 模块，请在 PowerShell 提示符下 (PS \) C： ，输入以下命令：</span><span class="sxs-lookup"><span data-stu-id="28ec7-104">To connect to the MSCommerce module, at the PowerShell prompt (PS C:\), enter the following command:</span></span>

`Connect-MSCommerce`

<span data-ttu-id="28ec7-105">这将打开登录对话框。</span><span class="sxs-lookup"><span data-stu-id="28ec7-105">This will open a sign-in dialog.</span></span> <span data-ttu-id="28ec7-106">输入用户名和密码以登录。</span><span class="sxs-lookup"><span data-stu-id="28ec7-106">Enter your username and password to sign-in.</span></span>

<span data-ttu-id="28ec7-107">**注意：** &nbsp; &nbsp;用于登录的帐户必须是公司或帐单管理员。</span><span class="sxs-lookup"><span data-stu-id="28ec7-107">**NOTE:**&nbsp;&nbsp;The account used to sign in must be a Company or Billing Administrator.</span></span>
