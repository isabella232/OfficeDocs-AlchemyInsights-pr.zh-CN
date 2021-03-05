---
title: 密码同步
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50449056"
---
# <a name="password-synchronization"></a><span data-ttu-id="39eb6-102">密码同步</span><span class="sxs-lookup"><span data-stu-id="39eb6-102">Password synchronization</span></span>

<span data-ttu-id="39eb6-103">**密码哈希同步完全不起作用**</span><span class="sxs-lookup"><span data-stu-id="39eb6-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="39eb6-104">密码哈希同步不起作用时客户遇到的一些常见问题包括：</span><span class="sxs-lookup"><span data-stu-id="39eb6-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="39eb6-105">Azure AD Connect 用于与本地 Active Directory 进行通信的 Active Directory帐户不会被授予复制目录更改和复制目录更改所有权限，密码同步需要这些权限 - 你需要通过向 Active Directory 帐户授予这些权限来解决此问题。</span><span class="sxs-lookup"><span data-stu-id="39eb6-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="39eb6-106">在管理员将用户 Sign-In 方法从密码同步更改为其他选项（如Azure AD Connect 向导中的 **AD FS** 联盟）后，密码哈希同步被禁用 - 可以通过在Azure AD Connect 向导中重新启用密码哈希同步功能来解决此问题。</span><span class="sxs-lookup"><span data-stu-id="39eb6-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="39eb6-107">本地 Active Directory 的连接问题。</span><span class="sxs-lookup"><span data-stu-id="39eb6-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="39eb6-108">例如，Azure AD Connect 无法访问某些域控制器，或者所需的端口被防火墙[](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports)阻止 - 你需要通过确保 Azure AD Connect 服务器和本地 Active Directory 之间的连接正常工作来解决此问题。</span><span class="sxs-lookup"><span data-stu-id="39eb6-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="39eb6-109">Azure AD Connect 服务器当前处于暂存模式，这可能会导致服务器无法执行密码哈希 - 若要解决问题，请按照"Azure [AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)同步密码同步疑难解答"一节中介绍的步骤操作 - 不同步密码。</span><span class="sxs-lookup"><span data-stu-id="39eb6-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="39eb6-110">**密码哈希同步对部分用户不起作用**</span><span class="sxs-lookup"><span data-stu-id="39eb6-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="39eb6-111">如果你注意到用户未同步密码哈希，请使用 Azure AD Connect中的疑难解答任务来调查和解决问题。</span><span class="sxs-lookup"><span data-stu-id="39eb6-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="39eb6-112">执行以下任务：</span><span class="sxs-lookup"><span data-stu-id="39eb6-112">Perform the following tasks:</span></span>

    <span data-ttu-id="39eb6-113">a.</span><span class="sxs-lookup"><span data-stu-id="39eb6-113">a.</span></span> [<span data-ttu-id="39eb6-114">在向导中运行疑难解答任务</span><span class="sxs-lookup"><span data-stu-id="39eb6-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="39eb6-115">b.</span><span class="sxs-lookup"><span data-stu-id="39eb6-115">b.</span></span> [<span data-ttu-id="39eb6-116">使用疑难解答 cmdlet 调查特定用途的密码哈希同步问题</span><span class="sxs-lookup"><span data-stu-id="39eb6-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="39eb6-117">为用户启用本地 Active Directory 用户对象必须在下一次 **登录选项时更改** 密码。</span><span class="sxs-lookup"><span data-stu-id="39eb6-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="39eb6-118">启用此选项后，将为用户分配一个临时密码，并提示用户在下次登录时更改密码。</span><span class="sxs-lookup"><span data-stu-id="39eb6-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="39eb6-119">Azure AD Connect 不会将临时密码同步到 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="39eb6-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="39eb6-120">若要解决上述问题，请执行以下任一任务：</span><span class="sxs-lookup"><span data-stu-id="39eb6-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="39eb6-121">要求用户登录到本地应用程序 (例如，Windows 桌面) 更改密码。</span><span class="sxs-lookup"><span data-stu-id="39eb6-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="39eb6-122">新密码将同步到 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="39eb6-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="39eb6-123">让管理员更新用户密码，而不启用"用户下次登录时必须更改密码"选项，并与用户共享新密码。</span><span class="sxs-lookup"><span data-stu-id="39eb6-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="39eb6-124">未正确为对象同步或密码同步配置本地Active Directory 用户对象。</span><span class="sxs-lookup"><span data-stu-id="39eb6-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="39eb6-125">若要解决此问题，请按照 Azure AD Connect 同步的密码哈希同步疑难解答 [中所述的步骤操作](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)。</span><span class="sxs-lookup"><span data-stu-id="39eb6-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







