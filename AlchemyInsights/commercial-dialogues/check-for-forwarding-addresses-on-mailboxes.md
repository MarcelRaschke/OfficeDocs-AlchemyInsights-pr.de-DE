---
title: Überprüfen auf Weiterleitungsadressen in Postfächern
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9002486"
- "7524"
ms.date: 02/17/2021
ms.openlocfilehash: 5dff247df1380dffecd212b52f7abc3bdc849f41
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66272944"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a>Überprüfen auf Weiterleitungsadressen in Postfächern

Manchmal leiten Hacker die E-Mail-Nachrichten von Benutzern an sich selbst weiter, daher prüfen wir zuerst nach Weiterleitungsadressen und Regeln für das Postfach. Anschließend überprüfen wir die Überwachungsprotokolle. Hier erfahren Sie, wie Sie nach Weiterleitungsadressen suchen:

1. Wählen Sie **"Aktive Benutzer"** >  aus.
1. Wählen Sie den Benutzer aus, dessen Konto kompromittiert wurde.
1. Erweitern Sie im angezeigten Flyout die **E-Mail-Einstellungen**, und klicken Sie dann auf "Für **E-Mail-Weiterleitung** **bearbeiten**".
1. Entfernen Sie alle Weiterleitungsadressen, die Sie nicht erkennen.