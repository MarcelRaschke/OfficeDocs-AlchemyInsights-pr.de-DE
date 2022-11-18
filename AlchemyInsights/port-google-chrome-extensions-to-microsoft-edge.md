---
title: Portieren von Google Chrome-Erweiterungen zu Microsoft Edge (Chromium)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004617"
- "9004032"
- "7102"
- "8297"
ms.date: 12/03/2020
ms.openlocfilehash: 8d61f359bd7499126bcaae8f32dc8e2b09db67b2
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66374547"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a>Portieren von Google Chrome-Erweiterungen zu Microsoft Edge (Chromium)

Es ist einfach, [Google Chrome-Erweiterungen zu Microsoft Edge (Chromium) zu portieren](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension). In den meisten Fällen sind nur minimale Änderungen erforderlich, um diese Erweiterungen auf Microsoft Edge auszuführen.

Die von Google Chrome unterstützten Erweiterungs-APIs und Manifestschlüssel sind codekompatibel mit Microsoft Edge. Microsoft Edge unterstützt jedoch nicht die Erweiterungs-APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken und chrome.instanceID.