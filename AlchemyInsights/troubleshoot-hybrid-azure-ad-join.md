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
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401897"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a><span data-ttu-id="7ffb1-102">混合 Azure AD 加入疑难解答</span><span class="sxs-lookup"><span data-stu-id="7ffb1-102">Troubleshoot Hybrid Azure AD join</span></span>

<span data-ttu-id="7ffb1-103">强烈建议通过使用[测试设备注册连接性脚本](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/)，确保设备可以访问系统账户下的设备注册端点。</span><span class="sxs-lookup"><span data-stu-id="7ffb1-103">Highly Recommended Ensure that a device can access Device Registration endpoints under the system account by using the [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span></span>

1. <span data-ttu-id="7ffb1-104">如果是首次设置设备注册，请务必查看我在 [Azure Active Directory 中设备管理简介](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/)，以了解如何将设备控制在 Azure AD 中。</span><span class="sxs-lookup"><span data-stu-id="7ffb1-104">If you are setting up device registrations for the first time, be sure to review I[ntroduction to device management in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) to learn how to get devices under the control of Azure AD.</span></span>
1. <span data-ttu-id="7ffb1-105">如果要将设备直接注册到 Azure AD 并注册到 Intune 中，请确保已 [配置了 Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) ，并首先拥有 [许可](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) 方案。</span><span class="sxs-lookup"><span data-stu-id="7ffb1-105">If you are registering devices into Azure AD directly and enrolling them into Intune, be sure that you've [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
1. <span data-ttu-id="7ffb1-106">确保有权在 Azure AD 和本地 AD 中执行操作。</span><span class="sxs-lookup"><span data-stu-id="7ffb1-106">Ensure that you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="7ffb1-107">只有 Azure AD 中的全局管理员可管理设备注册的设置。</span><span class="sxs-lookup"><span data-stu-id="7ffb1-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="7ffb1-108">此外，若要在本地 Active Directory 中设置自动注册，需成为 Active Directory 和 AD FS 的管理员 (如果适用)。</span><span class="sxs-lookup"><span data-stu-id="7ffb1-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="7ffb1-109">有关解决混合加入的潜在问题的详细信息，请参阅 [混合联接疑难解答](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) 以设置加入的混合 Azure AD 以及使用 Azure Ad 门户管理设备，请参阅 [设置加入已建立混合 Azure AD (本地域加入) 联接](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) 和 [使用 Azure 门户管理设备](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="7ffb1-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see [Set up hybrid Azure AD joined (on-premises domain-joined) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and [Manage devices using the Azure portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="7ffb1-110">若要解决混合 Azure Active Directory（AD）加入的常见问题，请参阅 [混合 Azure AD 加入的常见问题](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq)。</span><span class="sxs-lookup"><span data-stu-id="7ffb1-110">To resolve common issues with Hybrid Azure Active Directory (AD) join, see [Hybrid Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span></span>
