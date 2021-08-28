---
title: Entfernen des Hintergrunddienstes für Microsoft Search in Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/12/2021
ms.locfileid: "50753415"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>Entfernen des Hintergrunddienstes für Microsoft Search in Bing

Um den Hintergrunddienst für Microsoft Search in Bing zu entfernen, können Sie folgende Möglichkeiten versuchen:

1. Um zu den ursprünglichen Suchmaschinen-Einstellungen zurückzukehren, führen Sie Folgendes durch:

    a. Setzen Sie den Schalter **Bing als Standardsuchmaschine verwenden [auf](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Aus**.

    b. [Gehen Sie zum Microsoft 365 Admin Center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) und löschen Sie die Einstellung, welche alle Benutzer in Ihrer Organisation betrifft.

2. Um den Hintergrunddienst von einem einzelnen Gerät zu entfernen, führen Sie folgende Tasks durch:

    a. Wählen Sie **Systemsteuerung > Programme > Programme und Funktionen** aus.

    b. Klicken Sie in der Liste der installierten Programme mit der rechten Maustaste auf **Microsoft Search in Bing**, und anschließend klicken Sie auf **Deinstallieren**.

3. Um den Hintergrunddienst von mehreren Geräten in Ihrer Organisation zu entfernen, melden Sie sich als Administrator an und führen Sie den folgenden Befehl in einem Skript aus: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
