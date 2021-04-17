---
title: OneDrive 崩溃疑难解答
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
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826189"
---
# <a name="troubleshoot-onedrive-crashes"></a>OneDrive 崩溃疑难解答

如果 OneDrive 反复崩溃，请尝试以下故障排除步骤：

**确保未设置注册表项：**

1. 打开注册表编辑器，导航至 HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. 如果 DisableFileSyncNGSC 存在，并且设置为 1，请打开该项，将值更改为 0。
3. 通过转到“开始”，手动启动 OneDrive， ![按 Windows 徽标键](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)在搜索框中键入 OneDrive，然后单击 OneDrive 桌面应用程序。

**重置 OneDrive：**

注意：

- 重置 OneDrive 将断开所有现有同步连接（如果设置了个人 OneDrive 也会断开其连接）。
- 在计算机上重置 OneDrive 不会丢失文件或数据。

**重置 OneDrive：**

1. 按 Windows 徽标键和 “R”打开“运行”对话框。
2. 键入 %localappdata%\Microsoft\OneDrive\onedrive.exe /reset 并按“确定”。 “命令”窗口可能会一闪而过。
3. 通过转到“开始”，手动启动 OneDrive， ![按 Windows 徽标键](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)在搜索框中键入 OneDrive，然后单击 OneDrive 桌面应用程序。

注意：

- 如果在重置之前选择了仅同步部分文件夹，则同步完成之后将需要再次执行该操作。 有关详细信息，请参阅 [选择要同步到计算机的 OneDrive 文件夹](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) 。
- 您需要为您的个人 OneDrive 和 OneDrive for Business 完成此操作。