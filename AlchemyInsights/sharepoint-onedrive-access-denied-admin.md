---
title: Felsöka meddelanden om nekad åtkomst
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707972"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Felsöka meddelanden om nekad åtkomst i administrationscentret för Sharepoint/OneDrive

Om du får ett meddelande om nekad åtkomst när du försöker bläddra till ett administrationscenter för Sharepoint/OneDrive ska du se till att du tilldelar en [licens till användaren.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Om användaren har en licens bör du också kontrollera att de har [tilldelats en administratörsroll](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) som kan komma åt administratörscentrat.

Det här problemet kan också uppstå när en användare tas bort och på nytt skapas med samma huvudnamn (UPN). Det nya kontot skapas med ett annat PUID-värde (Passport Unique ID). När användaren försöker komma åt en webbplatssamling eller OneDrive har användaren ett felaktigt PUID. I det andra scenariot ingår katalogsynkronisering med organisationsenheten Active Directory (OU). Om användarna redan har loggat in på SharePoint och sedan flyttas till en annan OU och synkroniseras om med SharePoint kan det här problemet uppstå.

Lös problemet genom att återställa det ursprungliga UPN med stegen i artikeln Återställ [en användare i Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)

Obs! Om ett Administrationscenter för OneDrive eller SharePoint inte är tillgängligt för flera användare som tidigare har haft åtkomst kan det finnas ett tillfälligt problem med tjänsten.  [Kontrollera hälsoinstrumentpanelen för tjänster.](https://portal.office.com/adminportal/home#/servicehealth)


