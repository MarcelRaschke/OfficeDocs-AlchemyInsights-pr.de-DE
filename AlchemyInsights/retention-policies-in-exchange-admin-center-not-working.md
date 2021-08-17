---
title: Aufbewahrungsrichtlinien in Exchange Admin Center funktionieren nicht
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 6652ad5fc1691e1d5a4293d81f3a649f23ec38f18c8ed9fe06665628a901d13e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074931"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Aufbewahrungsrichtlinien im Exchange Admin Center

Wenn Sie möchten, dass wir automatisierte Überprüfungen für die unten genannten Einstellungen ausführen, wählen Sie die Schaltfläche "Zurück" < - oben auf dieser Seite aus, und geben Sie dann die E-Mail-Adresse des Benutzers ein, der Probleme mit Aufbewahrungsrichtlinien hat.

Wenn Sie Probleme mit Aufbewahrungsrichtlinien im Exchange Admin Center haben, die nicht auf Postfächer oder Elemente angewendet werden, die nicht in das Archivpostfach verschoben werden, überprüfen Sie Folgendes:

**Ursachen:**

- **Der Assistent für verwaltete Ordner** hat das Postfach des Benutzers nicht verarbeitet. Der Assistent für verwaltete Ordner versucht, jedes Postfach in Ihrer cloudbasierten Organisation einmal alle sieben Tage zu verarbeiten.

  **Lösung:** Führen Sie den Assistenten für verwaltete Ordner aus.

- **RetentionHold** wurde für das Postfach **aktiviert.** Wenn das Postfach auf ein RetentionHold-Objekt gesetzt wurde, wird die Aufbewahrungsrichtlinie für das Postfach während dieser Zeit nicht verarbeitet.

  **Lösung:** Überprüfen Sie den Status der Aufbewahrungssperre, und aktualisieren Sie sie nach Bedarf. Ausführliche Informationen finden Sie unter [Aufbewahrungssperre für Postfächer.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
 
**Hinweis:** Wenn ein Postfach kleiner als 10 MB ist, verarbeitet der Assistent für verwaltete Ordner das Postfach nicht automatisch.
 
Weitere Informationen zu Aufbewahrungsrichtlinien im Exchange Admin Center finden Sie unter:

- [Aufbewahrungstags und Aufbewahrungsrichtlinien](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Anwenden einer Aufbewahrungsrichtlinie auf Postfächer](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) oder [Hinzufügen oder Entfernen von Aufbewahrungstags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Identifizieren des auf ein Postfach angewandten Aufbewahrungstyps](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
