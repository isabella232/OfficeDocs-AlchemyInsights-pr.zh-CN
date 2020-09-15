---
title: 载入计算机问题
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: c3203ed68eb19d5f6d75eb2269094bb0422b14cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47676872"
---
# <a name="issues-with-onboarding-machines"></a>载入计算机问题

将计算机载入到 MDATP 服务时可能会遇到问题。 如果可以访问最终用户计算机，请按照下列步骤进行操作：

1. 下载[客户端连接分析器](https://aka.ms/mdatpanalyzer)诊断工具。
2. 提取并运行 MDATPAnalyzer.cmd。
3. 在名为 MDATPClientAnalyzerResult 的文件夹中找到诊断日志，该文件夹与下载分析器工具的文件夹相同。
4. 查看日志文件 MDATPClientAnalyzer.txt，以查找连接或 Internet 代理设置问题。