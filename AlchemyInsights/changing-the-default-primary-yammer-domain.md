---
title: Ändern der Yammer-Standarddomäne
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002662"
- "5162"
ms.openlocfilehash: 6a7215ef7187e8dc6c834470b4724692b239efd4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817975"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a>Ändern der standardmäßigen/primären Yammer-Domäne

Die Yammer-URL enthält den aktuellen primären Domänennamen für Ihr Yammer-Netzwerk. Dieser Domänenname stimmt mit dem in Office 365 oder Azure AD festgelegten primären Domänennamen möglicherweise nicht überein. Das Verhalten unterscheidet sich je nach der Anzahl der benutzerdefinierten Domänen, die dem Mandanten hinzugefügt wurden, und abhängig davon, ob sich Yammer in einer unterstützten Konfiguration (1 Mandant: 1 Netzwerk oder 1:1) befindet. Dokumentation zu [Yammer-Domänen und Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) steht zur Verfügung.

Der häufigste Grund für die Anzeige einer falschen Domäne: Es gibt mehrere Yammer-Netzwerke, die konsolidiert werden müssen. [Das Konsolidieren in ein einziges Netzwerk](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) mithilfe des Netzwerkmigrationstools ist ein wichtiger erster Schritt. Führen Sie ihn aus, bevor Sie versuchen, Ihre primäre Domäne festzulegen.

**Keine benutzerdefinierten Domänen**

Bei neuen Mandanten wird für Yammer die Standarddomäne (z. B. „fabrikam.onmicrosoft.com“) aus dem Mandanten verwendet. Die primäre Domäne wird auf „yammer.com/fabrikam.onmicrosoft.com“ festgelegt.

**Einzelne benutzerdefinierte Domäne**

Yammer wählt automatisch die benutzerdefinierte Domäne (z. B. „fabrikam.com“) aus dem Mandanten als primäre Domäne aus. Sie wird auf „yammer.com/fabrikam.com“ festgelegt. Diese Änderung wird vom Domänensynchronisierungsdienst vorgenommen, und es kann bis zu 24 Stunden dauern, bis sie wirksam wird.

**Mehrere benutzerdefinierte Domänen**

Bei Yammer kann es eine primäre Domäne geben, die sich von der Standardmandantendomäne unterscheidet. Da es mehrere benutzerdefinierte Domänen gibt, versucht Yammer nicht, die richtige Domäne aus den verfügbaren zu erraten. Sie müssen einen Supportfall öffnen, um anzufordern, dass der primäre Domänenname in die primäre Domäne Ihrer Wahl geändert wird.

**Zusätzliche Informationen zur Problembehandlung**

In einigen Fällen wurden Domänen möglicherweise zwischen Mandanten verschoben, und der Domänensynchronisierungsdienst konnte nicht erfolgreich ausgeführt werden. Vielleicht gibt es zusätzlich zu einer falschen primären Domäne Anmelde- oder andere Probleme. Zur Behebung dieses Problems müssen Domänen möglicherweise mithilfe des Microsoft-Supports in das richtige Netzwerk verschoben werden. Dies erfordert eine direkte Unterstützung, und die Behebung des Problems kann einige Zeit dauern – insbesondere, wenn es eine sehr lange Liste von Domänennamen gibt. Öffnen Sie einen Supportfall, um Unterstützung bei der Behebung dieser Arten von Problemen zu erhalten.

Bei der Arbeit mit einem Supportmitarbeiter wird geprüft, ob Domänen für einen Mandanten unter Ihrer Kontrolle überprüft werden. Vielleicht stellt er Ihnen zusätzliche Überprüfungsfragen zu Ihren Domänen, wenn sie Ihrem Mandanten hinzugefügt, aber nicht durch DNS überprüft werden. Stellen Sie bitte sicher, dass Domänen durch DNS überprüft werden, um den Vorgang zu beschleunigen.
