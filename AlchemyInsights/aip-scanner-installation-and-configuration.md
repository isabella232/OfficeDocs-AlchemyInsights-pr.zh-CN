---
title: AIP 扫描仪：安装和配置
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: be5b63ffccd5bbd83e7802e4ef5aa657ed921ae6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686632"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP 扫描仪：安装和配置

**若要安装 AIP 扫描程序，请按照推荐的指南操作**：

1. 如果要升级而不是执行全新安装，请确保已遵循[升级 Azure 信息保护扫描程序](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner)和统一标签客户端的准则，请参阅[升级 Azure 信息保护扫描程序](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)。
2. 验证是否符合所有[防火墙和网络基础结构设置要求](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)。
3. 请确保你的[策略设置](https://docs.microsoft.com/azure/information-protection/configure-policy)为“自动标记”或在策略中有一个默认标签。
4. 请确保已按照 [Azure 信息保护客户端支持的文件类型](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection)中的说明为标签/保护配置了相关文件类型。 此外，如果要更改默认行为，请遵循以下准则：[更改文件的默认保护级别](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)。
5. 验证配置为运行扫描程序服务的用户帐户是否有权访问所有配置的存储库。
6. 如果仍遇到问题，请将扫描程序日志导出并添加到支持票证中。

**导出 Azure 信息保护扫描程序日志**

1. 导航到运行扫描程序服务的用户上下文中的 %localappdata%\Microsoft\MSIP。
2. 将 MSIP 文件夹下的所有内容全部压缩。
3. 将日志保存到选定位置，并将其附加到服务请求中。
4. 还可以使用 [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)。

**有关详细信息，请参阅**：
- [部署 Azure 信息保护扫描程序以自动分类和保护文件](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [指定并使用 Set-AIPAuthentication 的令牌参数](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [运行发现周期并查看扫描仪报告](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [查阅 Azure 信息保护文档](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Azure 信息保护要求](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [下载 Azure 信息保护客户端](https://www.microsoft.com/download/details.aspx?id=53018)
