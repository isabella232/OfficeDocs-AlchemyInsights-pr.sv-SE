---
title: 646 så här konfigurerar du AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704507"
---
# <a name="configure-sync-features"></a><span data-ttu-id="5ec57-102">Konfigurera synkroniseringsfunktionen</span><span class="sxs-lookup"><span data-stu-id="5ec57-102">Configure sync features</span></span>

<span data-ttu-id="5ec57-103">Azure AD Connect innehåller flera funktioner som är aktiverade som standard eller som du kan aktivera senare.</span><span class="sxs-lookup"><span data-stu-id="5ec57-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="5ec57-104">För vissa funktioner krävs ytterligare konfiguration i specifika miljöer.</span><span class="sxs-lookup"><span data-stu-id="5ec57-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="5ec57-105">[Filtrering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) begränsar objekten synkroniseras till Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5ec57-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="5ec57-106">Som standard synkroniseras alla användare, kontakter, grupper och Windows 10-dator konton.</span><span class="sxs-lookup"><span data-stu-id="5ec57-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="5ec57-107">Du kan ta med eller utesluta objekt baserat på domäner, organisationsenheter eller andra attribut.</span><span class="sxs-lookup"><span data-stu-id="5ec57-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="5ec57-108">[Lösenordsskyddade lösen ord](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synkroniserar lösen ords-hashvärdet från den lokala Active Directory till Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5ec57-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="5ec57-109">Detta tillåter lösen ords hantering på en och samma plats men använder samma lösen ord i både lokala och moln miljöer.</span><span class="sxs-lookup"><span data-stu-id="5ec57-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="5ec57-110">Eftersom Active Directory är en auktoritativ källa kan du använda dina egna lösen ords principer.</span><span class="sxs-lookup"><span data-stu-id="5ec57-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="5ec57-111">Med [självbetjäning för återställning av lösen ord (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) kan användare återställa sina egna lösen ord i molnet och ändå tillämpa din lokala lösen ords princip.</span><span class="sxs-lookup"><span data-stu-id="5ec57-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="5ec57-112">Med funktionen för att [Ångra](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) kan registrerade enheter i Azure AD skrivas tillbaka till den lokala Active Directory så att de är avsedda för villkorlig åtkomst.</span><span class="sxs-lookup"><span data-stu-id="5ec57-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="5ec57-113">[Förhindra att oavsiktlig borttagning](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) är aktiverat som standard för att förhindra alltför många objekt borttagningar samtidigt (fler än 500 objekt per synkronisering).</span><span class="sxs-lookup"><span data-stu-id="5ec57-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="5ec57-114">Du kan ändra den här inställningen för att uppfylla organisationens behov.</span><span class="sxs-lookup"><span data-stu-id="5ec57-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="5ec57-115">[Automatisk uppgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) är aktiverat som standard för Express installationer och säkerställer att din version av Azure AD Connect alltid är aktuell.</span><span class="sxs-lookup"><span data-stu-id="5ec57-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
