---
title: Konfigurieren des Bereitstellungsdiensts
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: d78eeb7d60b63d56f02e61a1086ea51cd6e6f223
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66356187"
---
# <a name="configuring-the-provision-service"></a>Konfigurieren des Bereitstellungsdiensts

Damit die automatisierte Benutzerbereitstellung funktioniert, benötigt Azure AD gültige Anmeldeinformationen, die es ermöglichen, eine Verbindung mit der Workday Web Services-API herzustellen. Darüber hinaus überprüft die Schaltfläche "Verbindung testen" in der App "Arbeitstag zur AD-Benutzerbereitstellung", ob sie eine Verbindung mit dem Azure AD Connect-Bereitstellungs-Agent herstellen kann, der der AD-Domäne zugeordnet ist.

Wenn der Azure-Portal beim Speichern der Anmeldeinformationen einen Fehler zurückgibt, führen Sie die folgenden empfohlenen Schritte aus:

1. Vergewissern Sie sich, dass Sie das Benutzerkonto des Workday-Integrationssystems konfiguriert haben, wie im Lernprogrammabschnitt ["Konfigurieren des Benutzers des Integrationssystems in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)" angegeben.
2. Vergewissern Sie sich, dass der Azure AD Connect-Bereitstellungs-Agent-Dienst auf Ihrem lokalen Windows-Server mithilfe der Dienstverwaltungskonsole ausgeführt wird. Sie können auch den Status des Agents im Azure-Portal überprüfen, indem Sie auf die Schaltfläche "Lokale Agents anzeigen" klicken.
3. Stellen Sie sicher, dass Sie den Wert für das Feld "Arbeitstag-Benutzername" im Format username@workday-Mandantennamen eingeben. Wenn der Name "workday-tenant" fehlt, schlägt die Workday-Authentifizierung fehl.
4. Wenn Sie die Integration mit dem Workday-Implementierungsmandanten konfigurieren, beachten Sie die geplanten Ausfallzeiten Ihres Workday-Mandanten. Workday hat die Ausfallzeit für die Implementierungsmandanten über Wochenenden (in der Regel von Freitagabend bis Samstagmorgen) geplant, und Verbindungsfehler während dieses Ausfallzeitfensters sind ein bekanntes Problem, das automatisch behoben wird, sobald die Implementierungsmandanten wieder online sind.
5. In seltenen Fällen wird dieser Fehler möglicherweise auch angezeigt, wenn sich das Kennwort des Integrationssystembenutzers aufgrund einer Mandantenaktualisierung geändert hat oder wenn sich das Konto im gesperrten oder abgelaufenen Zustand befindet. Bitte überprüfen Sie den Status des Integrationssystems-Benutzers mit Ihrem Workday-Administrator.

Weitere Details zum Konfigurieren von Workday für die automatische Bereitstellung finden Sie unter [Tutorial: Konfigurieren von Workday für die automatische Benutzerbereitstellung](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
