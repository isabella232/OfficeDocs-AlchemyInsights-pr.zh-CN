---
title: 连接到 MSCommerce 模块
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3528"
ms.openlocfilehash: 41dd044d99d14f25ea15699bfb74f7c37e3928c1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713228"
---
# <a name="connect-to-the-mscommerce-module"></a><span data-ttu-id="273e8-102">连接到 MSCommerce 模块</span><span class="sxs-lookup"><span data-stu-id="273e8-102">Connect to the MSCommerce module</span></span>

<span data-ttu-id="273e8-103">您必须先连接到 MSCommerce 模块，然后才能查看或设置 AllowSelfServicePurchase 策略。</span><span class="sxs-lookup"><span data-stu-id="273e8-103">You must be connected to the MSCommerce module before you can view or set the AllowSelfServicePurchase policy.</span></span>  

<span data-ttu-id="273e8-104">若要连接到 MSCommerce 模块，请在 PowerShell 提示符下 (PS C： \) ，输入以下命令：</span><span class="sxs-lookup"><span data-stu-id="273e8-104">To connect to the MSCommerce module, at the PowerShell prompt (PS C:\), enter the following command:</span></span>

`Connect-MSCommerce`

<span data-ttu-id="273e8-105">这将打开登录对话框。</span><span class="sxs-lookup"><span data-stu-id="273e8-105">This will open a sign-in dialog.</span></span> <span data-ttu-id="273e8-106">输入您的用户名和密码以登录。</span><span class="sxs-lookup"><span data-stu-id="273e8-106">Enter your username and password to sign-in.</span></span>

<span data-ttu-id="273e8-107">**注意：** &nbsp; &nbsp;用于登录的帐户必须是公司或帐单管理员。</span><span class="sxs-lookup"><span data-stu-id="273e8-107">**NOTE:**&nbsp;&nbsp;The account used to sign in must be a Company or Billing Administrator.</span></span>
