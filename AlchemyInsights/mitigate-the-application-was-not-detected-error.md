---
title: Beheben des Fehlers "Sie Anwendung wurde nicht erkannt"
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 91f7d8d95dbbc1034e75a65a7ef3d66bb51160fc
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63273221"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>Beheben des Fehlers "Sie Anwendung wurde nicht erkannt"

Der von Intune gemeldete App-Installationsfehler "Die Anwendung wurde nicht erkannt" nach erfolgreichem Abschluss der Installation kann auf allen wichtigen Betriebssystemplattformen (Windows, IOS und Android) auftreten.

Zu den häufigsten Szenarien, die diesen Fehler generieren, gehören:

- Die App wurde nach der ersten Bereitstellung außerhalb von Intune (über den App Store eines Drittanbieters) aktualisiert. Einige Anwendungen wie Google Chrome können beispielsweise automatische Updates durchführen.
- Ein Benutzer hat die App nach der Erstinstallation deinstalliert.

Um dieses Problem zu vermeiden, untersuchen Sie zuerst die betroffenen Geräte, um das Szenario zu ermitteln, in dem der Fehler aufgetreten ist.

- Wenn die App außerhalb von Intune aktualisiert wurde, kann die App-Bereitstellung so festgelegt werden, dass diese Anwendungsversion ignoriert wird. Legen Sie dazu unter **App-Konfiguration > App-Informationen** die Option **App-Version ignorieren** auf **Ja** fest.
- Bei der Ausrichtung auf den Kunden kann es sinnvoll sein, die Anwendung als "Erforderlich" bereitzustellen, um sicherzustellen, dass die neueste Version bereitgestellt wird.
- Alternativ können Sie auf der iOS-Plattform die mit dem Apple-Volumenlizenzprogramm verknüpfte **AutoUpdate**-Funktionalität verwenden, die so konfiguriert werden kann, dass automatisch eine Aktualisierung auf neue Anwendungsversionen durchgeführt wird, sobald diese verfügbar sind.

Weitere Informationen zur Behandlung von Problemen bei der Installation von Apps finden Sie unter [Problembehandlung bei der App-Installation](https://docs.microsoft.com/intune/troubleshoot-app-install).
