---
title: 解决“未检测到应用程序”错误
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 4e0599f9bdf2c7d16d009627f44b3691c2c250b7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836341"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="5a5e6-102">解决“未检测到应用程序”错误</span><span class="sxs-lookup"><span data-stu-id="5a5e6-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="5a5e6-103">由 Intune 报告的应用安装错误“安装成功后未检测到应用程序”有可能发生在任何主要操作系统平台（Windows、iOS 和 Android）上。</span><span class="sxs-lookup"><span data-stu-id="5a5e6-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="5a5e6-104">产生此错误的最常见的情况包括：</span><span class="sxs-lookup"><span data-stu-id="5a5e6-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="5a5e6-105">初始部署后，在 Intune 之外的第三方应用商店中更新了应用。</span><span class="sxs-lookup"><span data-stu-id="5a5e6-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="5a5e6-106">例如，某些应用程序（如 Google Chrome）可能会执行自动更新。</span><span class="sxs-lookup"><span data-stu-id="5a5e6-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="5a5e6-107">用户在初始安装后卸载了应用。</span><span class="sxs-lookup"><span data-stu-id="5a5e6-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="5a5e6-108">若要解决此问题，请首先检查受影响的设备，确定发生错误的情况。</span><span class="sxs-lookup"><span data-stu-id="5a5e6-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="5a5e6-109">如果是在 Intune 之外更新了应用，可将应用部署设置为忽略应用程序版本。</span><span class="sxs-lookup"><span data-stu-id="5a5e6-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="5a5e6-110">若要执行此操作，请在 **“应用配置”>“应用信息”** 下，将“**忽略应用版本**”设置为“**是**”。</span><span class="sxs-lookup"><span data-stu-id="5a5e6-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="5a5e6-111">当以客户端为目标时，可以根据“需要”部署应用程序，并确保部署最新版本。</span><span class="sxs-lookup"><span data-stu-id="5a5e6-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="5a5e6-112">或者，如果是在 iOS 平台上，可使用与 Apple 批量购买计划相关联的 **自动更新** 功能，该计划可配置为在新的应用程序版本推出时自动更新。</span><span class="sxs-lookup"><span data-stu-id="5a5e6-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="5a5e6-113">有关解决应用安装问题的详细信息，请参阅[解决应用安装问题](https://docs.microsoft.com/intune/troubleshoot-app-install)。</span><span class="sxs-lookup"><span data-stu-id="5a5e6-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
