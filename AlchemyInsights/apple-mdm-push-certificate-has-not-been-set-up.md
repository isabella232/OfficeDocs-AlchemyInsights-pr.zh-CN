---
title: Apple MDM 推送证书尚未设置
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 4f8e3502a7be35b5579ec1436852fe2bff9b1316891c7a9020f6f5f4767b3d88
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931515"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Apple MDM 推送证书尚未设置

您的订阅尚未配置 Apple MDM 推送证书（也称为 Apple 推送通知服务 （APNS）证书）。 如果未配置 Apple MDM 推送证书，则无法注册和管理 iOS 和 MacOS 设备。 将证书添加到 Intune 后，用户可以安装公司门户应用程序以注册其 iOS 设备。

1. 选择 **“我同意。”** 为 Microsoft 授予向 Apple 发送数据的权限。

2. 选择“**下载 CSR**” 创建 Apple MDM 推送证书所需的 Intune 证书签名请求。 该文件用于从 Apple 推送证书门户请求信任关系证书。

3. 选择“**创建你的 MDM 推送证书**”以转到 Apple 推送证书门户。 使用公司 Apple ID 登录，然后选择“**创建证书**”。 选择“**选择文件**”，浏览到证书签名请求文件，然后选择“**上传**”。 在“确认”页面上，选择“**下载**”以下载证书（pem）文件，并将文件保存到本地。
 
**注意**：证书与用于创建它的 Apple ID 相关联。 最佳做法是，使用公司 Apple ID 管理任务，并确保由多个人或使用通讯组列表监视邮箱。 切勿使用个人 Apple ID。 使用相同的 Apple ID 每12个月续订一次 Apple 推送证书。
 
4. 输入用于创建 Apple MDM 推送证书的 Apple ID。 记录此 ID，以提醒您何时需要更新证书。

5. 转到证书（.pem）文件，选择“**打开**”，然后选择“**上传**”。 使用推送证书，Intune 可以注册和管理 Apple 设备。