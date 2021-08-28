---
title: Konfigurieren des Bereitstellungsdiensts
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
- "9004687"
- "8468"
ms.openlocfilehash: 271ab7ad34c0f85f6f5a9d8d3dc2d901fe6fe8f978a2cc98eed986f594036f17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033277"
---
# <a name="configuring-the-provision-service"></a>Konfigurieren des Bereitstellungsdiensts

Damit die automatisierte Benutzerbereitstellung funktioniert, benötigt Azure AD gültige Anmeldeinformationen, mit denen eine Verbindung mit der Workday-Webdienste-API hergestellt werden kann. Darüber hinaus überprüft die Schaltfläche "Verbindung testen" in der App "Workday to AD User Provisioning", ob sie in der Lage ist, eine Verbindung mit dem Azure AD Verbinden Bereitstellungs-Agent herzustellen, der der AD-Domäne zugeordnet ist.

Wenn das Azure-Portal beim Speichern der Anmeldeinformationen einen Fehler zurückgibt, führen Sie die folgenden empfohlenen Schritte aus:

1. Vergewissern Sie sich, dass Sie das Benutzerkonto des Workday-Integrationssystems konfiguriert haben, wie im Lernprogrammabschnitt "Konfigurieren des [Integrationssystembenutzers in Workday"](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)angegeben.
2. Vergewissern Sie sich, dass der Azure AD Verbinden Provisioning Agent Service auf Ihrem lokalen Windows-Server mithilfe der Dienste-Verwaltungskonsole ausgeführt wird. Sie können auch den Status des Agents im Azure-Portal überprüfen, indem Sie auf die Schaltfläche "Lokale Agents anzeigen" klicken.
3. Stellen Sie sicher, dass Sie den Wert für das Feld "Workday Username" mit dem Format username@workday-Mandanten-Name eingeben. Wenn der Name des workday-tenant-Werts fehlt, schlägt die Workday-Authentifizierung fehl.
4. Wenn Sie die Integration in den Workday-Implementierungsmandanten konfigurieren, notieren Sie sich die geplanten Ausfallzeiten Ihres Workday-Mandanten. Workday hat für die Implementierungsmandanten über Wochenenden (in der Regel von Freitagabend bis Samstag) Ausfallzeiten geplant, und Verbindungsfehler während dieses Ausfallzeitfensters sind ein bekanntes Problem, das automatisch behoben wird, sobald die Implementierungsmandanten wieder online sind.
5. In seltenen Fällen wird dieser Fehler auch angezeigt, wenn das Kennwort des Integrationssystembenutzers aufgrund einer Mandantenaktualisierung geändert wurde oder das Konto gesperrt oder abgelaufen ist. Überprüfen Sie den Status des Integrationssystembenutzers bei Ihrem Workday-Administrator.

Weitere Details zum Konfigurieren von Workday für die automatische Bereitstellung finden Sie unter [Tutorial: Konfigurieren von Workday für die automatische Benutzerbereitstellung](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
