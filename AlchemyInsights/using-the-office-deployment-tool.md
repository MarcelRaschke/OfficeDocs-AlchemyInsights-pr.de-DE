---
title: Verwenden des Office-Bereitstellungstools
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "2000022"
- "918"
ms.date: 04/21/2020
ms.openlocfilehash: 117ce6c4ca19498cb478104b36a212523d03d68b
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66526315"
---
# <a name="using-the-office-deployment-tool-odt"></a>Verwenden des Office-Bereitstellungstools (ODT)

Sie verwenden das Office-Bereitstellungstool (OFFICE Deployment Tool, ODT), um Office 365 Versionen von Office bereitzustellen. Das Office-Bereitstellungstool (setup.exe) wird über die Befehlszeile ausgeführt und verwendet eine XML-Konfigurationsdatei, um zu bestimmen, welche Einstellungen bei der Bereitstellung von Office angewendet werden sollen.
  
1. Laden Sie die neueste Version des Office-Bereitstellungstools aus dem [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065) herunter.

2. Verwenden Sie das [Office-Anpassungstool (OCT),](https://config.office.com) um Ihre Bereitstellungseinstellungen auszuwählen und die XML-Konfigurationsdatei zu erstellen. Exportieren Sie die Konfigurationsdatei, und platzieren Sie sie lokal in dem Ordner, in dem sich die setup.exe befindet.

    **Hinweis:** Probleme bei der Office-Installation treten häufig aufgrund falsch konfigurierter oder falsch formatierter Konfigurationsdateien auf. Um solche Probleme zu vermeiden, empfehlen wir, die Konfigurationsdatei mithilfe des Office-Anpassungstools zu erstellen. Sie können auch vorhandene Konfigurationsdateien in das Office-Anpassungstool importieren.

3. Wechseln Sie an einer Eingabeaufforderung mit erhöhten Rechten zu dem Speicherort, an dem sich setup.exe befindet, führen Sie das Office-Bereitstellungstool im Downloadmodus aus, und geben Sie die soeben gespeicherte Konfigurationsdatei an. In diesem Beispiel heißt die Konfigurationsdatei Configuration.xml:

```setup.exe /download Configuration.xml```

4.Führen Sie das Office-Bereitstellungstool im Konfigurationsmodus aus, und geben Sie die Konfigurationsdatei an.

```setup.exe /configure Configuration.xml```

**Hinweis:** Sie müssen diesen Schritt auf dem Clientcomputer ausführen, auf dem Sie Office installieren möchten, und Sie müssen über lokale Administratorberechtigungen auf diesem Computer verfügen.

Weitere Informationen zur Verwendung des Office-Bereitstellungstools für Ihre Microsoft 365 Apps for Enterprise Bereitstellungsszenarien finden Sie [unter Übersicht über das Office-Bereitstellungstool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Weitere Informationen zur Verwendung des Office-Anpassungstools finden Sie [unter Übersicht über das Office-Anpassungstool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
