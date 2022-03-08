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
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9004032"
- "7102"
- "8297"
- "9004617"
ms.openlocfilehash: 71be743be6da8f818eba6c1deb3e227618eeca0d
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63262853"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a>Porten von Google Chrome-Erweiterungen zu Microsoft Edge (Chromium)

Es ist einfach, [Google Chrome-Erweiterungen zu Microsoft Edge (Chromium) zu portieren](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension). In den meisten Fällen sind nur minimale Änderungen erforderlich, um diese Erweiterungen auf Microsoft Edge auszuführen.

Die von Google Chrome unterstützten Erweiterungs-APIs und Manifestschlüssel sind codekompatibel mit Microsoft Edge. Microsoft Edge unterstützt jedoch nicht die Erweiterungs-APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken und chrome.instanceID.