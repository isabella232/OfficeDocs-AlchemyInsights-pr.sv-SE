---
title: Single-Sign på för Azure Active Directory-anslutna enheter
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405662"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Enkel inloggning för Azure Active Directory-anslutna enheter

Om du har en lokal Active Directory-miljö (AD) och du vill ansluta dina AD-domänkopplingsdatorer till Azure AD kan du göra det genom att göra en hybridkoppling av Azure AD. [Så här gör du: Planera din hybrid-Azure Active](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) Directory-kopplingsimplementering ger dig relaterade steg för att implementera en hybrid-Azure AD-koppling i din miljö.

[Konfigurera Azure AD-anslutna enheter för lokala enheter Single-Sign På med Windows Hello för företag](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Problem med primär uppdateringstoken (PRT)** En primär uppdateringstoken (PRT) är en viktig artefakt av Azure AD-autentisering på Windows 10-, Windows Server 2016- och senare versioner, iOS- och Android-enheter. Det är en JSON Web Token (JWT) som utfärdats speciellt till Microsoft-tokenförmedlare för att aktivera enkel inloggning (SSO) i de program som används på dessa enheter. [I Vad är en primär uppdateringstoken?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)tillhandahåller vi information om hur en PRT utfärdas, används och skyddas på Windows 10-enheter.

**WamDefaultSet: YES och AzureADPrt: YES** De här fälten anger om användaren har autentiserats till Azure AD när du loggar in på enheten. Om värdena inte är **det** kan det bero på följande:

- Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).
- Alternativt inloggnings-ID
- DET går inte att hitta HTTP-proxy

Felsöka enheter med kommandot dsregcmd – [SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
