---
title: Website-Ermittlung durchführen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9005291"
- "9143"
ms.date: 03/08/2021
ms.openlocfilehash: 4e1bac726e9ceee5af027f431a3b39fa4a8b14ae
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66510600"
---
# <a name="do-site-discovery"></a>Website-Ermittlung durchführen

Falls in Ihrer Organisation noch ältere Webanwendungen genutzt werden und die Verwendung des Internet Explorer-Modus geplant ist (was auf die meisten Kunden zutrifft), sollten Sie etwas zusätzliche Website-Ermittlung durchführen.

**Sie haben bereits eine ältere Version von Microsoft Edge bereitgestellt**

Wenn Sie Ihre Enterprise-Websiteliste bereits für die ältere Version von Microsoft Edge konfiguriert haben, ist die Website-Ermittlung fast abgeschlossen. Wahrscheinlich müssen Sie nur noch neutrale Websites hinzufügen.

Neutrale Websites sind in der Regel Websites, die einmaliges Anmelden (Single Sign-On, SSO) bereitstellen. Wenn Sie zu einer neutralen Website über Microsoft Edge wechseln, möchten Sie zur Authentifizierung in Microsoft Edge bleiben. Wenn Sie im Internet Explorer-Modus zu einer neutralen Website wechseln, möchten Sie zur Authentifizierung im Internet Explorer-Modus bleiben.

Ermitteln Sie alle SSO- oder andere neutrale Websites, die Sie verwenden, und fügen Sie diese Ihrer Enterprise-Websiteliste hinzu.

**Internet Explorer ist Ihr Standardbrowser**

Wenn Sie derzeit nur Internet Explorer verwenden, wissen Sie möglicherweise nicht, welche Websites auf moderne Webstandards aktualisiert wurden, und für welche weiterhin Internet Explorer erforderlich ist. Sie sollten diese Websites ermitteln und der Enterprise-Websiteliste hinzufügen, damit der Internet Explorer-Modus nur für diese Websites verwendet werden kann.

**Hinweis**: Bei der [Unternehmenswebsiteermittlung](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) werden Websites ermittelt, für die möglicherweise der Internet Explorer-Modus benötigt wird. Dabei können Daten auf Computern mit Windows Internet Explorer 8 bis Internet Explorer 11 unter Windows 10, Windows 8.1 oder Windows 7 erfasst werden.

**Analysieren der Daten**

Nach deren Erfassung empfehlen wir die folgenden vier Schritte zum Analysieren der Daten:

1. Sortieren Sie die Daten nach Domäne und dann nach URL.
2. Definieren Sie die Grenzen einer App, die für den Internet Explorer-Modus konfiguriert werden soll. Ihr Ziel ist es, alle Websites und Websteuerelemente, die die App definieren, einzuschließen, jedoch keine zusätzlichen Websites und Steuerelemente. Einige Sites sind möglicherweise so einfach wie *<https://contoso.com/app1>*, während andere möglicherweise erfordern, dass Sie mehrere Websites und Seiten definieren.
3. Testen Sie die App, um zu verifizieren, dass sie nicht nativ funktioniert. Viele Websites stellen modernen Inhalt bereit, wenn sie einen modernen Browser erkennen, und älteren, wenn sie Internet Explorer erkennen.
4. Fügen Sie die App Ihrer Enterprise-Websiteliste hinzu, wenn der Test fehlschlägt.

**Hinweis**: Eine bewährte Methode beseht darin, alle Websites, die eine App umfassen, zu gruppieren. Auf diese Weise ist es einfacher, die gesamte Website aus dem Internet Explorer-Modus zu entfernen, wenn Sie ein Upgrade einer App durchführen, und mit der Verwendung eines modernen Browsers für diese App zu beginnen.

Nachdem Sie die Website-Ermittlung durchgeführt und die Daten analysiert haben, können Sie sich mit Ihrer Kanalstrategie befassen.
