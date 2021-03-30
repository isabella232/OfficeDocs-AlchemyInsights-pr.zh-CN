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
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403792"
---
# <a name="troubleshoot-azure-ad-join-issues"></a><span data-ttu-id="e221a-102">Azure AD 加入问题疑难解答</span><span class="sxs-lookup"><span data-stu-id="e221a-102">Troubleshoot Azure AD join issues</span></span>

1. <span data-ttu-id="e221a-103">如果是首次设置设备注册，请确保已查看 [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) 中的设备管理简介，该简介将指导你如何将控制下的设备获取到 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="e221a-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="e221a-104">如果你直接将设备注册到 Azure AD 中，并注册到 Intune 中，则需要确保你已配置[Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment)并首先获得[](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign)许可。</span><span class="sxs-lookup"><span data-stu-id="e221a-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="e221a-105">确保你有权在 Azure AD 中执行操作。</span><span class="sxs-lookup"><span data-stu-id="e221a-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="e221a-106">只有 Azure AD 中的全局管理员可以管理设备注册的设置。</span><span class="sxs-lookup"><span data-stu-id="e221a-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="e221a-107">若要执行 Azure AD 加入实现，请参阅 [规划 Azure AD 加入](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)。</span><span class="sxs-lookup"><span data-stu-id="e221a-107">To do Azure AD join implementation, see [Plan Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="e221a-108">有关解决 Azure AD 加入常见问题的更多详细信息，请参阅 [Azure Ad Join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) 和 Windows 10 专业版设备，请参阅无法将 Windows 10 专业版计算机加入 Azure [AD - 需要升级到 - Microsoft 社区](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)</span><span class="sxs-lookup"><span data-stu-id="e221a-108">For more details on resolving  common issues with Azure AD join see [Azure Ad Join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)</span></span>
