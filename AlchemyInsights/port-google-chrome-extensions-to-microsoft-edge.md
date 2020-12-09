---
title: '将 Google Chrome extensions 扩展到 Microsoft Edge (Chromium) '
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
ms.openlocfilehash: 2a20f258cbcbca7c8db4e38c52464fefb1b6f39d
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49600093"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a><span data-ttu-id="2af3c-102">将 Google Chrome extensions 扩展到 Microsoft Edge (Chromium) </span><span class="sxs-lookup"><span data-stu-id="2af3c-102">Port Google Chrome extensions to Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="2af3c-103">可以轻松地将 [Google Chrome 扩展移植到 Microsoft Edge (Chromium) ](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension)。</span><span class="sxs-lookup"><span data-stu-id="2af3c-103">It's easy to [port Google Chrome extensions to Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span></span> <span data-ttu-id="2af3c-104">在大多数情况下，只需最少的更改即可在 Microsoft Edge 上运行这些扩展。</span><span class="sxs-lookup"><span data-stu-id="2af3c-104">In most cases, only minimal changes are needed to run these extensions on Microsoft Edge.</span></span>

<span data-ttu-id="2af3c-105">Google Chrome 支持的扩展 Api 和清单键是与 Microsoft Edge 兼容的代码。</span><span class="sxs-lookup"><span data-stu-id="2af3c-105">The extension APIs and manifest keys supported by Google Chrome are code-compatible with Microsoft Edge.</span></span> <span data-ttu-id="2af3c-106">但是，Microsoft Edge 不支持扩展 Api chrome，getAccounts，chrome，getAuthToken，和 chrome. instanceID。</span><span class="sxs-lookup"><span data-stu-id="2af3c-106">However, Microsoft Edge does not support the extension APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken, and chrome.instanceID.</span></span>