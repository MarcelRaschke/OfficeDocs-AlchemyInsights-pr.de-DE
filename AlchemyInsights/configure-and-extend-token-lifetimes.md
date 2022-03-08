---
title: Konfigurieren und Verlängern der Tokengültigkeitsdauer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 78caa7ec3361344657429ce8351203e9639c85f2
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63267785"
---
# <a name="configure-and-extend-token-lifetimes"></a>Konfigurieren und Verlängern der Tokengültigkeitsdauer

Sie können die Gültigkeitsdauer für von Microsoft Identity Platform ausgestellte Zugriffs-, SAML- oder ID-Tokens angeben. Sie können die Tokengültigkeitsdauer für alle Apps in Ihrer Organisation festlegen, für eine mehrinstanzfähige (multiorganisatorische) Anwendung oder für einen bestimmten Dienstprinzipal in Ihrer Organisation. Weitere Informationen finden Sie unter [Konfigurierbare Tokengültigkeitsdauer](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

Beispiele finden Sie unter [Beispielen zur Konfiguration der Tokengültigkeitsdauer](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).

Wie Sie die Gültigkeitsdauer und Kompatibilität eines Tokens in Azure Active Directory B2C (Azure AD B2C) konfigurieren können, erfahren Sie unter [Konfigurieren von Token in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).

Der Artikel [Konfigurieren des Sitzungsverhaltens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) beschreibt die in Azure AD B2C verwendeten Methoden zum einmaligen Anmelden (Single Sign-On, SSO) und bietet Unterstützung bei der Auswahl der am besten geeigneten SSO-Methode bei der Konfiguration Ihrer Richtlinie.

**Wie lange bleiben die Token bestehen? Wie lange sind sie gültig?**

Die Tokengültigkeitsdauer beträgt 1 Stunde und die Sitzungsgültigkeitsdauer beträgt 24 Stunden. Das bedeutet, dass Sie sich erneut anmelden müssen, bevor Sie ein neues Token anfordern können, wenn innerhalb von 24 Stunden keine Anforderung erfolgt ist.

**Hinweis**: Nach dem 30. Mai 2020 können neue Mandanten die Richtlinie „Gültigkeitsdauer konfigurierbarer Token“ nicht mehr verwenden, um Sitzungs- und Aktualisierungstoken zu konfigurieren. Die Einstellung erfolgt in den nächsten Monaten, was bedeutet, dass bestehende Richtlinien für Sitzungs- und Aktualisierungstokens nicht mehr berücksichtigt werden. Sie können die Gültigkeitsdauer von Token auch nach der Einstellung noch konfigurieren.






