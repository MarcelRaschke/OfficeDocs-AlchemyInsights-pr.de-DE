---
title: Verwalten der globalen Adressliste und des Offlineadressbuchs der Organisation
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: f0969c720f85b115fe703dc1ae0e8745337d2d44
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66432931"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a>Verwalten der globalen Adressliste (GAL) und des Offlineadressbuchs (OAB) der Organisation

Bei einer globalen Adressliste (GAL) handelt es sich um eine Liste von E-Mail-aktivierten Objekten (beliebige Arten von E-Mail-Empfängern) in der Organisation. Eine GAL wird in jeder Organisation automatisch erstellt. Sie können weitere GALs erstellen, um Benutzer nach Organisation oder Standort zu trennen, aber ein einzelner Benutzer kann nur jeweils eine GAL sehen und verwenden.

Einige E-Mail-Clients, z. B. Outlook für Windows, laden die GAL für die Offlinenutzung herunter. Dies wird als Offlineadressbuch (OAB) bezeichnet. In Exchange Online wird ein OAB nur einmal alle 8 Stunden aktualisiert, und dann muss es zum Aktualisieren der lokalen OAB-Kopie von den Clients heruntergeladen werden. Alle Empfängeränderungen müssen zuerst in der globalen Adressliste angezeigt werden, um sie später in ein OAB zu übernehmen.

Hier sind einige häufig verwendete GAL- und OAB-Verfahren:

- Aus einer Vielzahl von Gründen möchten Sie möglicherweise, dass einige Objekte in der globalen Adressliste verborgen sind. Weitere Informationen finden Sie unter [Empfänger aus Adressliste ausblenden](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).
- Wenn Sie bestimmten Benutzergruppen angepasste Ansichten der GAL der Organisation bereitstellen müssen, lesen Sie [Adressbuchrichtlinien in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).
- Informationen zum [Erstellen einer globalen Adressliste in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) und zum Arbeiten mit GAL-Berechtigungen finden Sie unter [Adresslisten in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists). Beachten Sie, dass Sie, wenn Sie neue GALs erstellen, möglicherweise auch ein neues OAB erstellen sollten. Siehe [Verfahren für Offlineadressbücher](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).
