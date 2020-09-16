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
ms.openlocfilehash: 9dbb88492a3906f6780a345cf880327d411dcc66
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709717"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="af387-102">启用 Azure AD Connect 中的密码写回</span><span class="sxs-lookup"><span data-stu-id="af387-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="af387-103">若要启用自助服务密码重置写回，请首先在 Azure AD Connect 中启用写回选项。</span><span class="sxs-lookup"><span data-stu-id="af387-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="af387-104">在 Azure AD Connect 服务器中，完成以下步骤：</span><span class="sxs-lookup"><span data-stu-id="af387-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="af387-105">登录 Azure AD Connect 服务器，然后启动 **Azure AD Connect** 配置向导。</span><span class="sxs-lookup"><span data-stu-id="af387-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="af387-106">在“**欢迎**”页上，单击“**配置**”。</span><span class="sxs-lookup"><span data-stu-id="af387-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="af387-107">在“**其他任务**”页上，选择“**自定义同步选项**”，然后单击“**下一步**”。</span><span class="sxs-lookup"><span data-stu-id="af387-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="af387-108">在“**连接到 Azure AD**”页面上，输入全局管理员凭据，然后单击“下一步”。</span><span class="sxs-lookup"><span data-stu-id="af387-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click Next.</span></span>
5. <span data-ttu-id="af387-109">在“**连接到目录**”和“**域/OU**”筛选页上，单击“**下一步**”。</span><span class="sxs-lookup"><span data-stu-id="af387-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="af387-110">在“**可选功能**”页上，选中“**密码写回**”旁边的框，然后单击“**下一步**”。</span><span class="sxs-lookup"><span data-stu-id="af387-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="af387-111">在“**准备配置**”页上，单击“**配置**”并等待该过程完成。</span><span class="sxs-lookup"><span data-stu-id="af387-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="af387-112">当看到配置完成后，单击“**退出**”。</span><span class="sxs-lookup"><span data-stu-id="af387-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="af387-113">在 Azure AD Connect 中启用密码写回后，现在配置用于写回的 Azure AD SSPR。</span><span class="sxs-lookup"><span data-stu-id="af387-113">With password writeback enabled in Azure AD Connect, now configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="af387-114">若要在 SSPR 中启用密码写回，请完成以下步骤：</span><span class="sxs-lookup"><span data-stu-id="af387-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="af387-115">使用全局管理员帐户登录到 Azure 门户。</span><span class="sxs-lookup"><span data-stu-id="af387-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="af387-116">搜索并选择 **Azure Active Directory**，单击“**密码重置**”，然后选择“**本地集成**”。</span><span class="sxs-lookup"><span data-stu-id="af387-116">Search for and select **Azure Active Directory**, click **Password reset**, then choose **On-premises integration**.</span></span>
3. <span data-ttu-id="af387-117">把选项“**将密码回写到本地目录？**”设置为“**是**”。</span><span class="sxs-lookup"><span data-stu-id="af387-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="af387-118">将“**允许用户在不重置密码的情况下解锁帐户**”选项设置为“**是**”。</span><span class="sxs-lookup"><span data-stu-id="af387-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="af387-119">准备好后，单击“**保存**”。</span><span class="sxs-lookup"><span data-stu-id="af387-119">When ready, click **Save**.</span></span>

<span data-ttu-id="af387-120">有关详细信息，请参阅“[对本地环境启用 Azure Active Directory 自助服务密码重置写回](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)”。</span><span class="sxs-lookup"><span data-stu-id="af387-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>
