---
title: Identifizieren von Löschnachrichtenereignissen in Überwachungsprotokollen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: fdd25ee3017092a6f43618c1928cc83108adb7c0
ms.sourcegitcommit: c2b6eee90fbce71e65b4f7e95979344d875adc61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2022
ms.locfileid: "65588691"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Überwachungsprotokolle für gelöschte E-Mail-Nachrichten

Ab Januar 2019 aktiviert Microsoft standardmäßig die Postfachüberwachungsprotokollierung. Andernfalls müssen Sie zum Überprüfen von Löschnachrichtenereignissen für einen bestimmten Benutzer die Löschaktionen für die Überwachung manuell aktivieren. Wenn die Postfachüberwachungsprotokollierung für Ihre Organisation oder für den jeweiligen Benutzer bereits aktiviert ist, führen Sie die folgenden Schritte aus.

1. Führen Sie einen der folgenden Schritte aus:
   - Wechseln Sie in der Microsoft Purview-Complianceportal unter <https://compliance.microsoft.com>zu **"Lösungsüberwachung"**\>. Oder verwenden Sie <https://compliance.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.
   - Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com> zu **Überwachung**. Oder verwenden Sie <https://sip.security.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.

2. Vergewissern Sie sich, auf der Seite **Überwachung**, dass die Registerkarte **Suche** ausgewählt ist, und konfigurieren Sie dann die folgenden Einstellungen:
   - Wählen Sie den Datums-/Uhrzeitbereich in den Feldern **"Start** " und " **Ende** " aus.
   - **Aktivitäten**: Wählen Sie **"Gelöschte Nachrichten" aus dem Ordner "Gelöschte Elemente"** und **"Verschobene Nachrichten" in den Ordner "Gelöschte Elemente"** aus.
   - **Benutzer**: Geben Sie den zu untersuchenden Benutzernamen an (der Benutzer, der die Elemente gelöscht hat).

3. Wenn Sie den Vorgang abgeschlossen haben, klicken Sie auf **Suchen**. Die Aktivitäten werden auf der neuen Seite **Suche überwachen** angezeigt.

4. Wählen Sie in den Ergebnissen einen Überwachungsdatensatz aus. Im daraufhin angezeigten Detailflyout werden zusätzliche Informationen zum gelöschten Element (z. B. die Betreffzeile und die Position des Elements beim Löschen) im Feld **"AffectedItems** " angezeigt. Die **ClientInfoString-Eigenschaft** zeigt an, ob der Löschvorgang in Outlook, Outlook im Web (früher als Outlook Web App bezeichnet) oder auf einem anderen Gerät erfolgt ist.

Weitere Informationen finden Sie unter [Ermitteln, wer die E-Mail-Weiterleitung für ein Postfach eingerichtet](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items) hat.

**Hinweis**: Sie können gelöschte Elemente nicht mithilfe des Überwachungsprotokollfeatures abrufen. Informationen zum Abrufen gelöschter Nachrichten in Outlook im Web finden Sie unter [Wiederherstellen gelöschter Elemente in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
