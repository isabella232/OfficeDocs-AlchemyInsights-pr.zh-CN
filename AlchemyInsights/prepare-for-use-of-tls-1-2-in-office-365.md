---
title: 准备好在 Microsoft 365 中使用 TLS 1.2
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Critical
ms.custom:
- "1266"
- "1600052"
ms.assetid: d5c84f5c-a3ca-4abd-8633-7e9ff01328a9
ms.openlocfilehash: 1ec40ba36c69296298e24dca64a873d53682833a
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085894"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a>准备好在 Microsoft 365 中使用 TLS 1.2

自 2018 年 10 月 31 日起，Microsoft 365 将继续向 TLS 1.2 过渡。 自 2020 年 10 月 15 日起，O365 将开始在服务中弃用 TLS 1.0 和 1.1。 此更改的推出将在未来几个星期和几个月内继续进行，但客户应假定自 2020 年 10 月 15 日起、与 O365 交互时， TLS 1.0/1.1 调用不工作。 如前所述（2017 年 12 月的 MC126199、2018 年 2 月的 MC128929、2019 年 7 月的 MC186827 和 2020 年 7 月的 MC218794），我们正将所有在线服务转到传输层安全性 (TLS) 1.2+，以在默认情况下、提供最佳加密并提高服务安全性。 客户仍可选择在其服务器和资源上使用 TLS 1.0/1.1，但他们应假定与 O365 资源交互时，只有 TLS 1.2 或更高版本工作。
  
若要了解有关这些更改的详细信息，请参阅 [此处](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) 和 [此处](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide)。

  