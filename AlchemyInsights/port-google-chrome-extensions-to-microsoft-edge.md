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
ms.openlocfilehash: 34ec7e71a2f27eb5b46395876a4d1c903189be1050e523796c9f2a817c20aaa0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973696"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a>Porten von Google Chrome-Erweiterungen zu Microsoft Edge (Chromium)

Es ist einfach, [Google Chrome-Erweiterungen zu Microsoft Edge (Chromium) zu portieren.](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension) In den meisten Fällen sind nur minimale Änderungen erforderlich, um diese Erweiterungen auf Microsoft Edge auszuführen.

Die von Google Chrome unterstützten Erweiterungs-APIs und Manifestschlüssel sind codekompatibel mit Microsoft Edge. Microsoft Edge unterstützt jedoch nicht die Erweiterungs-APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken und chrome.instanceID.