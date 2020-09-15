---
title: 现有监视器疑难解答
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
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690701"
---
# <a name="troubleshoot-an-existing-monitor"></a>排除现有监视器的故障

请尝试使用以下解决方案对显示器进行故障排除。 

**刷新监视器的显示：**

同时按以下键： Windows 键 + Ctrl + Shift + B。这将刷新与您的图形驱动程序的通信。 你的监视器将短暂闪烁并在几秒钟后返回回来。

**监视器硬件故障排除：**

1. 拔下将电脑连接到显示器的电缆，然后重新插回。
2. 断开电脑 (等所有非必要设备，如适配器或停靠) 。

**如果你最近在你的电脑上安装了更新，则可以回滚你的显示驱动程序：**

1. 选择 " **开始**"，键入 " **设备管理器**"，然后从结果中选择 " **设备管理器** "。
2. 展开 " **显示适配器** " 部分，右键单击您的显示适配器，用 and "选择 **属性**"。
3. 导航到 " **驱动程序** " 选项卡，然后选择 " **返回驱动程序**"。 <br>
注意：如果此方法不可用或显示为灰色，请从以下选项中选择 " **否** " 以移到下一步。
4. 您可能需要重新启动电脑，这些更改才会生效。

**卸载并重新安装您的显示驱动程序：**

1. 选择 " **开始**"，键入 " **设备管理器**"，然后从结果中选择 " **设备管理器** "。
2. 展开 " **显示适配器** " 部分，右键单击您的显示适配器，用 and "选择 **卸载设备**"。 
3. 选择 " **删除此设备的驱动程序软件** " 旁边的框，然后选择 " **卸载**"。<br>
注意：系统可能会要求您在此阶段重新启动计算机。 重新启动之前，请务必记下剩余的说明。
4. 再次打开 "设备管理器"。
5. 展开 " **显示适配器** " 部分，右键单击您的显示适配器，然后选择 " **更新驱动程序**"。
6. **为更新驱动程序软件选择 "自动搜索**"，然后按照安装说明进行操作。