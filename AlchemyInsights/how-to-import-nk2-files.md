---
title: how-to-import-nk2-files
ms.author: daeite
author: daeite
manager: joallard
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "1800027"
- "1267"
ms.date: 04/21/2020
ms.openlocfilehash: 142c647baf18732cc738caab1d75216acf32a42f
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66353271"
---
# <a name="how-to-import-nk2-files"></a>Importieren von NK2-Dateien 

Wenn Sie Microsoft Outlook 2013, Outlook 2016, Outlook 2019 oder Outlook für Microsoft 365 zum ersten Mal starten, wird Ihr Spitznamencache (gespeichert in der Datei *"profilename.nk2*") in eine ausgeblendete Nachricht in Ihrem Standardnachrichtenspeicher importiert.

Um NK2-Dateien in Outlook 2013, Outlook 2016, Outlook 2019 oder Outlook für Microsoft 365 zu importieren, stellen Sie sicher, dass sich die NK2-Datei im folgenden Ordner befindet: %appdata%\Microsoft\Outlook

**Hinweis**: Die NK2-Datei muss denselben Namen wie Ihr aktuelles Outlook 2013- oder Outlook 2016-Profil aufweisen. Standardmäßig lautet der Profilname "Outlook". Führen Sie die folgenden Schritte aus, um den Profilnamen zu überprüfen: 
1. Klicken Sie auf **Start** und dann auf **Systemsteuerung**.
2. Doppelklicken Sie auf **"E-Mail**".
3. Wählen Sie im Dialogfeld "E-Mail-Setup" die Option **"Profile anzeigen"** aus.
4. Klicken Sie auf **Start** > **Ausführen**.
5. Geben Sie im Feld **"Öffnen** " *outlook.exe /importnk2* ein, und wählen Sie dann **"OK**" aus. 

Nachdem Sie die NK2-Datei importiert haben, werden die Inhalte der Datei mit dem vorhandenen Spitznamencache zusammengeführt, der in Ihrem Postfach gespeichert ist.

**Hinweis**: Die NK2-Datei wird beim nächsten Starten von Outlook 2013, Outlook 2016, Outlook 2019 oder Outlook für Microsoft 365 mit der Erweiterung ".old" umbenannt. Wenn Sie die NK2-Datei erneut importieren möchten, entfernen Sie zuerst die Erweiterung ".old".

Weitere Informationen finden Sie unter [Importieren oder Kopieren der AutoVervollständigen-Liste auf einen anderen Computer](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).