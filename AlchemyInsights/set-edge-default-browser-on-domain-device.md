---
title: Microsoft Edge als Standardbrowser auf einem domänenverbundenen Gerät festlegen
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: b66e0946260fc42ba8a4e4ad32e9ee558b40df86
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63212217"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a>Microsoft Edge als Standardbrowser auf einem domänenverbundenen Gerät festlegen

Legen Sie Microsoft Edge als Standardbrowser fest: 

1. [Erstellen Sie eine Konfigurationsdatei für Standardverknüpfungen](https://go.microsoft.com/fwlink/?linkid=2132437) und speichern Sie sie lokal oder auf einer Netzwerkfreigabe.

1. Öffnen Sie den Gruppenrichtlinien-Editor und gehen Sie dann zu **Computerkonfiguration** > **Administrative Vorlagen** > **Windows-Komponenten** > **Datei-Explorer**.

1. Wählen Sie **Konfigurationsdatei für Standardverknüpfungen festlegen**.

1. Wählen Sie **Richtlinieneinstellung**, und wählen Sie dann **Aktiviert**.

1. Geben Sie unter **Optionen** den Speicherort der Konfigurationsdatei für die Standardverknüpfungen ein und wählen Sie dann **OK**.
