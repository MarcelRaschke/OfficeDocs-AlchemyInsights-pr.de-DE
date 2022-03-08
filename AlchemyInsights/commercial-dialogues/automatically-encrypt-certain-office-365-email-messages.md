---
title: Automatische Verschlüsselung bestimmter Office 365 E-Mail-Nachrichten
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 05a098d7873888090d9c7a78a4b04b34ffea0078
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63186584"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a>Automatische Verschlüsselung bestimmter Office 365 E-Mail-Nachrichten

Sie können Nachrichten, die Benutzer an bestimmte externe Personen oder Organisationen senden, automatisch verschlüsseln. Führen Sie dazu die folgenden Schritte aus:

1. Wählen Sie im [Exchange Admin Center](https://outlook.office365.com/ecp/) den **Nachrichtenfluss > Regeln** aus. 
2. Klicken Sie auf das Symbol **"Neu" (+),** und klicken Sie dann auf **"Apply Office 365-Nachrichtenverschlüsselung und Rechteschutz für Nachrichten**".
3. Geben Sie in **"Name**" einen Namen für die Regel ein, z. B. *an DrToniRamos@gmail.com gesendete Nachrichten verschlüsseln*.
4. Wählen **Sie unter "Regel anwenden", wenn** **der Empfänger > diese Person ist**. 
5. Wählen Sie im Fenster **"Mitglieder auswählen** " den Namen der Person aus, auf die die Verschlüsselungsregel angewendet werden soll, und klicken Sie dann auf **"Hinzufügen**". 
6. Wenn Sie mit dem Hinzufügen von Benutzern fertig sind, klicken Sie auf **"OK**".
7. Next to the **Do the following** field, click **Select one**. 
8. Wählen Sie im Dropdownmenü der **RMS-Vorlage** **"Verschlüsseln**" aus, und klicken Sie dann auf **"OK**". (Wenn diese Option nicht angezeigt wird, bedeutet dies, dass Ihr Plan keine automatische Verschlüsselung umfasst. Aber Sie können es hinzufügen!)
9. Wählen Sie eine beliebige optionale Auswahl aus (aus einer Liste optionaler Auswahlen, die Sie an diesem Punkt treffen können, von denen viele der Einfachheit halber mit der Standardeinstellung übrig bleiben können).
10. Klicken Sie auf **Speichern**.

**Wichtig**: Sie können jederzeit zurückkehren und diese Regel später bearbeiten.

Weitere Informationen zum Erstellen von Regeln für die Verschlüsselung finden Sie unter [Definieren von Nachrichtenflussregeln zum Verschlüsseln von E-Mail-Nachrichten in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

