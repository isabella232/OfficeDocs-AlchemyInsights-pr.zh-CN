---
title: 远程修复将 Windows 10 设备载入 Microsoft Defender 高级威胁防护的问题
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
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736071"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a><span data-ttu-id="05e1b-102">远程修复将 Windows 10 设备载入 Microsoft Defender 高级威胁防护的问题</span><span class="sxs-lookup"><span data-stu-id="05e1b-102">Remotely fix problems with onboarding Windows 10 devices to Microsoft Defender Advanced Threat Protection</span></span>

<span data-ttu-id="05e1b-103">如果可以访问远程计算机，请按照以下步骤操作：</span><span class="sxs-lookup"><span data-stu-id="05e1b-103">If you can access the remote computer, follow these steps:</span></span>

1. <span data-ttu-id="05e1b-104">下载[客户端连接分析器](https://go.microsoft.com/fwlink/?linkid=2143466)诊断工具。</span><span class="sxs-lookup"><span data-stu-id="05e1b-104">Download the [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostic tool.</span></span>
2. <span data-ttu-id="05e1b-105">提取并运行 MDATPAnalyzer.cmd。</span><span class="sxs-lookup"><span data-stu-id="05e1b-105">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="05e1b-106">在 MDATPClientAnalyzerResult 文件夹中找到诊断日志，该文件夹是下载分析工具的同一文件夹。</span><span class="sxs-lookup"><span data-stu-id="05e1b-106">Locate the diagnostic log in the MDATPClientAnalyzerResult folder, which is the same folder where the Analyzer tool was downloaded.</span></span>
4. <span data-ttu-id="05e1b-107">若要查找连接或 Internet 代理设置问题，请查看日志文件 MDATPClientAnalyzer.txt。</span><span class="sxs-lookup"><span data-stu-id="05e1b-107">To find issues with connectivity or Internet proxy settings, review the log file MDATPClientAnalyzer.txt.</span></span>

<span data-ttu-id="05e1b-108">若要了解更多信息，请参阅 [载入计算机的问题](https://go.microsoft.com/fwlink/?linkid=2143634)。</span><span class="sxs-lookup"><span data-stu-id="05e1b-108">To learn more, see [Issues with onboarding machines](https://go.microsoft.com/fwlink/?linkid=2143634).</span></span>
