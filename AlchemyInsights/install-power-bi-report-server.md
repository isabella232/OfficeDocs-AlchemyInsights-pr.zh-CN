---
title: 安装 Power BI Report Server
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1304"
- "2500001"
ms.openlocfilehash: 3ea596547093773ab872ca34e8dd3a4e49e59fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755085"
---
# <a name="install-power-bi-report-server"></a>安装 Power BI Report Server

1. 查找 PowerBIReportServer.exe 的位置并启动安装程序。

2. 选择 " **安装 POWER BI Report Server**"。

3. 选择要安装的版本，然后选择 " **下一步**"。

4. 您可以从下拉中选择评估版或开发人员版。  否则，可以输入从 Power BI 服务或批量许可证服务中心获取的服务器的产品密钥。 有关如何获取产品密钥的详细信息，请参阅 "开始之前" 部分。 阅读并同意许可条款和条件，然后选择 " **下一步**"。

5. 您需要具有可用于存储报表服务器数据库的数据库引擎。 选择 " **下一步** " 仅安装报告服务器。

6. 指定报表服务器的安装位置。 选择 " **安装** " 以继续。

7. 成功安装后，选择 " **配置报表服务器** " 以启动 Reporting Services 配置管理器。

您不需要在安装时提供 SQL Server 数据库引擎服务器。 在安装后，您需要一个配置 Reporting Services 的。

有关详细信息，请执行以下操作： https://docs.microsoft.com/power-bi/report-server/install-report-server
