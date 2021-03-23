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
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="e7a26-102">Felsöka enkel inloggning för Azure AD-anslutna enheter</span><span class="sxs-lookup"><span data-stu-id="e7a26-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="e7a26-103">Om du har en lokal Active Directory-miljö (AD) och du vill ansluta dina AD-domänkopplingsdatorer till Azure AD kan du göra det genom att göra en hybridkoppling av Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e7a26-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="e7a26-104">[Så här gör du: Planera din hybrid-Azure Active](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) Directory-kopplingsimplementering ger dig relaterade steg för att implementera en hybrid-Azure AD-koppling i din miljö.</span><span class="sxs-lookup"><span data-stu-id="e7a26-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="e7a26-105">Mer information finns i Konfigurera [Azure AD-anslutna enheter för](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)lokala enheter Single-Sign På med Windows Hello för företag.</span><span class="sxs-lookup"><span data-stu-id="e7a26-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="e7a26-106">**Problem med primär uppdateringstoken (PRT)**</span><span class="sxs-lookup"><span data-stu-id="e7a26-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="e7a26-107">En primär uppdateringstoken (PRT) är en viktig artefakt av Azure AD-autentisering på Windows 10-, Windows Server 2016- och senare versioner, iOS- och Android-enheter.</span><span class="sxs-lookup"><span data-stu-id="e7a26-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="e7a26-108">Det är en JSON Web Token (JWT) som utfärdats speciellt till Microsoft-tokenförmedlare för att aktivera enkel inloggning (SSO) i de program som används på dessa enheter.</span><span class="sxs-lookup"><span data-stu-id="e7a26-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="e7a26-109">Mer information om hur en PRT utfärdas, används och skyddas på Windows 10-enheter finns i Vad är en [primär uppdateringstoken?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="e7a26-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="e7a26-110">**WamDefaultSet: YES och AzureADPrt: YES**</span><span class="sxs-lookup"><span data-stu-id="e7a26-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="e7a26-111">De här fälten anger om användaren har autentiserats till Azure AD när du loggar in på enheten.</span><span class="sxs-lookup"><span data-stu-id="e7a26-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="e7a26-112">Om värdena inte är **det** kan det bero på följande:</span><span class="sxs-lookup"><span data-stu-id="e7a26-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="e7a26-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span><span class="sxs-lookup"><span data-stu-id="e7a26-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="e7a26-114">Alternativt inloggnings-ID</span><span class="sxs-lookup"><span data-stu-id="e7a26-114">Alternate Login ID</span></span>
- <span data-ttu-id="e7a26-115">DET går inte att hitta HTTP-proxy</span><span class="sxs-lookup"><span data-stu-id="e7a26-115">HTTP Proxy not found</span></span>

<span data-ttu-id="e7a26-116">Information om hur du felsöker enheter med DSREGCMD-kommandot finns [i SSO-tillstånd.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="e7a26-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
