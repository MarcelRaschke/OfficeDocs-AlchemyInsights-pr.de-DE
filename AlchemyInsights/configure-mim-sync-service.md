---
title: Konfigurieren des MIM Sync-Diensts
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: f834bead0b6f22dcadc808d45dcefe7f6571ef62c74b7fd97355157ca49542af
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53978484"
---
# <a name="configure-mim-sync-service"></a>Konfigurieren des MIM Sync-Diensts

Der MIM-Synchronisierungsdienst (Microsoft Identity Manager) ist eine Komponente von MIM. Es handelt sich um einen zentralisierten lokalen Dienst, der Informationen für Organisationen speichert und integriert, die über mehrere lokale Verzeichnisse und Datenbanken verfügen. Möglicherweise können Sie Ihr Problem mit MIM Sync beheben, wenn die Ursache in einem aktuellen Update für MIM behoben wurde oder eines der anderen im folgenden Abschnitt genannten Probleme ist.

**Empfohlene Schritte**

1. Stellen Sie sicher, dass Sie ein aktuelles Update von MIM Sync verwenden, und prüfen Sie in den [MIM Sync-Versionshinweisen](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history), ob das Problem in einem Update behoben wurde.
2. Wenn das Problem mit dem Generic LDAP-, Generic SQL-, Lotus Domino- oder Web Services-Connector auftritt, stellen Sie sicher, dass Sie ein aktuelles Update der [generischen Connectors](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history) verwenden.
3. Wenn eine MIM Sync-Ausführung mit einem Fehler abbricht, suchen Sie in der [Tabelle der Ausführungsfehlercodes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) nach den möglichen Ursachen.
4. Wenn die Ausführung mit **extension-dll-exception** abbricht, klicken Sie auf diese Worte, um das **Eigenschaftenfenster des Connectorbereichs** zu öffnen, und klicken Sie auf **Stapelüberwachung...**, um weitere Informationen über die zugrunde liegende Ursache zu erhalten, wie unter [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx) beschrieben.
5. Wenn die PCNS-Komponente (Password Change Notification Service) während der Kennwortsynchronisierung den **Fehler 6025** im Ereignisprotokoll meldet, lesen Sie die Anleitung zur Problembehandlung für [den Fehler 6025 in PCNS](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).
6. Wenn die vollständige Synchronisierung mit dem FIM-Dienstverwaltungs-Agent langsam ist, überprüfen Sie die **auto grow**-Einstellung für TempDB, wie in [Problembehandlung bei der langsamen oder hängenden vollständigen Synchronisierung](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx) beschrieben.
7. Wenn ein stopped-server-Fehler mit „failed-creation-via-web-services“ bei Verwendung des FIM-Dienstverwaltungs-Agents auftritt, finden Sie unter [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) eine Übersicht über die Ursachen.

