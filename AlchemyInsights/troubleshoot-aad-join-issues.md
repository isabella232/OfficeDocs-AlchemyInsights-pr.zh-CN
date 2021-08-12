---
title: Azure AD 加入问题疑难解答
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 8e902aea30e6891717e08027cc009576d390c9cf2ba1649cbbc68d64883937f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939909"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Azure AD 加入问题疑难解答

1. 如果是首次设置设备注册，请确保已查看 Azure Active Directory 中的设备管理简介[，](https://docs.microsoft.com/azure/active-directory/devices/overview)该简介将指导你如何将控制下的设备获取到 Azure AD。 
1. 如果你直接将设备注册到 Azure AD 中，并注册到 Intune 中，则需要确保你已配置[Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment)并首先获得[](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign)许可。
1. 确保你有权在 Azure AD 中执行操作。 只有 Azure AD 中的全局管理员可管理设备注册的设置。
1. 若要执行 Azure AD 加入实现，请参阅 [规划 Azure AD 加入](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)。

有关解决 Azure AD 加入常见问题的更多详细信息，请参阅[Azure Ad Join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq)和 Windows 10 pro 设备，请参阅无法将 Windows 10 专业版 计算机加入 Azure [AD - 需要](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)升级到 - Microsoft Community
