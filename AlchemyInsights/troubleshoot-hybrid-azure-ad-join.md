---
title: 混合 Azure AD 加入疑难解答
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 23da360965a5972e328844d505698c91ece61788240d8fdb8909fff3a7ef0d7f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939261"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>混合 Azure AD 加入疑难解答

强烈建议通过使用[测试设备注册连接性脚本](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/)，确保设备可以访问系统账户下的设备注册端点。

1. 如果是首次设置设备注册，请务必查看我在 [Azure Active Directory 中设备管理简介](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/)，以了解如何将设备控制在 Azure AD 中。
1. 如果要将设备直接注册到 Azure AD 并注册到 Intune 中，请确保已 [配置了 Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) ，并首先拥有 [许可](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) 方案。
1. 确保有权在 Azure AD 和本地 AD 中执行操作。 只有 Azure AD 中的全局管理员可管理设备注册的设置。 此外，若要在本地 Active Directory 中设置自动注册，需成为 Active Directory 和 AD FS 的管理员 (如果适用)。

有关解决混合加入的潜在问题的详细信息，请参阅 [混合联接疑难解答](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) 以设置加入的混合 Azure AD 以及使用 Azure Ad 门户管理设备，请参阅 [设置加入已建立混合 Azure AD (本地域加入) 联接](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) 和 [使用 Azure 门户管理设备](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)。

若要解决混合 Azure Active Directory（AD）加入的常见问题，请参阅 [混合 Azure AD 加入的常见问题](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq)。
