---
title: Importieren und Exportieren von Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: 26fa78aebdd8cf2ace9652d6b1a0a9c4430fb198
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65720177"
---
# <a name="import-and-export-from-yammer"></a>Importieren und Exportieren von Yammer

**Importieren**

Die Optionen für den Benutzerimport variieren je nachdem, ob sich Ihr Yammer-Netzwerk im [Nativen Modus für Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode) befindet oder nicht.

- **Nicht nativer Modus**: Benutzer können mithilfe der Option [Aus Adressbuch hinzufügen](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (maximal 100 Benutzer) in den Gruppeneinstellungen in Gruppen oder mithilfe der [Massenaktualisierung](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) innerhalb des Netzwerkadministrators in das Netzwerk importiert werden.
- **Nativer Modus**: Gruppenmitgliedschafts- und Netzwerkmitgliedschaftsvorgänge sollten über das [Microsoft 365-Administratorportal](https://docs.microsoft.com/microsoft-365/admin/add-users), das [Azure AD-Portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) oder mithilfe einer anderen Azure AD-Option ausgeführt werden. Netzwerke im nativen Modus haben keinen Zugriff mehr auf Massenaktualisierungen und andere ältere Features.

    **Wichtig**: Yammer hat das Importieren von Inhalten aus dem Netzwerkadministrator nie unterstützt, selbst wenn das Datenexportfeature in einem anderen Netzwerk verwendet wurde. Inhalte können von Partnerlösungen oder den Yammer-REST-APIs erneut veröffentlicht werden.

**Export**

[Das Exportieren von Netzwerkdaten innerhalb von Netzwerkadministratoren](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) ermöglicht den Export von Inhalten aus Yammer-Netzwerken, einschließlich Nachrichten und Dateien. Anhänge können sehr groß sein und dazu führen, dass der Export viel Zeit in Anspruch nimmt. Wir empfehlen, aktive Netzwerke mithilfe der [Datenexport-API](https://developer.yammer.com/docs/data-export-api) in Blöcken nach Tag oder Woche zu exportieren. Der Microsoft-Support bietet zu diesem Zweck keine benutzerdefinierten Skripts an.

Es gibt einen separaten [GDPR-Export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise), um Inhalte für einen individuellen Benutzer zu exportieren.