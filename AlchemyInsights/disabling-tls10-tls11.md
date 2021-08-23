---
title: Inaktivera TLS1.0 och TLS 1.1 för sändning med SMTP AUTH-klient
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13649"
- "9005383"
ms.openlocfilehash: 6751f4e8a177958fdec674899606252a4ae40a72
ms.sourcegitcommit: d9e6f700cd73a61c109e2a99bc71e559dba34722
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/18/2021
ms.locfileid: "58455126"
---
# <a name="disabling-tls10-and-tls-11-for-smtp-auth-client-submission"></a>Inaktivera TLS1.0 och TLS 1.1 för sändning med SMTP AUTH-klient

Vi har nyligen börjat inaktivera TLS1.0 och TLS 1.1 för sändning med SMTP AUTH-klient. 

Om du har konfigurerat en enhet, ett program eller en server som skickar e-post till Microsoft 365 med metoden för sändning via SMTP AUTH-klient kontrollerar du att enheten, programmet eller servern har stöd för TLS 1.2 för SMTP. 