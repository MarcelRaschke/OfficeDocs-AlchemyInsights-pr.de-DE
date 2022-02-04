---
title: Office kann nicht aktiviert werden
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: 'NOINDEX, NOFOLLOW'
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
  - 2000023
  - 3509
---

# <a name="unable-to-activate-office"></a>Office kann nicht aktiviert werden

**Hinweis**: Wenn Sie eine ältere Version von Windows verwenden (z. B. Windows 7), stellen Sie sicher, dass TLS 1.2 als Standard aktiviert ist. Weitere Informationen finden Sie unter [Update zum Aktivieren von TLS 1.1 und TLS 1.2 als sichere Standardprotokolle in WinHTTP unter Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).

- Überprüfen Sie, ob Ihr Abonnementstatus abgelaufen ist.
- Stellen Sie sicher, dass Sie über ein Abonnement verfügen, das Clientlizenzen zulässt, z. B. Office 365 Business oder Business Premium, und [dass dem Benutzer eine Lizenz zugewiesen wurde](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users).
- Stellen Sie sicher, dass sich der Benutzer bei Office mit dem gleichen Konto anmeldet, dem die Lizenz zugewiesen wurde.
- Auf der Seite [Office 365 Service Health](https://docs.microsoft.com/office365/enterprise/view-service-health) werden mögliche bekannte Probleme mit dem Dienst angezeigt.
- Überprüfen Sie Ihre Firewall-, Antivirensoftware- und Proxyeinstellungen, um sich zu vergewissern, dass sie nicht den Zugriff auf das Internet für Microsoft 365-Apps blockieren. Weitere Informationen finden Sie unter [Office 365-URLs und IP-Adressbereiche](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365-URLs und -IP-Adressbereiche").

**Tipp** Auf Windows-Computern können wir mehrere häufige Probleme bei der Anmeldung bei Office für Sie diagnostizieren und automatisch beheben. Laden Sie den **[Microsoft Support- und Wiederherstellungs-Assistent](https://aka.ms/SaRA-OfficeSignInScenario)** herunter.

Ergreifen Sie die folgenden Maßnahmen zur Problembehandlung:

- Öffnen Sie eine Office-App, und [melden Sie sich von vorhandenen Benutzerkonten ab](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071). [Entfernen Sie die Office-Lizenz](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users), und [weisen Sie sie neu zu](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users), und [melden Sie sich dann unter Verwendung des betroffenen Benutzerkontos bei Office an](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9).
- Ausführen der [Aktivierungsproblembehandlung](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Zurücksetzen des Office-Aktivierungsstatus](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Zurücksetzen des Office-Aktivierungsstatus")
- [Ausführen einer Onlinereparatur von Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Zusätzliche Lösungen zur Problembehandlung finden Sie unter:  

- [Fehler "Nicht lizenziertes Produkt" und Aktivierungsfehler in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [Fehler "Leider können wir keine Verbindung mit Ihrem Konto herstellen. Versuchen Sie es bitte später erneut" bei der Aktivierung von Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)