---
title: Blockieren von vom Benutzer erstellten E-Mail-Signaturen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: ad743cea4b8735b35b90bd5bf3d0b5b933184ed82858e828a68beb2ca2f8270c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54103551"
---
# <a name="block-user-made-email-signatures"></a>Blockieren von vom Benutzer erstellten E-Mail-Signaturen

Die folgende Lösung gilt nur für E-Mail-Signaturen, die in Outlook im Web erstellt wurden. Sie können Signaturen in der Outlook App nur blockieren, wenn Sie über eine lokale Exchange Server verfügen.

1. Wählen Sie im Admin Center **Admin Center**  >  **Exchange** aus.
2. Klicken Sie auf **Berechtigungen**  >  **Outlook Web App Richtlinien.**
3. Wählen Sie die Richtlinie aus, und klicken Sie dann auf das Stiftsymbol, um sie zu bearbeiten.
4. Klicken Sie auf **"Features**  >  **Weitere Optionen".**
5. Deaktivieren Sie unter **"Benutzererfahrung"** das Kontrollkästchen **"E-Mail-Signatur",** und klicken Sie dann auf **"Speichern".**

**Wichtig:** Wenn vor dem Deaktivieren dieses Kontrollkästchens eine Signatur hinzugefügt wurde, kann der Benutzer sie weiterhin verwenden. Bitten Sie sie, es zu entfernen.
