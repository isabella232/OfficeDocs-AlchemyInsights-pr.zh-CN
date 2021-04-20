---
title: Teams 教育版客户常见问题
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000701"
- "3831"
- "3832"
ms.openlocfilehash: 6d1fac07673f6f945f382e4e640cf44afb76717d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51829438"
---
# <a name="teams-common-issues-for-education-customers"></a>Teams 教育版客户常见问题

**教育版客户**：

如果在部署 Teams 以支持远程教育时需要帮助，请访问 [FastTrack 中心](https://www.microsoft.com/fasttrack)提交请求。 请参阅以下面向 Teams 教育版客户的常见问题：

- 看到“**You're missing out!**”消息？ 确保“[为学校启用 Microsoft Teams](https://docs.microsoft.com/microsoft-365/education/intune-edu-trial/enable-microsoft-teams)”。 在 EDU 租户中，默认情况下不启用 Microsoft Teams ，必须首先将其打开。

- **不熟悉 Teams？** 请参阅[使用 Office 365 教育版远程教学](https://support.office.com/article/remote-teaching-and-learning-in-office-365-education-f651ccae-7b65-478b-8366-51bb884025c4)，了解如何设置学校、课程规划、虚拟会议和与学生共享内容。

- 启用后，用户可以通过安装[桌面版](https://docs.microsoft.com/MicrosoftTeams/get-clients#desktop-client)和[移动版客户端](https://docs.microsoft.com/MicrosoftTeams/get-clients#mobile-clients)或从 https://teams.microsoft.com 处的浏览器运行 Teams。

- **启用 Teams 来宾访问**：查看“[Teams 来宾访问检查清单](https://docs.microsoft.com/microsoftteams/guest-access-checklist)”并确保所有步骤已完成。
    - [了解 Microsoft Teams 中的来宾访问](https://docs.microsoft.com/microsoftteams/guest-access)
    - [设置 - Microsoft Teams 来宾访问清单](https://docs.microsoft.com/microsoftteams/guest-access-checklist)
    - [来宾加入团队的方式](https://docs.microsoft.com/microsoftteams/guest-joins)

- **Teams 会议和拨入**：在启用或设置 Microsoft Teams 中的音频会议方面需要帮助？ 此用户最近已创建？ 如果是这样，则需要等待 2–24小时，设置才会生效。 若要验证用户是否获得音频会议许可，是否拥有默认收费电话号码：
    1. 转到“活动用户”，随后选择有问题的用户。
    2. 根据管理中心的版本，选择“**许可证和应用程序**”或点击“**产品许可证**”上的“**编辑**”。
    3. 确认用户已选择了适用于音频会议、Microsoft Teams、Skype for Business Online (计划 2) 的许可证。
    4. 用户“管理中心”单击“**显示全部**”，并随后单击 **Teams**。
    5. 在“Microsoft Teams 管理中心”，单击“**旧门户**”。
    6. 在“Skype for Business 管理中心”中，单击“**音频会议**”，然后单击“**用户**”。
    7. 选择有问题的用户，并验证用户是否有“默认收费号码”。

    有关详细信息，请参阅[Microsoft Teams 通话套餐](https://docs.microsoft.com/microsoftteams/calling-plans-for-office-365)，或致电 Microsoft Commerce Billing 团队来获取授权相关问题的帮助。

    其他资源

    - [Microsoft Teams 中的会议](https://docs.microsoft.com/microsoftteams/deploy-meetings-microsoft-teams-landing-page)
    - [音频会议](https://docs.microsoft.com/microsoftteams/audio-conferencing-in-office-365)

- **会议策略**：会议策略用于控制组织中用户安排的会议的与会者可用的功能。 创建策略并进行更改后，即可以将用户分配到策略。

    - **更改或创建会议策略**：若要更改或创建会议策略，请转到 **Microsoft Teams 管理中心 > 会议 > 会议策略**。 从列表中选择一个策略，或者单击“**添加**”。 如果正在创建新策略，则添加名称和说明。 名称不能包含特殊字符或超过 64 个字符。 选择设置，然后单击“**保存**”。 
    
        例如，假设你有一组用户并且你想要限制这组用户的会议所需的带宽。 你要创建新的自定义策略并命名为“带宽限制”，然后禁用以下设置：

        在“**音频和视频**”中：
        - 禁用“**允许云录制**”。
        - 禁用“**允许 IP 视频**”。

        在“**内容共享**”下：

        - 禁用屏幕共享模式。
        - 禁用“**允许白板**”。
        - 禁用“**允许共享笔记**”。

        然后 **将此策略分配给用户**：

    1. 在 Microsoft Teams 管理员中心的左侧导航中，转到“**用户**”，然后单击相应的用户。
    2. 单击用户名的左侧以选择用户，然后单击“**编辑设置**”。
    3. 在“**会议策略**”下，选择想要分配的策略，然后单击“**应用**”。

    若要将策略一次性分配给多个用户，请参阅[批量编辑 Teams 用户设置](https://docs.microsoft.com/microsoftteams/edit-user-settings-in-bulk)。

    或者可以执行以下操作：
    1. 在 Microsoft Teams 管理员中心的左侧导航中，转到“**会议 > 会议策略**”。
    2. 单击策略名称的左侧以选择该策略。
    3. 单击“**管理用户**”。
    4. 在“**管理用户**”窗格中，按显示名称或用户名搜索用户，选择用户名，然后单击“**添加**”。 对想要添加的每一个用户重复此步骤。
    5. 添加用户完成之后，单击“**保存**”。

- **拨号盘缺失故障排除**：
    - 确保用户已分配了[Teams 许可证](https://docs.microsoft.com/MicrosoftTeams/assign-teams-licenses)。
    - 确保用户已分配了[通话套餐](https://docs.microsoft.com/MicrosoftTeams/calling-plan-landing-page)。
    - 为用户启用[企业语音](https://docs.microsoft.com/skypeforbusiness/skype-for-business-hybrid-solutions/plan-your-phone-system-cloud-pbx-solution/enable-users-for-enterprise-voice-online-and-phone-system-voicemail#to-enable-your-users-for-phone-system-in-office-365-voice-and-voicemail)。

- **Teams 登录问题故障排查**：首先，确保 [Microsoft Teams 服务正常](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/servicehealth)。 然后检查是否存在任何常见错误代码，并查阅[登录到 Microsoft Teams 时为何会遇到问题](https://support.office.com/article/a02f683b-61a3-4008-9447-ee60c5593b0f)？ 还需要查看 [Microsoft Teams 中的身份模型和身份验证](https://docs.microsoft.com/MicrosoftTeams/identify-models-authentication)。
