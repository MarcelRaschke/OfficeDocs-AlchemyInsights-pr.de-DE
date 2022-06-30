---
title: Benutzerbereitstellung
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004348"
- "8428"
ms.openlocfilehash: be4f177a89baae8711992521afc4732a9d9b8c3f
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66520052"
---
# <a name="user-provisioning"></a>Benutzerbereitstellung

- Verwenden Sie die [On-Demand-Bereitstellungsfunktion](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) , um einen Benutzer bereitzustellen und detaillierte Diagnosen zu den ausgeführten Schritten zu erhalten.
- Informationen zur Behebung von Problemen bei der Bereitstellung von Benutzern und Gruppen finden Sie im Fehlerbehebungshandbuch [Es werden keine Benutzer bereitgestellt](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned).
- Wenn Sie feststellen, dass Benutzer nicht bereitgestellt werden, lesen Sie [Bereitstellungsprotokolle (Vorschau)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) in Azure Active Directory (AD). Suchen Sie nach Protokolleinträgen, die sich auf einen bestimmten Benutzer beziehen.
- Starten Sie die Bereitstellung regelmäßig neu, um alle Benutzer zu erfassen, die in einem vorherigen Bereitstellungszyklus verpasst wurden.
- Der Benutzer/die Gruppe wurde möglicherweise nicht bereitgestellt, weil unser Dienst noch keine Möglichkeit hatte, den Benutzer zu bewerten. Lesen Sie die Anleitungen für die Dauer der Bereitstellung sowie die Statusanzeige auf der Seite für die Bereitstellungskonfiguration. Wenn der im Abschnitt mit den zusätzlichen Details angegebene stabile Zustand vor dem Datum liegt, an dem der Benutzer erstellt/aktualisiert/gelöscht wurde, bedeutet dies, dass der Benutzer noch nicht ausgewertet wurde. In diesem Szenario müssen Sie am besten warten, bis der Bereitstellungsdienst abgeschlossen ist. Wenn der stabile Zustand erreicht wurde, wird empfohlen, einen Neustart über die Benutzeroberfläche im Azure-Portal durchzuführen.
  - Beachten Sie, dass unser Dienst nur Änderungen an einem Benutzer/einer Gruppe im Quellsystem (Azure Active Directory) erkennt. Wenn ein Benutzer/eine Gruppe direkt in der Anwendung entfernt wird (z. B. ServiceNow), sind uns diese Änderungen nicht bekannt und werden nicht basierend auf dem Status des Benutzers im Quellsystem zurückgesetzt. In diesem Szenario empfiehlt es sich, die Änderung direkt in der Zielanwendung zurückgesetzt zu haben.
- Unser Dienst hat den Benutzer/die Gruppe ausgewertet und festgestellt, dass er nicht bereitgestellt werden sollte:
  - Wenn Sie den Bereich auf zugewiesene Benutzer und Gruppen festgelegt haben, überprüfen Sie, ob der Benutzer/die Gruppe der Anwendung zugewiesen ist.
  - Wenn der Benutzer/die Gruppe der Anwendung zugewiesen ist, stellen Sie sicher, dass er nicht der Standardzugriffsrolle zugewiesen ist. Diese Rolle kann nicht für die Bereitstellung verwendet werden.
  - Wenn Sie einen attributbasierten Bereichsdefinitionsfilter festgelegt haben, stellen Sie sicher, dass der Benutzer die von Ihnen angegebenen Kriterien erfüllt.
  - Wenn benutzer bereits im Zielsystem vorhanden sind und der Status des Benutzers in der Quell- und Ziel-Übereinstimmung vorhanden ist, werden wir keine weiteren Maßnahmen ergreifen.
- Unser Dienst hat versucht, den Benutzer bereitzustellen, und er ist fehlgeschlagen. Lesen Sie für diese Szenarien die Registerkarte "Problembehandlung und Empfehlungen" der Bereitstellungsprotokolle:
  - Ein erforderliches Attribut für den Benutzer fehlt möglicherweise in Azure Active Directory oder stimmt nicht mit dem von der Drittanbieteranwendung benötigten Format überein. Beispielsweise kann das Attribut "Country" für einen Benutzer auf USA festgelegt werden, wenn es us sein sollte.
  - Das Attribut ist ein referenzielles Attribut, das in der Zielanwendung noch nicht vorhanden ist. Ein referenzielles Attribut ist ein Attribut, das auf ein anderes Objekt verweist, z. B. auf einen Benutzer, der Mitglied einer Gruppe ist. Die ID des Benutzers wäre im Memberattribut der Gruppe enthalten, kann aber nur verarbeitet werden, wenn das Benutzerobjekt, auf das es verweist, bereits vorhanden ist.
