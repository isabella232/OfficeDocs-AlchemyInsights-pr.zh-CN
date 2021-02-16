---
title: 设备写回
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8279"
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2021
ms.locfileid: "50255147"
---
# <a name="device-writeback"></a><span data-ttu-id="02834-102">设备写回</span><span class="sxs-lookup"><span data-stu-id="02834-102">Device Writeback</span></span>

<span data-ttu-id="02834-103">设备写回用于以下方案：</span><span class="sxs-lookup"><span data-stu-id="02834-103">Device Writeback is used in the following scenarios:</span></span>

- <span data-ttu-id="02834-104">使用 [混合证书信任部署启用 Windows Hello 企业应用](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span><span class="sxs-lookup"><span data-stu-id="02834-104">Enable [Windows Hello for Business using hybrid certificate trust deployment](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span></span>
- <span data-ttu-id="02834-105">启用基于设备的条件访问 ADFS (2012 R2 或更高版本) 受信赖方信任 (应用程序) </span><span class="sxs-lookup"><span data-stu-id="02834-105">Enable Conditional Access based on devices to ADFS (2012 R2 or higher) protected applications (relying party trusts)</span></span>

    > [!NOTE]
    > <span data-ttu-id="02834-106">设备写回需要订阅 Azure AD Premium。</span><span class="sxs-lookup"><span data-stu-id="02834-106">A subscription to Azure AD Premium is required for device writeback.</span></span>

<span data-ttu-id="02834-107">这提供额外的安全和保证，即仅向受信任的设备授予对应用程序的访问权限。</span><span class="sxs-lookup"><span data-stu-id="02834-107">This provides additional security and assurance that access to applications is granted only to trusted devices.</span></span> <span data-ttu-id="02834-108">有关条件访问详细信息，请参阅 [使用条件](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) 访问管理风险，以及使用 [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview)设备注册设置本地条件访问。</span><span class="sxs-lookup"><span data-stu-id="02834-108">For more information on Conditional Access, see [Managing Risk with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) and [Setting up On-premises Conditional Access using Azure Active Directory Device Registration](https://docs.microsoft.com/azure/active-directory/devices/overview).</span></span>

<span data-ttu-id="02834-109">有关为设备启用设备写回功能详细信息，请参阅["启用设备写回"。](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)</span><span class="sxs-lookup"><span data-stu-id="02834-109">For more information on Enabling Device Writeback for Devices, see [Enable Device Writeback](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).</span></span>
