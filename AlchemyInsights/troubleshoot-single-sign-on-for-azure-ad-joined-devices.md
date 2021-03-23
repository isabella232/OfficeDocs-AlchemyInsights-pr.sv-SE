---
title: Felsöka enkel inloggning för Azure AD-anslutna enheter
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037334"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Felsöka enkel inloggning för Azure AD-anslutna enheter

Om du har en lokal Active Directory-miljö (AD) och du vill ansluta dina AD-domänkopplingsdatorer till Azure AD kan du göra det genom att göra en hybridkoppling av Azure AD. [Så här gör du: Planera din hybrid-Azure Active](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) Directory-kopplingsimplementering ger dig relaterade steg för att implementera en hybrid-Azure AD-koppling i din miljö.

Mer information finns i Konfigurera [Azure AD-anslutna enheter för](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)lokala enheter Single-Sign På med Windows Hello för företag.

**Problem med primär uppdateringstoken (PRT)**

En primär uppdateringstoken (PRT) är en viktig artefakt av Azure AD-autentisering på Windows 10-, Windows Server 2016- och senare versioner, iOS- och Android-enheter. Det är en JSON Web Token (JWT) som utfärdats speciellt till Microsoft-tokenförmedlare för att aktivera enkel inloggning (SSO) i de program som används på dessa enheter. Mer information om hur en PRT utfärdas, används och skyddas på Windows 10-enheter finns i Vad är en [primär uppdateringstoken?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: YES och AzureADPrt: YES**

De här fälten anger om användaren har autentiserats till Azure AD när du loggar in på enheten. Om värdena inte är **det** kan det bero på följande:

- Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)
- Alternativt inloggnings-ID
- DET går inte att hitta HTTP-proxy

Information om hur du felsöker enheter med DSREGCMD-kommandot finns [i SSO-tillstånd.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
