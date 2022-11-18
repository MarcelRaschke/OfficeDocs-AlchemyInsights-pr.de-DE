---
title: Problem mit einem einzelnen Benutzer
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
- "8469"
ms.openlocfilehash: dcc5af8cbbac9384c0af28890cb9ca014fc530b4
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66386805"
---
# <a name="problem-with-single-user"></a>Problem mit einem einzelnen Benutzer

- Der Benutzer wurde möglicherweise nicht bereitgestellt, weil der Dienst noch keine Möglichkeit hatte, den Benutzer auszuwerten. Lesen Sie die Anleitungen für die Dauer der Bereitstellung sowie die Statusanzeige auf der Seite für die Bereitstellungskonfiguration. Wenn der im Abschnitt mit den zusätzlichen Details angegebene stabile Zustand vor dem Datum liegt, an dem der Benutzer erstellt/aktualisiert/gelöscht wurde, bedeutet dies, dass der Benutzer noch nicht ausgewertet wurde. In diesem Szenario müssen Sie am besten warten, bis der Bereitstellungsdienst abgeschlossen ist.

  - Beachten Sie, dass unser Dienst nur Änderungen an einem Benutzer im Quellsystem (Cloud HR) erkennt. Es muss eine gültige Änderung im Quellsystem für Azure AD vorhanden sein, um die Änderung zu erkennen und in Active Directory zu fließen.
- Der Bereitstellungsdienst hat den Benutzer ausgewertet und festgestellt, dass er nicht bereitgestellt werden sollte:
  - Wenn Sie einen attributbasierten Bereichsdefinitionsfilter festgelegt haben, stellen Sie sicher, dass der Benutzer die von Ihnen angegebenen Kriterien erfüllt.
  - Wenn benutzer bereits im Zielsystem vorhanden sind und der Status des Benutzers in der Quell- und Ziel-Übereinstimmung vorhanden ist, werden wir keine weiteren Maßnahmen ergreifen.
- Der Bereitstellungsdienst hat versucht, den Benutzer bereitzustellen, und es ist ein Fehler aufgetreten. Lesen Sie für diese Szenarien die Registerkarte "Problembehandlung und Empfehlungen" der Bereitstellungsprotokolle:
  - Ein erforderliches Attribut für den Benutzer fehlt möglicherweise in lokales Active Directory oder Azure AD. Beispielsweise generieren die Generierungsregeln "userPrincipalName" oder "sAMAccountName" nicht den richtigen Wert.
  - Das übereinstimmende Attribut (in der Regel employeeId) wird nicht für einen eindeutigen Benutzer in lokales Active Directory oder Azure AD aufgelöst. Beispielsweise gibt es zwei Benutzer mit derselben employeeId in AD, und der Dienst gibt einen Fehlercode zurück, der doppelte Zieleinträge für denselben Quelleintrag angibt.

Informationen zum Überprüfen von Protokollen für einzelne Benutzer und Gruppen finden [Sie unter Überprüfen der Bereitstellungsprotokolle für ein Problem mit einem bestimmten Benutzer](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).
