---
title: Verwenden des Office-Bereitstellungstools
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 2e4953d8fb339031bb3b82c53e4da3920ef45320
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61965084"
---
# <a name="using-the-office-deployment-tool-odt"></a>Verwenden des Office-Bereitstellungstools (ODT)

Sie verwenden das Office Deployment Tool (ODT), um Office 365 Versionen von Office bereitzustellen. Das Office-Bereitstellungstool (setup.exe) wird über die Befehlszeile ausgeführt und verwendet eine XML-Konfigurationsdatei, um zu bestimmen, welche Einstellungen bei der Bereitstellung von Office angewendet werden sollen.
  
1. Laden Sie die neueste Version des Office-Bereitstellungstools aus dem [Microsoft Download Center herunter.](https://go.microsoft.com/fwlink/p/?LinkID=626065)

2. Verwenden Sie das [Office Customization Tool (OCT),](https://config.office.com) um Ihre Bereitstellungseinstellungen auszuwählen und die XML-Konfigurationsdatei zu erstellen. Exportieren Sie die Konfigurationsdatei, und platzieren Sie sie lokal im selben Ordner, in dem sich der setup.exe befindet.

    **Hinweis:** Office Installationsprobleme treten häufig aufgrund falsch konfigurierter oder falsch formatierter Konfigurationsdateien auf. Um solche Probleme zu vermeiden, empfehlen wir, das Office Anpassungstool zum Erstellen der Konfigurationsdatei zu verwenden. Sie können auch vorhandene Konfigurationsdateien in das Office Anpassungstool importieren.

3. Wechseln Sie an einer Eingabeaufforderung mit erhöhten Rechten zu dem Speicherort, an dem sich setup.exe befindet, und führen Sie das Office Bereitstellungstool im Downloadmodus aus, und geben Sie die Konfigurationsdatei an, die Sie gerade gespeichert haben. In diesem Beispiel heißt die Konfigurationsdatei Configuration.xml:

```setup.exe /download Configuration.xml```

4.Führen Sie das Office-Bereitstellungstool im Konfigurationsmodus aus, und geben Sie die Konfigurationsdatei an.

```setup.exe /configure Configuration.xml```

**Hinweis:** Sie müssen diesen Schritt auf dem Clientcomputer ausführen, auf dem Sie Office installieren möchten, und Sie müssen über lokale Administratorberechtigungen auf diesem Computer verfügen.

Weitere Informationen zur Verwendung Office Bereitstellungstools für Ihre Microsoft 365 Apps for Enterprise Bereitstellungsszenarien finden Sie unter ["Übersicht über das Office-Bereitstellungstool".](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool) Weitere Informationen zur Verwendung des tools zum anpassen von Office finden Sie unter [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
