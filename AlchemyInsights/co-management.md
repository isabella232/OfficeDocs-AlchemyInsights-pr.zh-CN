---
title: 协同管理
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1556"
- "9000080"
ms.openlocfilehash: fe7dcebf847fbd7d91632e93e2253bf62ac659aa
ms.sourcegitcommit: 4ed431b2e1aed26d07bd7eba282531537d29ad0e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/30/2019
ms.locfileid: "40910196"
---
# <a name="co-management"></a><span data-ttu-id="5e092-102">协同管理</span><span class="sxs-lookup"><span data-stu-id="5e092-102">Co-management</span></span>

<span data-ttu-id="5e092-103">**从 Config Manager 混合到 Intune 进行迁移的先决条件**</span><span class="sxs-lookup"><span data-stu-id="5e092-103">**Prerequisites for migrating from Config Manager Hybrid to Intune**</span></span>

- <span data-ttu-id="5e092-104">查看[本文](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-hybridmdm-to-intunesa)。</span><span class="sxs-lookup"><span data-stu-id="5e092-104">Review [this article](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-hybridmdm-to-intunesa).</span></span>
- <span data-ttu-id="5e092-105">向[您的用户添加 Intune 许可证](https://docs.microsoft.com/intune/licenses-assign)。</span><span class="sxs-lookup"><span data-stu-id="5e092-105">[Add an Intune license to your users](https://docs.microsoft.com/intune/licenses-assign).</span></span>
- <span data-ttu-id="5e092-106">配置共同管理时使用[边缘浏览器](https://www.microsoft.com/windows/microsoft-edge)。</span><span class="sxs-lookup"><span data-stu-id="5e092-106">Use the [Edge browser](https://www.microsoft.com/windows/microsoft-edge) when configuring Co-management.</span></span>

<span data-ttu-id="5e092-107">**如何在 Intune 管理的设备上安装配置管理器客户端**</span><span class="sxs-lookup"><span data-stu-id="5e092-107">**How to I install the Config Manager client on Intune-managed devices**</span></span>

<span data-ttu-id="5e092-108">请参阅[INTUNE MDM 托管 Windows 设备](https://docs.microsoft.com/sccm/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm)。</span><span class="sxs-lookup"><span data-stu-id="5e092-108">See [Intune MDM-managed Windows devices](https://docs.microsoft.com/sccm/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm).</span></span>

<span data-ttu-id="5e092-109">**如果我只想更改 MDM 颁发机构，该怎么办？**</span><span class="sxs-lookup"><span data-stu-id="5e092-109">**What if I just want to change MDM authority?**</span></span>

<span data-ttu-id="5e092-110">在不打开支持案例的情况下，可以更改 MDM 证书颁发机构。</span><span class="sxs-lookup"><span data-stu-id="5e092-110">MDM Authority can be changed without opening a support case.</span></span> <span data-ttu-id="5e092-111">请查看以下文档以帮助更改你的 MDM 证书颁发机构：</span><span class="sxs-lookup"><span data-stu-id="5e092-111">Please review the following documentation to assist in changing your MDM authority:</span></span>
- [<span data-ttu-id="5e092-112">将 MDM 颁发机构从 Config Manager 更改为 Intune 独立</span><span class="sxs-lookup"><span data-stu-id="5e092-112">Change MDM Authority from Config Manager to Intune standalone</span></span>](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-change-mdm-authority)
- [<span data-ttu-id="5e092-113">将 MDM 颁发机构从 Intune 独立更改为配置管理器</span><span class="sxs-lookup"><span data-stu-id="5e092-113">Change MDM Authority from Intune standalone to Config Manager</span></span>](https://docs.microsoft.com/intune-classic/deploy-use/prerequisites-for-enrollment#what-to-do-if-you-choose-the-wrong-mdm-authority-setting)