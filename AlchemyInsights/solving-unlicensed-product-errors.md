---
title: Beheben von Fehlern bei nicht lizenzierten Produkten
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: ab2b2feb91bb803ad07dff82ea56a5778e547f9e
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63291339"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Vorschläge zum Beheben von Fehlern beim "nicht lizenzierten Produkt"

Um Fehler bei einem "nicht lizenzierten Produkt" zu beheben, versuchen Sie Folgendes:

- Überprüfen Sie, ob Ihr Abonnementstatus abgelaufen ist.
- Stellen Sie sicher, dass Sie über ein Abonnement verfügen, das Clientlizenzen zulässt, z. B. Microsoft 365 Apps for Business oder Business Premium, und [stellen Sie sicher, dass dem Benutzer eine Lizenz zugewiesen ist](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). 
- Stellen Sie sicher, dass sich der Benutzer bei Office mit demselben Konto anmeldet, dem die Lizenz zugewiesen ist.
- Überprüfen Sie die [Seite "Dienstintegrität](https://docs.microsoft.com/office365/enterprise/view-service-health) ", um festzustellen, ob bekannte Probleme mit dem Dienst vorliegen.
- Überprüfen Sie ihre Firewall-, Antivirensoftware- und Proxyeinstellungen, um sicherzustellen, dass sie Microsoft 365 Apps den Zugriff auf das Internet nicht blockieren. Siehe [URLs und IP-Adressbereiche](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

Sie können auch die folgenden Problembehandlungsaktionen ausprobieren: 

- Öffnen Sie eine Office-App, und [melden Sie sich](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) von vorhandenen Benutzerkonten ab. [Entfernen Sie](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) die Office-Lizenz, [weisen Sie sie erneut](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) zu, und [melden Sie sich](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) dann mit dem betroffenen Benutzerkonto bei Office an.
- Führen Sie die [Aktivierungsproblembehandlung aus](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Setzen Sie den Office-Aktivierungsstatus zurück](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Führen Sie eine Onlinereparatur von Office durch](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

Zusätzliche Lösungen zur Problembehandlung finden Sie unter: 

- [Fehler "Nicht lizenziertes Produkt" und Aktivierungsfehler in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [Fehler "Leider können wir keine Verbindung mit Ihrem Konto herstellen. Versuchen Sie es bitte später erneut" bei der Aktivierung von Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)