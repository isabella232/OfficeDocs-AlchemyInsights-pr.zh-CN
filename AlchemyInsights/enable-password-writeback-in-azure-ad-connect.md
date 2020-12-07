---
title: 启用 Azure AD Connect 中的密码写回
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 0eecd89b2558359702935379d7ffbd8b7508f4cd
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/02/2020
ms.locfileid: "49560430"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="bdab0-102">启用 Azure AD Connect 中的密码写回</span><span class="sxs-lookup"><span data-stu-id="bdab0-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="bdab0-103">若要启用自助服务密码重置写回，请首先在 Azure AD Connect 中启用写回选项。</span><span class="sxs-lookup"><span data-stu-id="bdab0-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="bdab0-104">在 Azure AD Connect 服务器中，完成以下步骤：</span><span class="sxs-lookup"><span data-stu-id="bdab0-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="bdab0-105">登录 Azure AD Connect 服务器，然后启动 **Azure AD Connect** 配置向导。</span><span class="sxs-lookup"><span data-stu-id="bdab0-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="bdab0-106">在“**欢迎**”页上，单击“**配置**”。</span><span class="sxs-lookup"><span data-stu-id="bdab0-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="bdab0-107">在“**其他任务**”页上，选择“**自定义同步选项**”，然后单击“**下一步**”。</span><span class="sxs-lookup"><span data-stu-id="bdab0-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="bdab0-108">在“连接到 Azure AD”页面上，输入全局管理员凭据，然后单击“下一步”。</span><span class="sxs-lookup"><span data-stu-id="bdab0-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="bdab0-109">在“**连接到目录**”和“**域/OU**”筛选页上，单击“**下一步**”。</span><span class="sxs-lookup"><span data-stu-id="bdab0-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="bdab0-110">在“**可选功能**”页上，选中“**密码写回**”旁边的框，然后单击“**下一步**”。</span><span class="sxs-lookup"><span data-stu-id="bdab0-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="bdab0-111">在“**准备配置**”页上，单击“**配置**”并等待该过程完成。</span><span class="sxs-lookup"><span data-stu-id="bdab0-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="bdab0-112">当看到配置完成后，单击“**退出**”。</span><span class="sxs-lookup"><span data-stu-id="bdab0-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="bdab0-113">在 Azure AD Connect 中启用密码写回后，现在配置用于写回的 Azure AD SSPR。</span><span class="sxs-lookup"><span data-stu-id="bdab0-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="bdab0-114">若要在 SSPR 中启用密码写回，请完成以下步骤：</span><span class="sxs-lookup"><span data-stu-id="bdab0-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="bdab0-115">使用全局管理员帐户登录到 Azure 门户。</span><span class="sxs-lookup"><span data-stu-id="bdab0-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="bdab0-116">搜索并选择 **Azure Active Directory**，单击“**密码重置**”，然后选择“**本地集成**”。</span><span class="sxs-lookup"><span data-stu-id="bdab0-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="bdab0-117">把选项“**将密码回写到本地目录？**”设置为“**是**”。</span><span class="sxs-lookup"><span data-stu-id="bdab0-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="bdab0-118">将“**允许用户在不重置密码的情况下解锁帐户**”选项设置为“**是**”。</span><span class="sxs-lookup"><span data-stu-id="bdab0-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="bdab0-119">准备好后，单击“**保存**”。</span><span class="sxs-lookup"><span data-stu-id="bdab0-119">When ready, click **Save**.</span></span>

<span data-ttu-id="bdab0-120">有关详细信息，请参阅“[对本地环境启用 Azure Active Directory 自助服务密码重置写回](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)”。</span><span class="sxs-lookup"><span data-stu-id="bdab0-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="bdab0-121">当管理员在 Azure 门户中重置用户密码时，如果该用户是联盟用户或其密码哈希已同步，则该密码将回写到本地。</span><span class="sxs-lookup"><span data-stu-id="bdab0-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="bdab0-122">Office 管理门户当前不支持此功能。</span><span class="sxs-lookup"><span data-stu-id="bdab0-122">This functionality is currently not supported in the Office Admin portal.</span></span>