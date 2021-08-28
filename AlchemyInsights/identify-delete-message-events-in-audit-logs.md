---
title: Identifizieren von Löschen von Nachrichtenereignissen in Überwachungsprotokollen
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7e13c9e5fbfa6ade065c2810150687085c1a9daae1a11c134688ec9a83ad37d9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54115647"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Überwachungsprotokolle für gelöschte E-Mail-Nachrichten

Ab Januar 2019 aktiviert Microsoft standardmäßig die Postfachüberwachungsprotokollierung. Andernfalls müssen Sie zum Überprüfen von Löschnachrichtenereignissen für einen bestimmten Benutzer die Löschaktionen manuell für die Überwachung aktivieren. Wenn die Postfachüberwachungsprotokollierung bereits für Ihre Organisation oder für den jeweiligen Benutzer aktiviert ist, führen Sie die folgenden Schritte aus.

1. Melden Sie sich beim [Microsoft 365 Compliance Center](https://protection.office.com/) an.

2. Klicken Sie auf **"Suchen und Untersuchung",** und wählen Sie **"Überwachungsprotokollsuche" aus.**

3. Wählen Sie den Datumsbereich in den Feldern **Startdatum** und Enddatum aus.  Geben Sie den Benutzernamen für den Benutzer an, den Sie untersuchen möchten (den Benutzer, der die Elemente gelöscht hat). Wählen Sie im Feld **"Aktivitäten"** die Option **"Gelöschte Nachrichten" aus dem Ordner "Gelöschte Elemente"** und "Nachrichten in ordner **"Gelöschte Elemente" verschoben** aus.

4. Klicken Sie auf **Suchen**.

Wählen Sie in den Ergebnissen einen Überwachungsdatensatz aus. Klicken Sie im Flyout "Details" auf **"Weitere Informationen".** Zusätzliche Informationen zum gelöschten Element (z. B. die Betreffzeile und der Speicherort des Elements, als es gelöscht wurde) werden im **AffectedItems-Feld** angezeigt. Die **ClientInfoString-Eigenschaft** zeigt an, ob der Löschvorgang in Outlook, Outlook im Web (früher als Outlook Web App bezeichnet) oder einem anderen Gerät erfolgt ist.

Weitere Informationen finden Sie unter [Ermitteln, wer die E-Mail-Weiterleitung für ein Postfach eingerichtet hat.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)

**Hinweis:** Sie können gelöschte Elemente nicht mithilfe der Überwachungsprotokollfunktion abrufen. Informationen zum Abrufen gelöschter Nachrichten in Outlook im Web finden Sie unter [Wiederherstellen gelöschter Elemente in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
