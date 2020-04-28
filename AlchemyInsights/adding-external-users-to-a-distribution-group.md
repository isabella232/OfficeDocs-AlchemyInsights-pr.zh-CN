---
title: 向通讯组添加外部用户
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910922"
---
# <a name="add-external-users-to-a-distribution-group"></a>将外部用户添加到通讯组

向通讯组添加外部联系人（DG）的过程分为两个步骤：
  
1. 为外部用户创建邮件联系人：
    
    1. 在管理中心中，转到 "**用户** > [联系人](https://admin.microsoft.com/adminportal/home#/Contact)" 页。 
    
    2. 选择 "**添加联系人**"。
    
    3. 键入您的联系人的信息，然后选择 "**添加**"。
    
2. 将邮件联系人添加到你的 DG：
    
    1. 在 "管理中心" 中，转到 "**组** > [组](https://admin.microsoft.com/adminportal/home#/groups)" 页面。 
    
    2. 找到要向其添加外部用户的 DG，然后选择该 DG 以打开 "编辑" 对话框。
    
    3. 在 "**成员**" 选项卡上，选择 "**查看所有和管理成员**"。 
    
    4. 选择“**添加成员**”。
    
    5. 选择您在上一步中创建的邮件联系人，然后选择 "**保存**"。
    
如果执行这些步骤后，你的外部用户无法向 DG 发送电子邮件或不接收来自该 DG 的电子邮件，则可能会将此 DG 标记为仅允许来自内部用户的电子邮件。 您可以查看此配置并按照[此处](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)的说明进行修复。
  
 **注意：** 如果您的组的类型是 "Microsoft 365 组" 而不是 "通讯组"，则不适用这些说明。 如果是这种情况，则可以将外部用户直接添加到 Outlook 中的组。 有关 Microsoft 365 组来宾的详细信息，以及有关如何添加外部来宾的说明，请参阅[本文](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)。
  