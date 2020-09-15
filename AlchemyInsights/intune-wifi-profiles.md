---
title: Intune Wi-Fi 配置文件
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: afc8142a635b8a9d715eb4325b570be20ad26645
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696251"
---
# <a name="intune-wi-fi-profiles"></a>Intune Wi-Fi 配置文件

MDM 客户端的 Wi-Fi 连接的成功实现依赖于可反映公司 Wi-Fi 基础结构要求的正确部署的配置文件。 若要查看正在调查的客户端平台的相应设置，请参阅： 

[在 Microsoft Intune 中为运行 Android 的设备添加 Wi-Fi 设置](https://docs.microsoft.com/intune/wi-fi-settings-android)

[在 Microsoft Intune 中为 Android 企业版专用且完全托管的设备添加 Wi-Fi 设置](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[在 Microsoft Intune 中为 iOS 和 iPadOS 设备添加 Wi-Fi 设置](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[在 Intune 中为 Windows 10 和更高版本的设备添加 Wi-Fi 设置](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[在 Intune 中为 Windows 设备导入 Wi-Fi 设置](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**常见问题**

**我正在部署的 Wi-Fi 配置文件依赖于该 Wi-Fi 配置文件中指定的已部署证书。但是，配置的配置文件显示错误状态。**

请检查你的设备是否收到了证书。

1. 在 Intune 中，转到“**所有设备**”，然后选择选择相应设备 >“**设备配置**”。

2. 检查是否列出了所有预期的配置文件，并且状态为成功。

3. 对于 Android 配置文件，如果证书链中有中间证书，请确保将其部署到 Android 设备。

    若要检查证书状态，请转到“**设备配置**” > “**配置文件**” > “**Android 中间 CA**” > “**属性**” > “**受信任的证书**”。

如果仍然出现错误，请查看过程和疑难解答部分。 有关详细信息，请参阅[有关使用 Microsoft Intune 解决 SCEP 证书配置文件问题的概述](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)。

**我已将 Wi-Fi 配置文件部署到设备。Intune 显示该操作已成功，但设备却未连接到 Wi-Fi。**

成功状态表示 Intune 已按照配置成功部署了配置文件。 但是，这些配置可能不符合您的网络和/或身份验证要求。 有关尝试的连接的更多详细信息，请查看基础结构和身份验证服务中的日志（在 Wi-Fi 接入点控制器和 NPS/Radius 服务器上）。 你可能需要与网络基础结构团队或第三方 Wi-Fi 供应商合作，以收集和查看日志。