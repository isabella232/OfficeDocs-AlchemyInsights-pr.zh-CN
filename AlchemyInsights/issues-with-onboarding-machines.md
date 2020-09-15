---
title: 载入计算机问题
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: c3203ed68eb19d5f6d75eb2269094bb0422b14cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47676872"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="f8caf-102">载入计算机问题</span><span class="sxs-lookup"><span data-stu-id="f8caf-102">Issues with onboarding machines</span></span>

<span data-ttu-id="f8caf-103">将计算机载入到 MDATP 服务时可能会遇到问题。</span><span class="sxs-lookup"><span data-stu-id="f8caf-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="f8caf-104">如果可以访问最终用户计算机，请按照下列步骤进行操作：</span><span class="sxs-lookup"><span data-stu-id="f8caf-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="f8caf-105">下载[客户端连接分析器](https://aka.ms/mdatpanalyzer)诊断工具。</span><span class="sxs-lookup"><span data-stu-id="f8caf-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="f8caf-106">提取并运行 MDATPAnalyzer.cmd。</span><span class="sxs-lookup"><span data-stu-id="f8caf-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="f8caf-107">在名为 MDATPClientAnalyzerResult 的文件夹中找到诊断日志，该文件夹与下载分析器工具的文件夹相同。</span><span class="sxs-lookup"><span data-stu-id="f8caf-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="f8caf-108">查看日志文件 MDATPClientAnalyzer.txt，以查找连接或 Internet 代理设置问题。</span><span class="sxs-lookup"><span data-stu-id="f8caf-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>