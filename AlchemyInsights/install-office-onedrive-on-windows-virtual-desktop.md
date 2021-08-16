---
title: 在 Windows Virtual Desktop 安装 Office 和 OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 226bd24a955f6165969102c8cf00cf45da537ee05a5363c74f1dfd055d922e1d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028606"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>在 Windows Virtual Desktop 安装 Office 和 OneDrive

1. [准备和自定义主 VHD](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image)。 如果尚未创建虚拟机 （VM），请创建虚拟机。

1. [在共享计算机激活模式下安装 Office](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode)。 通过共享计算机激活，多个用户访问 Office。

1. [在按计算机模式下安装 OneDrive](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode)。通常，OneDrive 是按用户安装的，但此处应按计算机进行安装。