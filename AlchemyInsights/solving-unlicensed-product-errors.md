---
title: Beheben von Fehlern des nicht lizenzierten Produkts
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9001428"
- "3412"
ms.openlocfilehash: e8864c583152da0c45bfcceacd693d70fef08533
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66262846"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Vorschläge zum Beheben von Fehlern des "Nicht lizenzierten Produkts"

Um Fehler bei einem "Nicht lizenzierten Produkt" zu beheben, versuchen Sie Folgendes:

- Überprüfen Sie, ob Ihr Abonnementstatus abgelaufen ist.
- Stellen Sie sicher, dass Sie über ein Abonnement verfügen, das Clientlizenzen wie Microsoft 365 Apps for Business oder Business Premium zulässt, und [stellen Sie sicher, dass dem Benutzer eine Lizenz zugewiesen ist](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). 
- Stellen Sie sicher, dass sich der Benutzer bei Office mit demselben Konto anmeldet, dem die Lizenz zugewiesen ist.
- Überprüfen Sie die [Seite Dienststatus](https://docs.microsoft.com/office365/enterprise/view-service-health), um festzustellen, ob bekannte Probleme mit dem Dienst vorliegen.
- Überprüfen Sie Ihre Firewall-, Antivirensoftware- und Proxyeinstellungen, um sicherzustellen, dass sie den Zugriff auf das Internet von Microsoft 365-Apps nicht blockieren. Siehe [URLs und IP-Adressbereiche](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

Sie können auch die folgenden Problembehandlungsaktionen ausprobieren: 

- Öffnen Sie eine Office-App, und [melden Sie sich von](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) vorhandenen Benutzerkonten ab. [Entfernen Sie](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) die [Office-Lizenz](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) , weisen Sie sie erneut zu, und [melden Sie sich](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) dann mit dem betroffenen Benutzerkonto bei Office an.
- Führen Sie die [Aktivierungsproblembehandlung](https://aka.ms/SARA-OfficeActivation-Alchemy) aus.
- [Setzen Sie den Office-Aktivierungsstatus zurück](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Führen Sie eine Onlinereparatur von Office durch](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

Zusätzliche Lösungen zur Problembehandlung finden Sie unter: 

- [Fehler "Nicht lizenziertes Produkt" und Aktivierungsfehler in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [Fehler "Leider können wir keine Verbindung mit Ihrem Konto herstellen. Versuchen Sie es bitte später erneut" bei der Aktivierung von Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)