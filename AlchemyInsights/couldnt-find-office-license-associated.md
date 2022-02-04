---
title: Beheben Microsoft 365 Apps konnte keine Office-Lizenzen zugeordnete Nachricht finden
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 9e0fbee833d79beffc6e7f7358158d910f498af7
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61972689"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Beheben der Meldung "Office-Lizenzen wurden nicht gefunden" Microsoft 365 Apps

Wenn Sie diese Nachricht erhalten, versuchen Sie Folgendes:

1. Überprüfen Sie ihre Firewall-, Antivirensoftware- und Proxyeinstellungen, um sicherzustellen, dass sie den Internetzugriff auf Microsoft 365 Apps nicht blockieren. Siehe [Microsoft 365 URLs und IP-Adressbereiche.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
2. Entfernen Sie [die Office-Lizenz](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) für den betroffenen Benutzer, und weisen Sie sie erneut zu. 
3. Öffnen Sie eine Office-App, und melden Sie sich von vorhandenen Benutzerkonten [ab.](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)
4. Wechseln Sie zu Windows Einstellungen >   >  **E-Mail-Konten & Konten,** und entfernen Sie alle Geschäftskonten mit Ausnahme des betroffenen Kontos.
5. Wechseln Sie zu Windows Einstellungen > **Konten**  >  **auf Geschäfts- oder Schulkonto zugreifen,** und trennen Sie alle Geschäftskonten mit Ausnahme des betroffenen Kontos.
6. Setzen Sie den Office-Aktivierungsstatus zurück. [Anleitung](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Melden Sie sich](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) mit dem betroffenen Benutzerkonto an.

Weitere Problembehandlungslösungen finden Sie unter ["Nicht lizenziertes Produkt" und Aktivierungsfehler in Office.](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)