---
title: 解决 Mac 上的 MDATP 安装问题
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
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735669"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="8a298-102">解决 Mac 上的 MDATP 安装问题</span><span class="sxs-lookup"><span data-stu-id="8a298-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="8a298-103">如果手动安装失败，则 **安装向导的** "摘要"页将显示以下错误：</span><span class="sxs-lookup"><span data-stu-id="8a298-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="8a298-104">"在安装过程中出错。</span><span class="sxs-lookup"><span data-stu-id="8a298-104">"An error occurred during installation.</span></span> <span data-ttu-id="8a298-105">安装程序遇到导致安装失败的错误。</span><span class="sxs-lookup"><span data-stu-id="8a298-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="8a298-106">请与软件制造商联系寻求帮助。"</span><span class="sxs-lookup"><span data-stu-id="8a298-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="8a298-107">对于 MDM 部署，页面也显示常规安装失败。</span><span class="sxs-lookup"><span data-stu-id="8a298-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="8a298-108">尽管我们不会向最终用户显示确切的错误，但我们在 **/Library/Logs/Microsoft/mdatp/install.log** 中日志文件安装进度进行跟踪。</span><span class="sxs-lookup"><span data-stu-id="8a298-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="8a298-109">每个安装会话都附加到此日志文件。</span><span class="sxs-lookup"><span data-stu-id="8a298-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="8a298-110">若要仅输出上次安装会话，请使用 `sed` 。</span><span class="sxs-lookup"><span data-stu-id="8a298-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="8a298-111">若要了解更多信息，请参阅 [解决 Microsoft Defender ATP for Mac 的安装问题](https://go.microsoft.com/fwlink/?linkid=2144615)。</span><span class="sxs-lookup"><span data-stu-id="8a298-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
