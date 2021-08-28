---
title: Probleme mit geheimen Clientschlüsseln oder Zertifikaten für die App-Registrierung
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9685"
ms.openlocfilehash: 588273f43f7c2d57b377b234885cf4283d466919b562536f78a64356422f9f9f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951492"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Probleme mit geheimen Clientschlüsseln oder Zertifikaten für die App-Registrierung

Ablauf des geheimen Anwendungsclientschlüssels?

Unabhängig davon, wie die registrierte Anwendung erstellt wurde, ob über den Standardregistrierungsprozess im App-Registrierungsportal oder wenn der Dienstprinzipal in Ihrem Mandanten mithilfe der Anwendungszustimmung erstellt wurde, muss vor ablaufen des aktuellen Clientschlüssels ein neuer geheimer Clientschlüssel erstellt und im zugehörigen Anwendungscode aktualisiert werden. Die maximale Gültigkeitsdauer beträgt 2 Jahre. Zur Erinnerung muss der geheime Wert aufgezeichnet werden, da er nach verlassen der App-Registrierungsseite im Portal nicht mehr sichtbar ist. Weitere Informationen finden Sie unter [Schnellstart: Registrieren einer App in der Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) und bewährte Methoden für die [Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).

Weitere Informationen finden Sie unter [Erstellen einer Azure AD-App & Dienstprinzipals im Portal – Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).
