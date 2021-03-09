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
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568477"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="f412a-102">解决 Mac 上的 MDATP 安装问题</span><span class="sxs-lookup"><span data-stu-id="f412a-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="f412a-103">如果手动安装失败， **则安装向导的** "摘要"页将显示以下错误：</span><span class="sxs-lookup"><span data-stu-id="f412a-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="f412a-104">"安装期间出错。</span><span class="sxs-lookup"><span data-stu-id="f412a-104">"An error occurred during installation.</span></span> <span data-ttu-id="f412a-105">安装程序遇到导致安装失败的错误。</span><span class="sxs-lookup"><span data-stu-id="f412a-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="f412a-106">请联系软件制造商寻求帮助。"</span><span class="sxs-lookup"><span data-stu-id="f412a-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="f412a-107">对于 MDM 部署，页面还显示常规安装失败。</span><span class="sxs-lookup"><span data-stu-id="f412a-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="f412a-108">尽管我们不会向最终用户显示确切的错误，但我们在 **/Library/Logs/Microsoft/mdatp/install.log** 中日志文件安装进度。</span><span class="sxs-lookup"><span data-stu-id="f412a-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="f412a-109">每个安装会话都附加到此日志文件。</span><span class="sxs-lookup"><span data-stu-id="f412a-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="f412a-110">若要仅输出最后一个安装会话，请使用 `sed` 。</span><span class="sxs-lookup"><span data-stu-id="f412a-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="f412a-111">若要了解更多信息，请参阅 Microsoft Defender ATP for Mac 的安装 [问题疑难解答](https://go.microsoft.com/fwlink/?linkid=2144615)。</span><span class="sxs-lookup"><span data-stu-id="f412a-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
