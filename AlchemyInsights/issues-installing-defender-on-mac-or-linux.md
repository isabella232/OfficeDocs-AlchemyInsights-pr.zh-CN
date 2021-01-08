---
title: 有关在 Mac 或 Linux 上安装 Microsoft Defender 的问题
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
- "6028"
- "9001222"
ms.openlocfilehash: a8d5ad2246b9b83e1e0a4d5be4dd8bb41c16e734
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "49768346"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a><span data-ttu-id="12703-102">有关在 Mac 或 Linux 上安装 Microsoft Defender 的问题</span><span class="sxs-lookup"><span data-stu-id="12703-102">Issues installing Microsoft Defender on Mac or Linux</span></span>

<span data-ttu-id="12703-103">**Mac**</span><span class="sxs-lookup"><span data-stu-id="12703-103">**Mac**</span></span>

- <span data-ttu-id="12703-104">在安装 Mac 版 Microsoft Defender ATP 前确保满足系统要求。</span><span class="sxs-lookup"><span data-stu-id="12703-104">Ensure that system requirements are met before installing Microsoft Defender ATP for Mac.</span></span> <span data-ttu-id="12703-105">有关更多信息，请参阅[如何安装 Mac 版 Microsoft Defender ATP](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)。</span><span class="sxs-lookup"><span data-stu-id="12703-105">For more info, see [How to install Microsoft Defender ATP for Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span></span>  
- <span data-ttu-id="12703-106">检查此文件中的信息："/Library/Logs/Microsoft/mdatp/install.log"。</span><span class="sxs-lookup"><span data-stu-id="12703-106">Review the information in the file: "/Library/Logs/Microsoft/mdatp/install.log".</span></span>

<span data-ttu-id="12703-107">**Linux**</span><span class="sxs-lookup"><span data-stu-id="12703-107">**Linux**</span></span>

- <span data-ttu-id="12703-108">在安装 Linux 版 Microsoft Defender ATP 前确保满足系统要求。</span><span class="sxs-lookup"><span data-stu-id="12703-108">Ensure that system requirements are met before installing Microsoft Defender ATP for Linux.</span></span> <span data-ttu-id="12703-109">有关更多信息，请参阅[如何安装 Linux 版 Microsoft Defender ATP](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)。</span><span class="sxs-lookup"><span data-stu-id="12703-109">For more info, see [How to install Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span> 
- <span data-ttu-id="12703-110">要验证 MDATP 服务正在允许，请参阅[安装失败](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)。</span><span class="sxs-lookup"><span data-stu-id="12703-110">To verify that MDATP service is running, see [Installation failed](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span></span>  
    <span data-ttu-id="12703-111">如果服务未运行，要故障排除和解决问题，请参阅[mdatp 服务未运行时故障排除步骤](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)。</span><span class="sxs-lookup"><span data-stu-id="12703-111">To troubleshoot and resolve issues if the service is not running, see [Steps to troubleshoot if mdatp service isn't running](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span></span>
- <span data-ttu-id="12703-112">客户端配置用于验证产品的健康，有关检查客户端配置步骤和运行检测测试 EICAR 文本文件的信息，请参阅[客户端配置](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)。</span><span class="sxs-lookup"><span data-stu-id="12703-112">For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span></span>  

    <span data-ttu-id="12703-113">**注意** 要查看受支持的文件系统的访问活动列表，请参与[Linux 版 Microsoft Defender ATP](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)。</span><span class="sxs-lookup"><span data-stu-id="12703-113">**Note** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span>