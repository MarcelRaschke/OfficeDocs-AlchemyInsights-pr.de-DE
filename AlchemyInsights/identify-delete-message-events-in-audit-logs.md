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
ms.openlocfilehash: d2b2e3f2c8f6bc5c993afe11cfe5d813212a22ba
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62552115"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Überwachungsprotokolle für gelöschte E-Mail-Nachrichten

Ab Januar 2019 aktiviert Microsoft standardmäßig die Postfachüberwachungsprotokollierung. Andernfalls müssen Sie zum Überprüfen von Löschnachrichtenereignissen für einen bestimmten Benutzer die Löschaktionen manuell für die Überwachung aktivieren. Wenn die Postfachüberwachungsprotokollierung bereits für Ihre Organisation oder für den jeweiligen Benutzer aktiviert ist, führen Sie die folgenden Schritte aus.

1. Führen Sie einen der folgenden Schritte aus:
   - Wechseln Sie im Microsoft 365 Compliance Center unter <https://compliance.microsoft.com> zu **Lösungen** \> **Überwachung**. Oder verwenden Sie <https://compliance.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.
   - Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com> zu **Überwachung**. Oder verwenden Sie <https://sip.security.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.

2. Vergewissern Sie sich, auf der Seite **Überwachung**, dass die Registerkarte **Suche** ausgewählt ist, und konfigurieren Sie dann die folgenden Einstellungen:
   - Select the date/time range in the **Start** and **End** boxes.
   - **Aktivitäten**: Wählen Sie **"Gelöschte Nachrichten" aus dem Ordner "Gelöschte Elemente"** und **"Nachrichten in ordner "Gelöschte Elemente" verschoben** aus.
   - **Benutzer**: Geben Sie den zu untersuchenden Benutzernamen an (den Benutzer, der die Elemente gelöscht hat).

3. Wenn Sie den Vorgang abgeschlossen haben, klicken Sie auf **Suchen**. Die Aktivitäten werden auf der neuen Seite **Suche überwachen** angezeigt.

4. Wählen Sie in den Ergebnissen einen Überwachungsdatensatz aus. Im angezeigten Detail-Flyout werden zusätzliche Informationen zum gelöschten Element (z. B. die Betreffzeile und der Speicherort des Elements, als es gelöscht wurde) im **Feld "Betroffene Elemente** " angezeigt. Die **ClientInfoString-Eigenschaft** zeigt an, ob der Löschvorgang in Outlook, Outlook im Web (früher als Outlook Web App bezeichnet) oder einem anderen Gerät erfolgt ist.

Weitere Informationen finden Sie unter [Ermitteln, wer die E-Mail-Weiterleitung für ein Postfach eingerichtet](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items) hat.

**Hinweis**: Sie können gelöschte Elemente nicht mithilfe der Überwachungsprotokollfunktion abrufen. Informationen zum Abrufen gelöschter Nachrichten in Outlook im Web finden Sie unter ["Wiederherstellen gelöschter Elemente in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)".
