---
title: Problembehandlung bei der Registrierung von Android-Geräten in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 0ae926e6b31493e7359981c621fd27e8f53d49a17bdf107173b087fe6cc688fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54008077"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Problembehandlung bei der Registrierung von Android-Geräten in Microsoft Intune

Überprüfen Sie die unten aufgeführten Ressourcen, um Ihr Problem jetzt zu beheben.
  
Einige häufige Probleme und Lösungsschritte:
  
 **Fehler "Gerät nicht verschlüsselt" in Unternehmensportal:** Neuere Versionen von Android, insbesondere ab Version 7.0, erfordern eine Startkennung, um sicherzustellen, dass Ihr Gerät vollständig verschlüsselt ist. Gängige Lösungen sind das Aktivieren eines Start-Pins oder das vollständige Verschlüsseln des Geräts. Lesen Sie [dieses Dokument,](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) um weitere Informationen zu erfahren.
  
 **Geräte können beim Intune-Dienst nicht einchecken oder in der Intune-Verwaltungskonsole als "Fehlerhaft" angezeigt werden:** Einige Samsung 4.4- und 5.5-Geräte werden möglicherweise nicht in den Dienst eingecheckt. Es gibt drei mögliche Lösungen für dieses Problem:
  
1. Öffnen Sie manuell die Intune-Unternehmensportal App, die automatisch eine Gerätesynchronisierung initiiert.

2. Aktualisieren Sie das Gerät auf Android 6.0 oder höher.

3. Deaktivieren Sie die Verwaltung des Intune-Unternehmensportal durch den Smart Manager von Samsung. Weitere Details zu diesen Problemen und Lösungen finden Sie in [diesem Dokument.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console)

 Fehler **"Benutzerlizenztyp ungültig"** oder **"Benutzername nicht erkannt":** Dem Benutzer muss eine Intune- oder EMS-Lizenz zugewiesen werden. Überprüfen Sie diese Dokumente, um eine Lizenz über: Office Admin Center oder Azure-Portal zuzuweisen.
  
Zusätzliche Ressourcen zur Behebung Des Problems:
  
1. Verwenden Sie das [Intune-Problembehandlungsportal,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) um häufige Registrierungsfehler zu diagnostizieren und zu beheben. Weitere Informationen finden Sie in [diesem Dokument.](https://docs.microsoft.com/intune/help-desk-operators)

2. In [diesem Dokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) wird eine Liste der häufigsten Fehler aufgeführt, die die Registrierung und Auflösung der einzelnen Fehler verhindern.

3. [Erfahren Sie, wie Sie Android-Geräte in Microsoft Intune registrieren.](https://docs.microsoft.com/intune/android-enroll)
