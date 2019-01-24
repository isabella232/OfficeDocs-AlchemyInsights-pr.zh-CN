---
title: 902 （重复对象由于同步错误）
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f8db233167a5e2b2ef7290438b8e6d92d0dccb1e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29459893"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="d2984-102">由于重复的对象的同步错误</span><span class="sxs-lookup"><span data-stu-id="d2984-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="d2984-103">目录同步完成后，您可能收到以下错误消息之一：</span><span class="sxs-lookup"><span data-stu-id="d2984-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>
  
- <span data-ttu-id="d2984-104">无法更新此 Microsoft Online Services 中的对象，因为此对象相关联的以下属性具有已可能与本地目录中的其他对象相关联的值。</span><span class="sxs-lookup"><span data-stu-id="d2984-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>
    
- <span data-ttu-id="d2984-105">Microsoft Online Services 目录中已存在具有相同的代理地址同步的对象。</span><span class="sxs-lookup"><span data-stu-id="d2984-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>
    
- <span data-ttu-id="d2984-106">无法更新此对象，因为此对象相关联的以下属性具有已可能与您的本地目录服务中的其他对象相关联的值： UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="d2984-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>
    
<span data-ttu-id="d2984-107">要找出并修复问题，请下载并运行[IdFix 目录同步错误修复工具](https://www.microsoft.com/download/details.aspx?id=36832)。</span><span class="sxs-lookup"><span data-stu-id="d2984-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>
  
<span data-ttu-id="d2984-108">有关详细信息，请参阅[KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)。</span><span class="sxs-lookup"><span data-stu-id="d2984-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
  

