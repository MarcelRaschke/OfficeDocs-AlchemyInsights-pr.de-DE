---
title: Beheben Microsoft 365 Apps konnte keine Office-Lizenzen zugeordnete Nachricht finden
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
- "3421"
- "9001426"
ms.openlocfilehash: 19b7868c4dd29e14e85ccda1223015a7a4db29cf
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63132185"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Beheben der Meldung "Office-Lizenzen konnten nicht gefunden werden" Microsoft 365 Apps

Wenn Sie diese Nachricht erhalten, versuchen Sie Folgendes:

1. Überprüfen Sie ihre Firewall-, Antivirensoftware- und Proxyeinstellungen, um sicherzustellen, dass sie den Internetzugriff auf Microsoft 365 Apps nicht blockieren. Siehe [Microsoft 365 URLs und IP-Adressbereiche](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Entfernen Sie [die Office-Lizenz](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) für den betroffenen Benutzer, und weisen Sie sie erneut zu. 
3. Öffnen Sie eine Office-App, und [melden Sie sich](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) von vorhandenen Benutzerkonten ab.
4. Wechseln Sie zu Windows Einstellungen > **AccountsEmail** >  **& Konten**, und entfernen Sie alle Geschäftskonten mit Ausnahme des betroffenen Kontos.
5. Wechseln Sie zu Windows Einstellungen > **AccountsAccess-Geschäfts** > -, Schul- oder Unikonto, und trennen Sie alle Geschäftskonten mit Ausnahme des betroffenen Kontos.
6. Setzen Sie den Office-Aktivierungsstatus zurück. [Anleitung](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Melden Sie sich](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) mit dem betroffenen Benutzerkonto an.

Weitere Problembehandlungslösungen finden Sie unter ["Nicht lizenziertes Produkt" und Aktivierungsfehler in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).