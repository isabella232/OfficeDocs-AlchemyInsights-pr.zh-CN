---
title: 副本集
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 45cf530c3258fa3c7008c3e8251fdb7b74be6911d0487f58c5ce2530e25ca282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54110670"
---
# <a name="replica-set"></a>副本集

AADDS 也称为托管域。 它实际上是由后端运行和维护的两个域控制器。 这两个 DCS 包括一个主 DC 和一个复制 DC。 AADDS (托管) 中的备份是由 Azure 平台管理的自动化过程。 如果托管域出现问题，Azure 支持可帮助你从备份中还原。

您可以在虚拟网络中创建每个副本集。 每个虚拟网络都必须与托管托管域的副本集的所有其他虚拟网络对等。 此配置创建支持目录复制的网格网络拓扑。 虚拟网络可以支持多个副本集，但每个副本集位于不同的虚拟子网中。

有关副本集的更多详细信息，请参阅概 [念副本集](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)。
