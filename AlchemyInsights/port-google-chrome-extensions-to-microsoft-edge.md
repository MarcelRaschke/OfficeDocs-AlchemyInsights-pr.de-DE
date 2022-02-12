---
title: Porten von Google Chrome-Erweiterungen zu Microsoft Edge (Chromium)
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
ms.openlocfilehash: 8e04149a8e22ae8ca0f5a36ca786f7e57b3e31bc
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62648580"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a>Porten von Google Chrome-Erweiterungen zu Microsoft Edge (Chromium)

Es ist einfach, [Google Chrome-Erweiterungen zu Microsoft Edge (Chromium) zu portieren](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension). In den meisten Fällen sind nur minimale Änderungen erforderlich, um diese Erweiterungen auf Microsoft Edge auszuführen.

Die von Google Chrome unterstützten Erweiterungs-APIs und Manifestschlüssel sind codekompatibel mit Microsoft Edge. Microsoft Edge unterstützt jedoch nicht die Erweiterungs-APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken und chrome.instanceID.