---
title: AIP 扫描仪：安装和配置
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
- "9002278"
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821653"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="31242-102">AIP 扫描仪：安装和配置</span><span class="sxs-lookup"><span data-stu-id="31242-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="31242-103">**若要安装 AIP 扫描程序，请按照推荐的指南操作**：</span><span class="sxs-lookup"><span data-stu-id="31242-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="31242-104">如果要升级而不是执行全新安装，请确保已遵循[升级 Azure 信息保护扫描程序](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner)和统一标签客户端的准则，请参阅[升级 Azure 信息保护扫描程序](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)。</span><span class="sxs-lookup"><span data-stu-id="31242-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="31242-105">验证是否符合所有[防火墙和网络基础结构设置要求](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)。</span><span class="sxs-lookup"><span data-stu-id="31242-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="31242-106">请确保你的[策略设置](https://docs.microsoft.com/azure/information-protection/configure-policy)为“自动标记”或在策略中有一个默认标签。</span><span class="sxs-lookup"><span data-stu-id="31242-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="31242-107">请确保已按照 [Azure 信息保护客户端支持的文件类型](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection)中的说明为标签/保护配置了相关文件类型。</span><span class="sxs-lookup"><span data-stu-id="31242-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="31242-108">此外，如果要更改默认行为，请遵循以下准则：[更改文件的默认保护级别](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)。</span><span class="sxs-lookup"><span data-stu-id="31242-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="31242-109">验证配置为运行扫描程序服务的用户帐户是否有权访问所有配置的存储库。</span><span class="sxs-lookup"><span data-stu-id="31242-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="31242-110">如果仍遇到问题，请将扫描程序日志导出并添加到支持票证中。</span><span class="sxs-lookup"><span data-stu-id="31242-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="31242-111">**导出 Azure 信息保护扫描程序日志**</span><span class="sxs-lookup"><span data-stu-id="31242-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="31242-112">导航到运行扫描程序服务的用户上下文中的 %localappdata%\Microsoft\MSIP。</span><span class="sxs-lookup"><span data-stu-id="31242-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="31242-113">将 MSIP 文件夹下的所有内容全部压缩。</span><span class="sxs-lookup"><span data-stu-id="31242-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="31242-114">将日志保存到选定位置，并将其附加到服务请求中。</span><span class="sxs-lookup"><span data-stu-id="31242-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="31242-115">还可以使用 [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)。</span><span class="sxs-lookup"><span data-stu-id="31242-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="31242-116">**有关详细信息，请参阅**：</span><span class="sxs-lookup"><span data-stu-id="31242-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="31242-117">部署 Azure 信息保护扫描程序以自动分类和保护文件</span><span class="sxs-lookup"><span data-stu-id="31242-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="31242-118">指定并使用 Set-AIPAuthentication 的令牌参数</span><span class="sxs-lookup"><span data-stu-id="31242-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="31242-119">运行发现周期并查看扫描仪报告</span><span class="sxs-lookup"><span data-stu-id="31242-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="31242-120">查阅 Azure 信息保护文档</span><span class="sxs-lookup"><span data-stu-id="31242-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="31242-121">Azure 信息保护要求</span><span class="sxs-lookup"><span data-stu-id="31242-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="31242-122">下载 Azure 信息保护客户端</span><span class="sxs-lookup"><span data-stu-id="31242-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
