---
title: 配置 Microsoft Defender ATP 扫描排除
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6027"
- "9001464"
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "49768352"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="3cba3-102">配置 Microsoft Defender ATP 扫描排除</span><span class="sxs-lookup"><span data-stu-id="3cba3-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="3cba3-103">一般来说，你可以从 Microsoft Defender ATP 扫描排除一些文件拓展和文件夹位置。</span><span class="sxs-lookup"><span data-stu-id="3cba3-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="3cba3-104">你也可以为由某些过程打开的文件配置排除。</span><span class="sxs-lookup"><span data-stu-id="3cba3-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="3cba3-105">有关更多信息，请参阅[基于文件拓展和文件夹位置配置和验证排除](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus)和[为由某些过程打开的文件配置排除](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)。</span><span class="sxs-lookup"><span data-stu-id="3cba3-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="3cba3-106">要为 **Windows Server 2016 和 2019** 配置排除，请参阅[在 Windows Server 上配置 Microsoft Defender 防病毒排除](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)。</span><span class="sxs-lookup"><span data-stu-id="3cba3-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="3cba3-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="3cba3-107">**Mac**</span></span>

<span data-ttu-id="3cba3-108">有关更多关于受支持的排除类型以及在 Mac 上配置排除列表，请参阅[受支持的排除类型](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types)和[如何配置排除列表](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions)。</span><span class="sxs-lookup"><span data-stu-id="3cba3-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="3cba3-109">**注意** 你也可以使用 EICAR 测试文件验证排除列表。</span><span class="sxs-lookup"><span data-stu-id="3cba3-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="3cba3-110">有关更多信息，请参阅[使用 EICAR 测试文件验证排除列表](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)。</span><span class="sxs-lookup"><span data-stu-id="3cba3-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="3cba3-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="3cba3-111">**Linux**</span></span>

<span data-ttu-id="3cba3-112">有关更多关于受支持的排除类型以及在 Linux 上配置排除列表，请参阅[受支持的排除类型](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types)和[在 Linux 上配置和验证排除](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)。</span><span class="sxs-lookup"><span data-stu-id="3cba3-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="3cba3-113">**注意** 你也可以使用 EICAR 测试文件验证排除列表。</span><span class="sxs-lookup"><span data-stu-id="3cba3-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="3cba3-114">有关更多信息，请参阅[使用 EICAR 测试文件验证排除列表](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)。</span><span class="sxs-lookup"><span data-stu-id="3cba3-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 