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
ms.openlocfilehash: 5f95c9bee29db44a4153e0de0b8f6fb49b274920
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716847"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="c2720-102">Apple MDM 推送证书尚未设置</span><span class="sxs-lookup"><span data-stu-id="c2720-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="c2720-103">您的订阅尚未配置 Apple MDM 推送证书（也称为 Apple 推送通知服务 （APNS）证书）。</span><span class="sxs-lookup"><span data-stu-id="c2720-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="c2720-104">如果未配置 Apple MDM 推送证书，则无法注册和管理 iOS 和 MacOS 设备。</span><span class="sxs-lookup"><span data-stu-id="c2720-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="c2720-105">将证书添加到 Intune 后，用户可以安装公司门户应用程序以注册其 iOS 设备。</span><span class="sxs-lookup"><span data-stu-id="c2720-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="c2720-106">选择 **“我同意。”**</span><span class="sxs-lookup"><span data-stu-id="c2720-106">Select **"I agree."**</span></span> <span data-ttu-id="c2720-107">为 Microsoft 授予向 Apple 发送数据的权限。</span><span class="sxs-lookup"><span data-stu-id="c2720-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="c2720-108">选择“**下载 CSR**” 创建 Apple MDM 推送证书所需的 Intune 证书签名请求。</span><span class="sxs-lookup"><span data-stu-id="c2720-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="c2720-109">该文件用于从 Apple 推送证书门户请求信任关系证书。</span><span class="sxs-lookup"><span data-stu-id="c2720-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="c2720-110">选择“**创建你的 MDM 推送证书**”以转到 Apple 推送证书门户。</span><span class="sxs-lookup"><span data-stu-id="c2720-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="c2720-111">使用公司 Apple ID 登录，然后选择“**创建证书**”。</span><span class="sxs-lookup"><span data-stu-id="c2720-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="c2720-112">选择“**选择文件**”，浏览到证书签名请求文件，然后选择“**上传**”。</span><span class="sxs-lookup"><span data-stu-id="c2720-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="c2720-113">在“确认”页面上，选择“**下载**”以下载证书（pem）文件，并将文件保存到本地。</span><span class="sxs-lookup"><span data-stu-id="c2720-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="c2720-114">**注意**：证书与用于创建它的 Apple ID 相关联。</span><span class="sxs-lookup"><span data-stu-id="c2720-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="c2720-115">最佳做法是，使用公司 Apple ID 管理任务，并确保由多个人或使用通讯组列表监视邮箱。</span><span class="sxs-lookup"><span data-stu-id="c2720-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="c2720-116">切勿使用个人 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="c2720-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="c2720-117">使用相同的 Apple ID 每12个月续订一次 Apple 推送证书。</span><span class="sxs-lookup"><span data-stu-id="c2720-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="c2720-118">输入用于创建 Apple MDM 推送证书的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="c2720-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="c2720-119">记录此 ID，以提醒您何时需要更新证书。</span><span class="sxs-lookup"><span data-stu-id="c2720-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="c2720-120">转到证书（.pem）文件，选择“**打开**”，然后选择“**上传**”。</span><span class="sxs-lookup"><span data-stu-id="c2720-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="c2720-121">使用推送证书，Intune 可以注册和管理 Apple 设备。</span><span class="sxs-lookup"><span data-stu-id="c2720-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>