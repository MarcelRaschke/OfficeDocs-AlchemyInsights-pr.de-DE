---
title: Benutzerbereitstellung
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
- "9004348"
- "8428"
ms.openlocfilehash: c4df8d991d4a429abe3977d34e0bec173aef8d50
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62690674"
---
# <a name="user-provisioning"></a>Benutzerbereitstellung

- Verwenden Sie die [On-Demand-Bereitstellungsfunktion](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) , um einen Benutzer bereitzustellen und detaillierte Diagnosen zu den schritten zu erhalten.
- Informationen zur Behebung von Problemen bei der Bereitstellung von Benutzern und Gruppen finden Sie im Fehlerbehebungshandbuch [Es werden keine Benutzer bereitgestellt](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned).
- Wenn Sie feststellen, dass Benutzer nicht bereitgestellt werden, lesen Sie [Bereitstellungsprotokolle (Vorschau)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) in Azure Active Directory (AD). Suchen Sie nach Protokolleinträgen, die sich auf einen bestimmten Benutzer beziehen.
- Starten Sie die Bereitstellung regelmäßig neu, um alle Benutzer abzufangen, die in einem vorherigen Bereitstellungszyklus übersehen wurden.
- Der Benutzer/die Gruppe wurde möglicherweise nicht bereitgestellt, da unser Dienst noch keine Möglichkeit hatte, den Benutzer auszuwerten. Überprüfen Sie die Anleitung für die Dauer der Bereitstellung sowie die Statusanzeige auf der Seite mit der Bereitstellungskonfiguration. Wenn der im Abschnitt mit zusätzlichen Details angegebene stabile Zustand vor dem Erstellungs-/Aktualisierungs-/Löschungsdatum des Benutzers liegt, bedeutet dies, dass der Benutzer noch nicht ausgewertet wurde. In diesem Szenario sollten Sie am besten warten, bis der Bereitstellungsdienst abgeschlossen ist. Wenn der stabile Zustand erreicht wurde, wird empfohlen, einen Neustart über die Benutzeroberfläche im Azure-Portal durchzuführen.
  - Beachten Sie, dass unser Dienst nur Änderungen an einem Benutzer/einer Gruppe im Quellsystem erkennt (Azure Active Directory). Wenn ein Benutzer/eine Gruppe direkt in der Anwendung entfernt wird (z. B. ServiceNow), sind wir uns dieser Änderungen nicht bewusst und führen kein Rollback basierend auf dem Status des Benutzers im Quellsystem durch. In diesem Szenario empfiehlt es sich, ein Rollback der Änderung direkt in der Zielanwendung vorzunehmen.
- Unser Dienst hat den Benutzer/die Gruppe ausgewertet und festgestellt, dass er nicht bereitgestellt werden sollte:
  - Wenn Sie den Bereich auf zugewiesene Benutzer und Gruppen festgelegt haben, überprüfen Sie, ob der Benutzer/die Gruppe der Anwendung zugewiesen ist.
  - Wenn der Benutzer/die Gruppe der Anwendung zugewiesen ist, stellen Sie sicher, dass er nicht der Standardzugriffsrolle zugewiesen ist. Diese Rolle kann nicht für die Bereitstellung verwendet werden.
  - Wenn Sie einen attributbasierten Bereichsfilter festgelegt haben, stellen Sie sicher, dass der Benutzer die angegebenen Kriterien erfüllt.
  - Wenn Benutzer bereits im Zielsystem vorhanden sind und der Status des Benutzers in der Quell- und Zielübersprechung vorhanden ist, werden keine weiteren Maßnahmen ergriffen.
- Unser Dienst hat versucht, den Benutzer bereitzustellen, und es ist fehlgeschlagen. Überprüfen Sie für diese Szenarien die Registerkarte "Problembehandlung und Empfehlungen" der Bereitstellungsprotokolle:
  - Ein erforderliches Attribut für den Benutzer fehlt möglicherweise in Azure Active Directory oder entspricht nicht dem format, das von der Drittanbieteranwendung benötigt wird. Beispielsweise kann das "Country"-Attribut eines Benutzers auf "Usa" festgelegt werden, wenn es "USA" sein sollte.
  - Das Attribut ist ein referentielles Attribut, das noch nicht in der Zielanwendung vorhanden ist. Ein referentielles Attribut ist ein Attribut, das auf ein anderes Objekt verweist, z. B. auf einen Benutzer, der Mitglied einer Gruppe ist. Die Benutzer-ID befindet sich im Memberattribut der Gruppe, kann jedoch nur verarbeitet werden, wenn das Benutzerobjekt, auf das es verweist, bereits vorhanden ist.
