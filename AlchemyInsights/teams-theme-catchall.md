---
title: 团队主题容器
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2605"
- "9000701"
ms.openlocfilehash: 47e9aa76f8624ce3ddf4cfd03637b5b2714eb435
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030390"
---
# <a name="teams-common-issues-and-resolutions"></a>Teams 常见问题和解决方法

**重要信息**：由于最近 Teams 使用量增加，当向用户分配 Teams 许可证时，可能需要大约 24 小时才能完全设置。 在此之前，将无法为他们分配团队策略，并且可能无法访问某些团队功能，例如呼叫和音频会议。

**常见问题和解决方法**

若要获得更具体的答案，请尝试重新撰写你的问题，包括看到的任何错误或正在使用的 Teams 功能。

如果因为新型冠状病毒肺炎（COVID-19）需要帮助部署 Teams 以支持远程工作者，请参阅“[使用 Microsoft Teams 支持远程工作者](https://docs.microsoft.com/microsoftteams/support-remote-work-with-teams)”。 此外，还有资格获得 Microsoft 365 FastTrack 程序的部署帮助，具体请访问 [FastTrack 中心](https://www.microsoft.com/fasttrack)提交请求。

所有 Teams 客户：

- **不熟悉 Teams？** 请参阅“[Microsoft Teams 入门指南](https://docs.microsoft.com/microsoftteams/get-started-with-teams-quick-start)”。
- **启用 Teams 来宾访问：** 查看“[Teams 来宾访问检查清单](https://docs.microsoft.com/microsoftteams/guest-access-checklist)”并确保所有步骤已完成。 其他资源：
    - [了解 Microsoft Teams 中的来宾访问](https://docs.microsoft.com/microsoftteams/guest-access)
    - [设置 - Microsoft Teams 来宾访问清单](https://docs.microsoft.com/microsoftteams/guest-access-checklist)
    - [来宾加入团队的方式](https://docs.microsoft.com/microsoftteams/guest-joins)

- **Teams 会议和拨入**：在启用或设置 Microsoft Teams 中的音频会议方面需要帮助？ 此用户最近已创建？ 如果是这样，则需要等待 2–24小时，**设置才会生效**。 

    若要验证用户是否获得音频会议许可，是否拥有默认收费电话号码：
    1.    转到“活动用户”，并随后选择有问题的用户。
    2.    根据管理中心的版本，选择“**许可证和应用程序**”或点击“**产品许可证**”上的“**编辑**”。
    3.    确认用户已选择了适用于音频会议、Microsoft Teams、Skype for Business Online (计划 2) 的许可证。
    4.    用户“管理中心”单击“**显示全部**”，并随后单击 **Teams**。
    5.    在“Microsoft Teams 管理中心”，单击“**旧门户**”。
    6.    在“Skype for Business 管理中心”中，单击“**音频会议**”，然后单击“**用户**”。
    7.    选择有问题的用户，并验证用户是否有“默认收费号码”。
    
    有关详细信息，请参阅 [Office 365 通话套餐](https://docs.microsoft.com/microsoftteams/calling-plans-for-office-365)或致电 Microsoft Commerce 计费团队来获取授权相关问题的帮助。

    其他资源：

    - [Microsoft Teams 中的会议](https://docs.microsoft.com/microsoftteams/deploy-meetings-microsoft-teams-landing-page)
    - [Office 365 中的音频会议](https://docs.microsoft.com/microsoftteams/audio-conferencing-in-office-365)

- **Teams Exploratory 许可证**：借助 Microsoft Teams Exploratory 体验，组织中拥有 Azure Active Directory (AAD) 且未获得 Teams 许可的用户可以启用 Teams 的探索体验。 管理员可以为组织中的用户打开或关闭此功能。 以前的 [Microsoft 商业云试用版](https://docs.microsoft.com/microsoftteams/iw-trial-teams)现在替换为 Teams Exploratory 体验。

    其他资源：

    - [如何注册 Teams Exploratory 体验？](https://docs.microsoft.com/microsoftteams/teams-exploratory#how-users-sign-up-for-the-teams-exploratory-experience)
    - [管理 Teams Exploratory 体验](https://docs.microsoft.com/microsoftteams/teams-exploratory#manage-the-teams-exploratory-experience)

- **专用频道**：Microsoft Teams 专用频道创建专用空间供团队展开协作。 仅属于专用渠道的所有者或成员的团队用户可以访问此渠道。 只要已是团队的成员（包括来宾），均可将其添加为专用渠道的成员。

    如果想要将协作限制为有知情需求的人员之间，或者想要促进分配到特定项目的一组人员之间的通信，你可能会需要使用专用渠道，而不必创建额外的团队并进行管理。

    其他资源：
    - [专用渠道创建和成员资格](https://docs.microsoft.com/microsoftteams/private-channels#private-channel-creation-and-membership)
    - [管理专用渠道成员资格和设置](https://docs.microsoft.com/microsoftteams/private-channels#manage-private-channel-membership-and-settings)

- **会议策略**：会议策略用于控制组织中用户安排的会议的与会者可用的功能。 创建策略并进行更改后，即可以将用户分配到策略。 
    - **更改或创建会议策略**：若要更改或创建会议策略，请转到“Microsoft Teams 管理中心 > 会议 > 会议策略”。**** 从列表中选择一个策略，或者选择“添加”。 若正在创建新策略，则添加名称和说明。 名称不能包含特殊字符或超过 64 个字符。 选择设置，然后单击“保存”****。

        例如，假设你有一组用户并且你想要限制这组用户的会议所需的带宽量。 你要创建新的自定义策略并命名为“带宽限制”，然后禁用以下设置：

        在“音频和视频”中：****
        - 禁用“允许云录制”。
        - 禁用“允许 IP 视频”。

        在“内容共享”中：****
        - 禁用屏幕共享模式。
        - 禁用“允许白板”。
        - 禁用“允许共享笔记”。

        然后将此策略分配给用户。

- **将会议策略分配给用户**

    1. 在 Microsoft Teams 管理员中心的左侧导航中，转到“用户”，然后单击相应的用户。****
    2. 单击用户名的左侧以选择用户，然后单击“编辑设置”。****
    3. 在“会议策略”中，选择想要分配的策略，然后单击“应用”。********

    若要将策略一次性分配给多个用户，请参阅[批量编辑 Teams 用户设置](https://docs.microsoft.com/microsoftteams/edit-user-settings-in-bulk)。 或者可以执行以下操作：

    1. 在 Microsoft Teams 管理员中心的左侧导航中，转到“**会议 > 会议策略**”。
    2. 单击策略名称的左侧以选择该策略。
    3. 选择“管理用户”****。
    4. 在“管理用户”窗格中，按显示名称或用户名搜索用户，选择用户名，然后单击“添加”。******** 对想要添加的每一个用户重复此步骤。
    5. 添加完用户后，单击“保存”。****

- **拨号盘故障排除：**  

    - 确保用户已分配了[Teams 许可证](https://docs.microsoft.com/MicrosoftTeams/assign-teams-licenses)。
    - 确保用户已分配了[通话套餐](https://docs.microsoft.com/MicrosoftTeams/calling-plan-landing-page)。
    - 为用户启用[企业语音](https://docs.microsoft.com/skypeforbusiness/skype-for-business-hybrid-solutions/plan-your-phone-system-cloud-pbx-solution/enable-users-for-enterprise-voice-online-and-phone-system-voicemail#to-enable-your-users-for-phone-system-in-office-365-voice-and-voicemail)。

- **有关 Teams 登录的疑难解答：** 首先请确保 [Microsoft Teams 服务正常](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/servicehealth)。 然后查看任何常见的错误代码，查看“[为什么我在登录 Microsoft 团队时遇到问题？](https://support.office.com/article/a02f683b-61a3-4008-9447-ee60c5593b0f)”  还可需要查看“[Microsoft Teams 中的身份模型和身份验证](https://docs.microsoft.com/MicrosoftTeams/identify-models-authentication)”。

**教育版客户：**

如果你的用户看到 "You're missing out!" 确保“[为学校启用 Microsoft Teams](https://docs.microsoft.com/microsoft-365/education/intune-edu-trial/enable-microsoft-teams)”。 在 EDU 租户中，默认情况下不启用 Microsoft Teams ，必须首先将其打开。

下一步，请参阅“[使用 Office 365 教育版远程教学和学习](https://support.office.com/article/remote-teaching-and-learning-in-office-365-education-f651ccae-7b65-478b-8366-51bb884025c4)”，了解如何设置学校、课程规划、虚拟会议和与学生共享内容。

最后，请务必查看下方中的 Microsoft Teams IT 管理培训视频、幻灯片等：https://docs.microsoft.com/MicrosoftTeams/itadmin-readiness#technical-training 
