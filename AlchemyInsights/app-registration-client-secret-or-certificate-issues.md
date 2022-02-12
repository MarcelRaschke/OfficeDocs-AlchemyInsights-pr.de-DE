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
ms.openlocfilehash: 270eaa24e0126577e2074d447d405557489b7c87
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62627551"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Probleme mit geheimen Clientschlüsseln oder Zertifikaten für die App-Registrierung

Ablauf des geheimen Anwendungsclientschlüssels?

Unabhängig davon, wie die registrierte Anwendung erstellt wurde, ob über den Standardregistrierungsprozess im App-Registrierungsportal oder wenn der Dienstprinzipal in Ihrem Mandanten mithilfe der Anwendungszustimmung erstellt wurde, muss vor ablaufen des aktuellen Clientschlüssels ein neuer geheimer Clientschlüssel erstellt und im zugehörigen Anwendungscode aktualisiert werden. Die maximale Gültigkeitsdauer beträgt 2 Jahre. Zur Erinnerung muss der geheime Wert aufgezeichnet werden, da er nach verlassen der App-Registrierungsseite im Portal nicht mehr sichtbar ist. Weitere Informationen finden Sie unter [Schnellstart: Registrieren einer App im Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) und [bewährte Methoden für die Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).

Weitere Informationen finden Sie unter [Erstellen eines Azure AD App-& Dienstprinzipals im Portal – Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).
