---
title: Laufwerkversand im Microsoft 365-Importdienst
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: c351d49e3eae1606a7000673eecc4a052ac450d3
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62623092"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a>Laufwerkversand im Microsoft 365-Importdienst

Verwenden Sie den Laufwerksversand, indem Sie die PSTs auf eine Festplatte kopieren und die Festplatte dann an Microsoft senden.

So starten Sie die Anfrage:

1. Wählen Sie im Microsoft 365 Compliance Center unter **Informationsgovernance** die Option **Importieren**.

1. Wählen Sie den **Typ des Importauftrags** aus und wählen Sie dann **Weiter**.

1. Wenn Sie die Schritte für diese Importoption sehen möchten, wählen Sie **Festplattenlaufwerke an einen unserer physischen Standorte versenden**.

Hier sind einige Dinge, die Sie beachten sollten:

- Ihnen muss die Rolle „Postfachimport/-export“ in Exchange Online zugewiesen sein, um PST-Dateien in Microsoft 365-Postfächer zu importieren. Bei PSTs mit mehr als 20 GB kann die Leistung beeinträchtigt werden.

- Nur 2,5-Zoll-Festkörperlaufwerke (SSDs) oder interne 2,5-/3,5-Zoll-SATA II/III-Festplatten werden unterstützt.
Eine Festplatte, die PST-Dateien enthält, muss mit BitLocker verschlüsselt werden.

- Die Kosten für das Importieren von PST-Dateien in Microsoft 365-Postfächer mithilfe des Laufwerkversands betragen 2 USD pro GB an Daten.

Weitere Informationen zur Verwendung der Laufwerkversandmethode für den Import von PST-Dateien finden Sie unter [Verwenden des Laufwerkversands zum Importieren der PST-Dateien Ihrer Organisation](https://docs.microsoft.com/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).