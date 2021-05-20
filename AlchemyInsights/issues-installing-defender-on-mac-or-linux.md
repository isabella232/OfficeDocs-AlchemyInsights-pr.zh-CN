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
ms.openlocfilehash: 39f180852fd0438597fa1ce665b2703fbc7b1aa4
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539670"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a><span data-ttu-id="d9e12-102">有关在 Mac 或 Linux 上安装 Microsoft Defender 的问题</span><span class="sxs-lookup"><span data-stu-id="d9e12-102">Issues installing Microsoft Defender on Mac or Linux</span></span>

<span data-ttu-id="d9e12-103">**Mac**</span><span class="sxs-lookup"><span data-stu-id="d9e12-103">**Mac**</span></span>

- <span data-ttu-id="d9e12-104">在安装 Mac 版 Microsoft Defender ATP 前确保满足系统要求。</span><span class="sxs-lookup"><span data-stu-id="d9e12-104">Ensure that system requirements are met before installing Microsoft Defender ATP for Mac.</span></span> <span data-ttu-id="d9e12-105">有关更多信息，请参阅[如何安装 Mac 版 Microsoft Defender ATP](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)。</span><span class="sxs-lookup"><span data-stu-id="d9e12-105">For more info, see [How to install Microsoft Defender ATP for Mac](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span></span>  
- <span data-ttu-id="d9e12-106">检查此文件中的信息："/Library/Logs/Microsoft/mdatp/install.log"。</span><span class="sxs-lookup"><span data-stu-id="d9e12-106">Review the information in the file: "/Library/Logs/Microsoft/mdatp/install.log".</span></span>

<span data-ttu-id="d9e12-107">**Linux**</span><span class="sxs-lookup"><span data-stu-id="d9e12-107">**Linux**</span></span>

- <span data-ttu-id="d9e12-108">在安装 Linux 版 Microsoft Defender ATP 前确保满足系统要求。</span><span class="sxs-lookup"><span data-stu-id="d9e12-108">Ensure that system requirements are met before installing Microsoft Defender ATP for Linux.</span></span> <span data-ttu-id="d9e12-109">有关详细信息，请参阅[如何安装 Linux 版 MDATP](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)。</span><span class="sxs-lookup"><span data-stu-id="d9e12-109">For more info, see [How to install MDATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span> 
- <span data-ttu-id="d9e12-110">要验证 MDATP 服务正在允许，请参阅[安装失败](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)。</span><span class="sxs-lookup"><span data-stu-id="d9e12-110">To verify that MDATP service is running, see [Installation failed](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span></span>  
    <span data-ttu-id="d9e12-111">如果服务未运行，要故障排除和解决问题，请参阅[mdatp 服务未运行时故障排除步骤](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)。</span><span class="sxs-lookup"><span data-stu-id="d9e12-111">To troubleshoot and resolve issues if the service is not running, see [Steps to troubleshoot if mdatp service isn't running](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span></span>
- <span data-ttu-id="d9e12-112">客户端配置用于验证产品的健康，有关检查客户端配置步骤和运行检测测试 EICAR 文本文件的信息，请参阅[客户端配置](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)。</span><span class="sxs-lookup"><span data-stu-id="d9e12-112">For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span></span>  

    <span data-ttu-id="d9e12-113">**注意** 要查看受支持的文件系统的访问活动列表，请参与 [Linux 版 Microsoft Defender ATP](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)。</span><span class="sxs-lookup"><span data-stu-id="d9e12-113">**Note** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span>