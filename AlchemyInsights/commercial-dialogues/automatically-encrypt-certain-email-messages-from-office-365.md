---
title: Automatisches Verschlüsseln bestimmter E-Mail-Nachrichten aus Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9000078"
- "7342"
ms.date: 02/24/2021
ms.openlocfilehash: ce8dd9464079ae5720797675cbf70621eebbd9b7
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66357663"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>Automatisches Verschlüsseln bestimmter E-Mail-Nachrichten aus Office 365

1. Wählen Sie im [Exchange Admin Center](https://outlook.office365.com/ecp/) den **Nachrichtenfluss > Regeln** aus. 
2. Klicken Sie auf das Symbol **"Neu" (+)** und dann auf **"Office 365 Nachrichtenverschlüsselung und Rechteschutz auf Nachrichten anwenden**".
3. Geben Sie im **Namen** einen Namen für die Regel ein, z. B. *"Alle Nachrichten verschlüsseln*".
4. Wählen **Sie in "Diese Regel anwenden"** **die Option [Für alle Nachrichten übernehmen] aus**. 
5. Klicken Sie neben dem Feld **"Ausführen des folgenden** Felds" auf **"Eins auswählen"**. 
6. Wählen Sie im Dropdownmenü " **RMS-Vorlage** " die Option **"Verschlüsseln**" aus, und klicken Sie dann auf **"OK**". (Wenn diese Option nicht angezeigt wird, bedeutet dies, dass Ihr Plan keine automatische Verschlüsselung enthält. Aber Sie können es hinzufügen!)
7. Aktivieren Sie das Kontrollkästchen **"Diese Regel mit Schweregrad überwachen** ", und wählen Sie dann die gewünschte Ebene aus. Wenn Ihr Unternehmen vertragliche Verpflichtungen zum Senden aller verschlüsselten E-Mails hat, empfehle ich, die Stufe auf **"Hoch**" festzulegen.
8. Klicken **Sie unter "Modell für diese Regel auswählen**" auf **"Erzwingen"**. 
9. Wählen Sie eine beliebige optionale Auswahl aus (aus einer Liste optionaler Auswahlen, die Sie an diesem Punkt treffen können, von denen viele der Einfachheit halber mit der Standardeinstellung verbleiben können).
10. Klicken Sie auf **Speichern**.

**Wichtig**: Sie können diese Regel später immer wieder bearbeiten.

Weitere Informationen zum Erstellen von Verschlüsselungsregeln finden Sie unter [Definieren von Nachrichtenflussregeln zum Verschlüsseln von E-Mail-Nachrichten in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

