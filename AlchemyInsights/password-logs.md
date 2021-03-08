---
title: Kennwortprotokolle
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50523085"
---
# <a name="password-logs"></a>Kennwortprotokolle

**Ich habe Probleme beim Zugriff auf Überwachungsprotokolle für die Kennwortzurücksetzung**

Führen Sie den folgenden Schritt aus, um Probleme im Zusammenhang mit dem Zugriff auf Überwachungsprotokolle für die Kennwortzurücksetzung zu behandeln:

Stellen Sie sicher, dass Sie zum Anzeigen von Überwachungsprotokollen autorisiert sind. 

Nur die folgenden Rollen sind autorisiert:
 - Globaler Administrator
 - Sicherheitsadministrator
 - Benutzer mit Leseberechtigung für Sicherheitsfunktionen

**Ich möchte alle Überwachungsereignisse für die Kennwortzurücksetzung ab der ersten Bereitstellung sehen**

In den Berichten der letzten 30 Tage wurden bis zu 120.000 Kennwortzurücksetzungs-/Registrierungsereignisse gespeichert. Dieses maximale Limit gilt für die Benutzeroberfläche beim Herunterladen der CSV-Datei. 1 Million Ereignisse stehen über PowerShell zur Verfügung.
Weitere Informationen finden Sie in den nachfolgenden Tipps:

- [Self-Service-Kennwortzurücksetzungsereignisse aus den Azure AD-Berichts- und -Ereignis-API](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Schnelles Herunterladen von Registrierungsereignissen für die Kennwortzurücksetzung mit PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**Ich möchte mehr über die Berichterstellungsfunktionen für die Kennwortzurücksetzung erfahren**

Überprüfen Sie im Azure-Portal unter **„Benutzer und Gruppen"**, wer Kennwörter mit Azure AD-Protokollen zur Kennwortzurücksetzung registriert oder zurücksetzt.
Weitere Informationen finden Sie unter den folgenden Links:

- [Übersicht über das Zurücksetzen von Kennwörtern](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Anzeigen von Berichten zur Kennwortzurücksetzung im Azure-Portal](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Self-Service-Kennwortzurücksetzungsereignisse aus den Azure AD-Berichts- und -Ereignis-API](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Schnelles Herunterladen von Registrierungsereignissen für die Kennwortzurücksetzung mit PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


