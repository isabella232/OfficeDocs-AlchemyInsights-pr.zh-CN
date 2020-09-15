---
title: Intune 设备清单
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667868"
---
# <a name="intune-device-inventory"></a>Intune 设备清单

“设备”边栏选项卡使管理员能够按设备深入了解 Intune 中管理的设备。 所显示的信息包括：硬件、发现的应用程序、设备合规性状态和设备配置状态。

硬件和发现的应用程序的清单数据将按七天周期收集。 根据设备操作系统以及设备是个人拥有还是企业拥有，报告的应用程序和硬件特定元素会有所不同。

有关详细信息，请参阅[查看 Intune 中的设备详细信息](https://docs.microsoft.com/intune/device-inventory)。

**常见问题解答**

问：我没有收到注册了 Intune 的 Windows 设备上存在的应用程序的完整清单。 这是为什么？

答：此时，仅列出被标识为公司设备的 Windows 10 电脑的新式应用。 Intune 不会收集有关在这些设备上安装的 Win32 应用的信息。

答：为什么不从所有设备收集电话号码？

答：例如，当你运行移动设备清单报告时，在 Intune 中被归类为公司设备的电话不会用其完整电话号码标识。 “自带设备办公”电话号码总是用星号 (****) 部分屏蔽，并且只显示最后四位数字。