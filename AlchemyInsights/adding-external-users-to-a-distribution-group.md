---
title: 将外部用户添加到通讯组
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: d8c06c81ecc66df0fbaa4cac9908178cdc1d9c6bdc38d19010c7b55e9bca8776
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934823"
---
# <a name="add-external-users-to-a-distribution-group"></a>将外部用户添加到通讯组

将外部联系人添加到通讯组 (DG) 过程包括两个步骤：
  
1. 为外部用户创建邮件联系人：
    
    1. 在管理中心，转到"**用户**  >  [联系人"](https://admin.microsoft.com/adminportal/home#/Contact)页面。 
    
    2. 选择 **"添加联系人"。**
    
    3. 键入联系人的信息，然后选择"添加 **"。**
    
2. 将邮件联系人添加到 DG：
    
    1. 在管理中心，转到组  >  [组](https://admin.microsoft.com/adminportal/home#/groups)页面。 
    
    2. 找到要添加外部用户的 DG，然后选择它以打开编辑对话框。
    
    3. 在"**成员"** 选项卡上，**选择"查看所有和管理成员"。** 
    
    4. 选择“**添加成员**”。
    
    5. 选择在上一步中创建的邮件联系人，**然后选择保存。**
    
如果执行这些步骤后，外部用户无法向 DG 发送电子邮件或没有收到来自 DG 的电子邮件，可能是 DG 被标记为仅允许来自内部用户的电子邮件。 你可以检查此配置，并按照此处说明 [进行修复](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)。
  
 **注意：** 如果你的组类型是"Microsoft 365组"而不是"通讯组"，则这些说明不适用。 如果是这种情况，你可以直接从组中添加外部用户Outlook。 有关"Microsoft 365组来宾的详细信息以及添加外部来宾的说明，请参阅[本文](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)。
  