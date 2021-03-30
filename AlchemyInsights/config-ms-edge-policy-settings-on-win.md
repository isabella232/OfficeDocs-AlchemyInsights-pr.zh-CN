---
title: 在 Windows 上配置 Microsoft Edge 策略设置
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003845"
- "9004632"
- "6894"
- "8358"
ms.openlocfilehash: e9bb489b4d8ecd76fd777ade9fb740ecad542900
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402365"
---
# <a name="configure-microsoft-edge-policy-settings-on-windows"></a><span data-ttu-id="9c6e7-102">在 Windows 上配置 Microsoft Edge 策略设置</span><span class="sxs-lookup"><span data-stu-id="9c6e7-102">Configure Microsoft Edge policy settings on Windows</span></span>

<span data-ttu-id="9c6e7-103">若要为 Microsoft Edge 配置策略设置和托管更新，请使用组策略对象 (GPO) 。</span><span class="sxs-lookup"><span data-stu-id="9c6e7-103">To configure policy settings and managed updates for Microsoft Edge, use Group Policy Objects (GPOs).</span></span> <span data-ttu-id="9c6e7-104">您还可以通过注册表设置策略;这适用于加入 Microsoft Active Directory 域的 (1) Windows 设备，以及注册在 Microsoft Intune 中管理设备的 (2) Windows 10 专业版和企业版实例。</span><span class="sxs-lookup"><span data-stu-id="9c6e7-104">You can also provision policy through the registry; this would be appropriate for (1) Windows devices joined to a Microsoft Active Directory domain and for (2) Windows 10 Pro and Enterprise instances enrolled for device management in Microsoft Intune.</span></span>

<span data-ttu-id="9c6e7-105">若要使用 GPO 配置 Microsoft Edge，请执行下列操作：</span><span class="sxs-lookup"><span data-stu-id="9c6e7-105">To configure Microsoft Edge by using GPOs, do the following:</span></span>

1. <span data-ttu-id="9c6e7-106">Go to the Group Policy Central Store in your Active Directory domain， or to the Policy Definition template folder on individual computers， install all administrative templates that add rules and settings for Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="9c6e7-106">Go to the Group Policy Central Store in your Active Directory domain, or to the Policy Definition template folder on individual computers, install all administrative templates that add rules and settings for Microsoft Edge.</span></span>
2. <span data-ttu-id="9c6e7-107">配置要设置的特定策略。</span><span class="sxs-lookup"><span data-stu-id="9c6e7-107">Configure the specific policies you want to set.</span></span>

<span data-ttu-id="9c6e7-108">若要了解更多信息，请参阅在 Windows 上 [配置 Microsoft Edge 策略设置](https://go.microsoft.com/fwlink/?linkid=2135024)。</span><span class="sxs-lookup"><span data-stu-id="9c6e7-108">To learn more, see [Configure Microsoft Edge policy settings on Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span></span>
