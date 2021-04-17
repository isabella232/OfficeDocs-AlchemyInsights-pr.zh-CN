---
title: 现有监视器疑难解答
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
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824569"
---
# <a name="troubleshoot-an-existing-monitor"></a>现有监视器疑难解答

尝试这些解决方案对监视器进行疑难解答。 

**刷新监视器的显示：**

同时按以下键：Windows 键 + Ctrl + Shift + B。这将刷新与图形驱动程序的通信。 监视器将暂时闪烁，几秒钟后将返回。

**监视器硬件疑难解答：**

1. 拔下电脑与显示器的连接电缆，然后重新插入。
2. 断开电脑上所有不必要的设备（例如适配器或扩展坞）的连接。

**如果你最近在你的电脑上安装了更新，你可以回滚显示驱动程序：**

1. 选择 **"开始**"， **键入设备管理器**，然后 **从结果中选择"设备** 管理器"。
2. 展开"**显示适配器"** 部分，右键单击显示适配器，然后选择"属性 **"。**
3. 导航到驱动程序 **选项卡** ，然后选择 **回滚驱动程序**。 <br>
注意：如果不可用或灰显，请从以下选项中选择"否"以移动到下一步。
4. 你可能需要重新启动电脑，这些更改才能生效。

**卸载并重新安装显示驱动程序：**

1. 选择 **"开始**"， **键入设备管理器**，然后 **从结果中选择"设备** 管理器"。
2. 展开"**显示适配器"** 部分，右键单击显示适配器，然后选择"**卸载设备"。** 
3. 选中"删除此设备的 **驱动程序软件"旁边的框，** 然后选择"卸载 **"。**<br>
注意：在此阶段，系统可能会要求你重新启动计算机。 在重新启动之前，请务必记下剩余的说明。
4. 再次打开设备管理器。
5. 展开"**显示适配器"** 部分，右键单击显示适配器，然后选择"**更新驱动程序"。**
6. 选择 **"自动搜索"以更新驱动程序软件，** 然后按照安装说明进行操作。