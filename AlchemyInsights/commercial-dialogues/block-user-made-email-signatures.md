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
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: 914edb63676bef0d03d1167ba1ac890a2e8c2a1e
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63227481"
---
# <a name="block-user-made-email-signatures"></a>Blockieren von vom Benutzer erstellten E-Mail-Signaturen

Die folgende Lösung gilt nur für E-Mail-Signaturen, die in Outlook im Web erstellt wurden. Signaturen in der Outlook-App können nur blockiert werden, wenn Sie über eine lokale Exchange Server verfügen.

1. Wählen Sie im Admin Center **Admin Center** >  **aus Exchange**.
2. Klicken Sie auf **Berechtigungen** >  **Outlook Web App Richtlinien**.
3. Wählen Sie die Richtlinie aus, und klicken Sie dann auf das Stiftsymbol, um sie zu bearbeiten.
4. Klicken Sie auf **"FeaturesMehr** >  **Optionen"**.
5. Deaktivieren Sie unter **"Benutzererfahrung**" das Kontrollkästchen " **E-Mail-Signatur** ", und klicken Sie dann auf **"Speichern**".

**Wichtig:** Wenn vor dem Deaktivieren dieses Kontrollkästchens eine Signatur hinzugefügt wurde, kann der Benutzer sie weiterhin verwenden. Bitten Sie sie, es zu entfernen.
