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
ms.openlocfilehash: 3dd198d4c264d930d0a0e3d87114d10eb6802f0b
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62762147"
---
# <a name="block-user-made-email-signatures"></a>Blockieren von vom Benutzer erstellten E-Mail-Signaturen

Die folgende Lösung gilt nur für E-Mail-Signaturen, die in Outlook im Web erstellt wurden. Sie können Signaturen in der Outlook App nur blockieren, wenn Sie über eine lokale Exchange Server verfügen.

1. Wählen Sie im Admin Center **Admin Center** >  **aus Exchange**.
2. Klicken Sie auf **Berechtigungen** >  **Outlook Web App Richtlinien**.
3. Wählen Sie die Richtlinie aus, und klicken Sie dann auf das Stiftsymbol, um sie zu bearbeiten.
4. Klicken Sie auf **"FeaturesMehr** >  **Optionen"**.
5. Deaktivieren Sie unter **"Benutzererfahrung**" das Kontrollkästchen " **E-Mail-Signatur** ", und klicken Sie dann auf **"Speichern**".

**Wichtig:** Wenn vor dem Deaktivieren dieses Kontrollkästchens eine Signatur hinzugefügt wurde, kann der Benutzer sie weiterhin verwenden. Bitten Sie sie, es zu entfernen.
