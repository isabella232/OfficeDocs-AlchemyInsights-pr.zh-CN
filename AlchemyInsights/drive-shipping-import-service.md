---
title: Microsoft 365 导入服务中的驱动器传送
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: ea9f78176bcc3208c01da5ccfaeb97af4373a5b5d1a4abc652422a0f85df7d9a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004180"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a>Microsoft 365 导入服务中的驱动器传送

使用驱动器传送，将 PSTS 复制到硬盘，然后将硬盘发运到 Microsoft。

请按照以下步骤开始操作:

1. 在 Microsoft 365 合规中心的“**信息治理”** 下，选择“**导入**”。

1. 选择“**选择导入作业类型**”，然后选择“**下一步**”。

1. 若要查看此导入选项的步骤，请选择“**将硬盘传送到我们其中的一个物理位置**”。

以下是几点注意事项:

- 你必须分配有 Exchange Online 中的邮箱导入导出角色，才能将 PST 文件导入到 Microsoft 365 邮箱。对于大于 20GB 的 PST，性能可能会受到影响。

- 仅支持将 2.5 英寸固态硬盘 (SSD) 或 2.5 英寸或 3.5 英寸 SATA II/III 内部硬盘。
包含 PST 文件的硬盘必须使用 BitLocker 进行加密。

- 使用驱动器传送将 PST 文件导入到 Microsoft 365 邮箱的成本为每 GB 数据 2 美元。

有关使用驱动器传送方法导入 PST 的其他信息，请参阅[使用驱动器传送导入组织的 PST 文件](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365)。