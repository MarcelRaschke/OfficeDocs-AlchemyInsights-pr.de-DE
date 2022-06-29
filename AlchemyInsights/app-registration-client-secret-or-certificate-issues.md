---
title: Probleme mit dem geheimen App-Registrierungsclient oder zertifikatsbasierten Zertifikaten
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004352"
- "9685"
ms.openlocfilehash: 081bd860f8df94c04dc371ed8c8e4b5de9c4002b
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66300520"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Probleme mit dem geheimen App-Registrierungsclient oder zertifikatsbasierten Zertifikaten

Ablauf des geheimen Anwendungsclientschlüssels?

Unabhängig davon, wie die registrierte Anwendung erstellt wurde, ob über den Standardregistrierungsprozess im App-Registrierungsportal oder wenn der Dienstprinzipal in Ihrem Mandanten mithilfe der Anwendungszustimmung erstellt wurde, muss vor ablaufen des aktuellen Schlüssels ein neuer geheimer Clientschlüssel erstellt und im zugehörigen Anwendungscode aktualisiert werden. Die maximale Gültigkeitsdauer beträgt 2 Jahre. Zur Erinnerung muss der geheime Wert aufgezeichnet werden, da er nach dem Verlassen der App-Registrierungen Seite im Portal nicht mehr sichtbar ist. Weitere Informationen finden Sie [in der Schnellstartanleitung: Registrieren einer App im Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) und [bewährten Methoden für die Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).

Weitere Informationen finden [Sie unter Erstellen einer Azure AD-App & Dienstprinzipal im Portal – Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).
