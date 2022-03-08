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
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: 12ce40886c2442309a0c5fb0a734928b763db2c5
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63126353"
---
# <a name="problem-with-single-user"></a>Problem mit einem einzelnen Benutzer

- Der Benutzer wurde möglicherweise nicht bereitgestellt, da der Dienst noch keine Möglichkeit hatte, den Benutzer auszuwerten. Überprüfen Sie die Anleitung für die Dauer der Bereitstellung sowie die Statusanzeige auf der Seite mit der Bereitstellungskonfiguration. Wenn der im Abschnitt mit zusätzlichen Details angegebene stabile Zustand vor dem Erstellungs-/Aktualisierungs-/Löschungsdatum des Benutzers liegt, bedeutet dies, dass der Benutzer noch nicht ausgewertet wurde. In diesem Szenario sollten Sie am besten warten, bis der Bereitstellungsdienst abgeschlossen ist.

  - Beachten Sie, dass unser Dienst nur Änderungen an einem Benutzer im Quellsystem (Cloud HR) erkennt. Es muss eine gültige Änderung im Quellsystem vorhanden sein, damit Azure AD die Änderung erkennen und in Active Directory fließen können.
- Der Bereitstellungsdienst hat den Benutzer ausgewertet und festgestellt, dass er nicht bereitgestellt werden sollte:
  - Wenn Sie einen attributbasierten Bereichsfilter festgelegt haben, stellen Sie sicher, dass der Benutzer die angegebenen Kriterien erfüllt.
  - Wenn Benutzer bereits im Zielsystem vorhanden sind und der Status des Benutzers in der Quell- und Zielübersprechung vorhanden ist, werden keine weiteren Maßnahmen ergriffen.
- Der Bereitstellungsdienst hat versucht, den Benutzer bereitzustellen, und es ist ein Fehler aufgetreten. Überprüfen Sie für diese Szenarien die Registerkarte "Problembehandlung und Empfehlungen" der Bereitstellungsprotokolle:
  - Möglicherweise fehlt ein erforderliches Attribut für den Benutzer in lokalem Active Directory oder Azure AD. Beispielsweise generieren die UserPrincipalName- oder sAMAccountName-Generierungsregeln nicht den richtigen Wert.
  - Das übereinstimmende Attribut (in der Regel employeeId) wird nicht für einen eindeutigen Benutzer im lokalen Active Directory oder Azure AD aufgelöst. Beispielsweise gibt es zwei Benutzer mit derselben EmployeeId in AD, und der Dienst gibt einen Fehlercode zurück, der auf doppelte Zieleinträge für denselben Quelleintrag hinweist.

Informationen zum Überprüfen von Protokollen für einzelne Benutzer und Gruppen finden Sie unter ["Überprüfen der Bereitstellungsprotokolle für ein Problem mit einem bestimmten Benutzer](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)".
