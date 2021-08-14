---
title: '将 Google Chrome 扩展移植到 Microsoft Edge (Chromium) '
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004032"
- "7102"
- "8297"
- "9004617"
ms.openlocfilehash: 34ec7e71a2f27eb5b46395876a4d1c903189be1050e523796c9f2a817c20aaa0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973687"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a>将 Google Chrome 扩展移植到 Microsoft Edge (Chromium) 

可轻松将 Google [Chrome 扩展移植到 Microsoft Edge (Chromium) 。 ](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension) 在大多数情况下，只需进行最少的更改，才能在 Microsoft Edge。

Google Chrome 支持的扩展 API 和清单密钥与 Microsoft Edge。 但是，Microsoft Edge不支持扩展 API chrome.gcm、chrome.identity.getAccounts、chrome.identity.getAuthToken 和 chrome.instanceID。