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
ms.localizationpriority: medium
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: ad99f311c6708ffd92697287cb985c1f193eabca
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63176719"
---
# <a name="using-the-office-deployment-tool-odt"></a>Verwenden des Office-Bereitstellungstools (ODT)

Sie verwenden das Office Deployment Tool (ODT), um Office 365 Versionen von Office bereitzustellen. Das Office-Bereitstellungstool (setup.exe) wird über die Befehlszeile ausgeführt und verwendet eine XML-Konfigurationsdatei, um zu bestimmen, welche Einstellungen bei der Bereitstellung von Office angewendet werden sollen.
  
1. Laden Sie die neueste Version des Office-Bereitstellungstools aus dem [Microsoft Download Center herunter](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Verwenden Sie das [Office Customization Tool (OCT),](https://config.office.com) um Ihre Bereitstellungseinstellungen auszuwählen und die XML-Konfigurationsdatei zu erstellen. Exportieren Sie die Konfigurationsdatei, und platzieren Sie sie lokal in demselben Ordner, in dem sich die setup.exe befindet.

    **Hinweis:** Office Installationsprobleme treten häufig aufgrund falsch konfigurierter oder falsch formatierter Konfigurationsdateien auf. Um solche Probleme zu vermeiden, empfehlen wir, dass Sie das Office-Anpassungstool verwenden, um die Konfigurationsdatei zu erstellen. Sie können vorhandene Konfigurationsdateien auch in das Anpassungstool für Office importieren.

3. Wechseln Sie an einer Eingabeaufforderung mit erhöhten Rechten zu dem Speicherort, an dem sich setup.exe befindet, und führen Sie das Office Bereitstellungstool im Downloadmodus aus, und geben Sie die Konfigurationsdatei an, die Sie gerade gespeichert haben. In diesem Beispiel heißt die Konfigurationsdatei Configuration.xml:

```setup.exe /download Configuration.xml```

4.Führen Sie das Office-Bereitstellungstool im Konfigurationsmodus aus, und geben Sie die Konfigurationsdatei an.

```setup.exe /configure Configuration.xml```

**Hinweis:** Sie müssen diesen Schritt auf dem Clientcomputer ausführen, auf dem Sie Office installieren möchten, und Sie müssen über lokale Administratorberechtigungen auf diesem Computer verfügen.

Weitere Informationen zur Verwendung Office Bereitstellungstools für Ihre Microsoft 365 Apps for Enterprise Bereitstellungsszenarien finden Sie unter ["Übersicht über das Bereitstellungstool für Office"](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Weitere Informationen zur Verwendung des Tools zum anpassen von Office finden Sie unter ["Übersicht über das Tool zum anpassen von Office"](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
