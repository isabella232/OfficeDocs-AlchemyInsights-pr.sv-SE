---
title: 646 Så här konfigurerar du AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722581"
---
# <a name="configure-sync-features"></a><span data-ttu-id="4a738-102">Konfigurera synkroniseringsfunktioner</span><span class="sxs-lookup"><span data-stu-id="4a738-102">Configure sync features</span></span>

<span data-ttu-id="4a738-103">Azure AD Connect innehåller flera funktioner som är aktiverade som standard eller som du kan aktivera senare.</span><span class="sxs-lookup"><span data-stu-id="4a738-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="4a738-104">Vissa funktioner kräver ytterligare konfiguration i specifika miljöer.</span><span class="sxs-lookup"><span data-stu-id="4a738-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="4a738-105">[Filtreringsgränser](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) objekten synkroniseras till Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4a738-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="4a738-106">Som standard synkroniseras alla användare, kontakter, grupper och Windows 10-datorkonton.</span><span class="sxs-lookup"><span data-stu-id="4a738-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="4a738-107">Du kan inkludera eller utesluta objekt baserat på domäner, ru:er eller andra attribut.</span><span class="sxs-lookup"><span data-stu-id="4a738-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="4a738-108">[Synkronisering av lösenord hash](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synkroniserar lösenordshhen från den lokala Active Directory till Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4a738-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="4a738-109">Detta möjliggör lösenordshantering på en plats, men användning av samma lösenord i både lokala miljöer och molnmiljöer.</span><span class="sxs-lookup"><span data-stu-id="4a738-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="4a738-110">Eftersom Active Directory är den auktoritära källan kan du använda dina egna lösenordsprinciper.</span><span class="sxs-lookup"><span data-stu-id="4a738-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="4a738-111">[Med självbetjäningslösenordsåterställning (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) kan användare återställa sina egna lösenord i molnet samtidigt som de tillämpar din lokala lösenordsprincip.</span><span class="sxs-lookup"><span data-stu-id="4a738-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="4a738-112">[Enhetsåterskrivning](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) gör att registrerade enheter i Azure AD kan skrivas tillbaka till den lokala Active Directory så att de kan användas för villkorlig åtkomst.</span><span class="sxs-lookup"><span data-stu-id="4a738-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="4a738-113">[Förhindra oavsiktliga borttagningar](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) är aktiverat som standard för att förhindra för många samtidiga objektborttagningar (fler än 500 objekt per synkronisering).</span><span class="sxs-lookup"><span data-stu-id="4a738-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="4a738-114">Du kan ändra den här inställningen så att den uppfyller organisationens behov.</span><span class="sxs-lookup"><span data-stu-id="4a738-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="4a738-115">[Automatisk uppgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) är aktiverad som standard för expressinstallationer och säkerställer att din version av Azure AD Connect alltid är aktuell.</span><span class="sxs-lookup"><span data-stu-id="4a738-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
