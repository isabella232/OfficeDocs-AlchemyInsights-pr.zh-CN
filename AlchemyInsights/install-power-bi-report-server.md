---
title: 安装 Power BI 报表服务器
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1304"
- "2500001"
ms.openlocfilehash: 8479be2a538228b71033aca3907d3aba2f5e28fb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51832084"
---
# <a name="install-power-bi-report-server"></a>安装 Power BI 报表服务器

1. 找到安装PowerBIReportServer.exe并启动安装程序。

2. 选择 **"安装 Power BI 报表服务器"。**

3. 选择要安装的版本，然后选择"下一 **步"。**

4. 你可以从下拉列表中选择评估版或开发人员版。  否则，您可以输入从 Power BI 服务或批量许可服务中心获取的服务器的产品密钥。 若要详细了解如何获取产品密钥，请参阅开始之前部分。 阅读并同意许可条款和条件，然后选择"下一 **步"。**

5. 您需要有一个数据库引擎可用于存储报表服务器数据库。 选择 **"下** 一步"以仅报表服务器安装程序。

6. 指定客户端的安装报表服务器。 选择 **"安装** "以继续。

7. 成功设置后，选择 **"配置报表服务器** "以启动 Reporting Services Configuration Manager。

在安装时，SQL Server数据库引擎服务器可用。 安装后，您需要一个配置 Reporting Services。

有关详细信息： https://docs.microsoft.com/power-bi/report-server/install-report-server
