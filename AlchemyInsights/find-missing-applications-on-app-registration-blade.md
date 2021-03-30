---
title: Hitta program som saknas på registreringsbladet för appar
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
- "9004352"
- "9654"
ms.openlocfilehash: 00b5821e2edad8b60ff60b1f85264d81c72277e4
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405222"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Hitta program som saknas på registreringsbladet för appar

1. Det går inte att hitta program på registreringsportalen för appar.

    Om ett program är ett program med flera innehavare och det har registrerats i en annan klientorganisation visas det inte under Blad för appregistrering. Men du kan hitta det under Enterprise Applications-bladet när det har använts (efter medgivande) och tjänstens huvudnamn har skapats i klientorganisationen. Mer information finns i Artikeln [& tjänsthuvudnamn i Azure AD – Microsoft Identity Platform.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
2. Det går inte att visa appar i blad för appregistrering trots att du är administratör.

    Se till att du är i rätt katalog på Azure Portal.
3. Mitt program visas inte under bladet för företagsprogram men det visas när jag kör en fråga för PowerShell-kommandot.

    Ibland när du har tagit bort programmet från Azure Portal visas det inte i portalen, men det kanske inte har tagits bort helt. Mer information finns i:
    - Du kan hämta listan med tidigare borttagna program och se om programmet visas i listan med hjälp av **Powershell-kommandot: Get-AzureADDeletedApplication**. Mer information finns i [Get-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)
    - Om du vill ta bort programmet helt kan du prova följande i PowerShell: **Remove-AzureADApplication -ObjectId**. Mer information finns i [Remove-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)
    - Du kan också försöka återställa det borttagna programmet med hjälp av följande Powershell-kommando: **Restore AzureADDeletedApplication -ObjectId**. Mer information finns i [Restore-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
4. Det går inte att hitta listan över alla förinstallerade företagsprogram i min nya Azure-klient.

    Det finns inga förinstallerade företagsprogram i Azure AD som standard. Du måste lägga till det manuellt via alternativet Nytt program genom att gå igenom det från Azure AD-galleriet eller lägga till ett program som inte är galleriprogram. Mer information finns i [Snabbstart: Lägga till ett program i Azure Active Directory-klientorganisationen (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    Om du är global administratör kan du enkelt komma åt dina appar med hjälp av [startprogrammet för Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher)
5. Det går inte att hitta mina appar från Mina appar-portalen.

    Kontrollera att apparna inte är dolda på samlingssidan Mina program. Mer information finns i [Samlingar (förhandsversion) i Mina appar-portalen – Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections)
6. Information om hur du startar appar från portalen Mina appar finns [i Hitta & använda appar i Portalen Mina appar – Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access)
7. Office 365 Mover-appen visas inte i bladet Företagsprogram efter installationen.

    Programmet "Office 365 Mover" är ett flerprogram som inte behöver läggas till i AAD med hjälp av avsnittet Galleriprogram under Registrering av företagsappar. För att få åtkomst till Office 365 Mover-appen loggar du bara in på appen och ber användaren om medgivande för behörigheterna. När användaren ger medgivande läggs det här programmet automatiskt till i klientorganisationen med det e-post-ID du har loggat in.

    När du har loggat in i programmet bör du kunna hitta den här appens post under Enterprise Applications-bladet i AAD. Du behöver söka efter programmet genom att antingen skriva det fullständiga namnet, det vill säga "Office 365 Mover", eller genom att helt enkelt söka på "office" så ska programmet listas. Mer information finns i [Office 365 Mover säger](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)att det redan är installerat, men det visas inte i galleriet för företagsprogram.
8. Snabbstart: Visa listan över program som använder [Azure Active Directory-klientorganisationen (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) för identitetshantering visar hur du visar de program, även kallade appar, som redan är konfigurerade för att använda Azure AD-klientorganisationen som sin identitetsprovider (IdP).
9. [Felsöka vanliga problem med att lägga till eller ta](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) bort ett program i Azure Active Directory så att du förstår vilka problem som kan uppstå med att visa appar i Azure Active Directory.
