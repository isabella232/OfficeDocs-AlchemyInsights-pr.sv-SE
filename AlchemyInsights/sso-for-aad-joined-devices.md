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
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="f76c6-102">Enkel inloggning för Azure Active Directory-anslutna enheter</span><span class="sxs-lookup"><span data-stu-id="f76c6-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="f76c6-103">Om du har en lokal Active Directory-miljö (AD) och du vill ansluta dina AD-domänkopplingsdatorer till Azure AD kan du göra det genom att göra en hybridkoppling av Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f76c6-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="f76c6-104">[Så här gör du: Planera din hybrid-Azure Active](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) Directory-kopplingsimplementering ger dig relaterade steg för att implementera en hybrid-Azure AD-koppling i din miljö.</span><span class="sxs-lookup"><span data-stu-id="f76c6-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="f76c6-105">Konfigurera Azure AD-anslutna enheter för lokala enheter Single-Sign På med Windows Hello för företag</span><span class="sxs-lookup"><span data-stu-id="f76c6-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="f76c6-106">**Problem med primär uppdateringstoken (PRT)** En primär uppdateringstoken (PRT) är en viktig artefakt av Azure AD-autentisering på Windows 10-, Windows Server 2016- och senare versioner, iOS- och Android-enheter.</span><span class="sxs-lookup"><span data-stu-id="f76c6-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="f76c6-107">Det är en JSON Web Token (JWT) som utfärdats speciellt till Microsoft-tokenförmedlare för att aktivera enkel inloggning (SSO) i de program som används på dessa enheter.</span><span class="sxs-lookup"><span data-stu-id="f76c6-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="f76c6-108">[I Vad är en primär uppdateringstoken?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)tillhandahåller vi information om hur en PRT utfärdas, används och skyddas på Windows 10-enheter.</span><span class="sxs-lookup"><span data-stu-id="f76c6-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="f76c6-109">**WamDefaultSet: YES och AzureADPrt: YES** De här fälten anger om användaren har autentiserats till Azure AD när du loggar in på enheten.</span><span class="sxs-lookup"><span data-stu-id="f76c6-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="f76c6-110">Om värdena inte är **det** kan det bero på följande:</span><span class="sxs-lookup"><span data-stu-id="f76c6-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="f76c6-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span><span class="sxs-lookup"><span data-stu-id="f76c6-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="f76c6-112">Alternativt inloggnings-ID</span><span class="sxs-lookup"><span data-stu-id="f76c6-112">Alternate Login ID</span></span>
- <span data-ttu-id="f76c6-113">DET går inte att hitta HTTP-proxy</span><span class="sxs-lookup"><span data-stu-id="f76c6-113">HTTP Proxy not found</span></span>

<span data-ttu-id="f76c6-114">Felsöka enheter med kommandot dsregcmd – [SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="f76c6-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
