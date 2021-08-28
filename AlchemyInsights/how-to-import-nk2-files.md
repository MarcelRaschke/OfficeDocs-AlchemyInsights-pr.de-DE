---
title: How-to-import-nk2-files
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: f2b034926ec165b819119b5c4e060f10022d6017ec5dba8794d18ee3e96c709a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54043205"
---
# <a name="how-to-import-nk2-files"></a>Importieren von NK2-Dateien 

Wenn Sie Microsoft Outlook 2013, Outlook 2016, Outlook 2019 oder Outlook für Microsoft 365 zum ersten Mal starten, wird ihr Spitznamencache (gespeichert in der *NK2-Datei* des Profilnamens) in eine ausgeblendete Nachricht in Ihrem Standardnachrichtenspeicher importiert.

Um NK2-Dateien in Outlook 2013, Outlook 2016, Outlook 2019 oder Outlook für Microsoft 365 zu importieren, stellen Sie sicher, dass sich die NK2-Datei im folgenden Ordner befindet: %appdata%\Microsoft\Outlook

**Hinweis:** Die NK2-Datei muss denselben Namen wie Ihr aktuelles Outlook 2013- oder Outlook 2016-Profil aufweisen. Standardmäßig lautet der Profilname "Outlook". Gehen Sie folgendermaßen vor, um den Profilnamen zu überprüfen: 
1. Klicken Sie auf **Start** und dann auf **Systemsteuerung**.
2. Doppelklicken Sie auf **E-Mail**.
3. Wählen Sie im Dialogfeld E-Mail-Setup die Option **Profile anzeigen aus.**
4. Klicken Sie auf **Start** > **Ausführen**.
5. Geben Sie im **Feld "Öffnen"** *outlook.exe /importnk2* ein, und wählen Sie dann **OK** aus. 

Nachdem Sie die NK2-Datei importiert haben, wird der Inhalt der Datei mit dem vorhandenen Spitznamencache zusammengeführt, der in Ihrem Postfach gespeichert ist.

**Hinweis:** Die NK2-Datei wird beim nächsten Start Outlook 2013, Outlook 2016, Outlook 2019 oder Outlook für Microsoft 365 mit der Dateinamenerweiterung ".old" umbenannt. Wenn Sie die NK2-Datei erneut importieren möchten, entfernen Sie zuerst die Dateinamenerweiterung ".old".

Weitere Informationen finden Sie unter [Importieren oder Kopieren der AutoVervollständigen-Liste auf einen anderen Computer.](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%)