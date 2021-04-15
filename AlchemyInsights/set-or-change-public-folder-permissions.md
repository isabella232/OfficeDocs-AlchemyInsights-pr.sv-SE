---
title: Ange eller ändra behörigheter för gemensamma mappar
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: e419c72a890e68fc7b6d40d2b64406e42f9b0769
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51789225"
---
# <a name="permissions-and-public-folders"></a>Behörigheter och gemensamma mappar

Du kan ändra behörigheterna för dina gemensamma mappar med Outlook, Exchange admin center (EAC) eller PowerShell:
  
- För Outlook instruktioner klickar [du här](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).
    
- Anvisningar för EAC finns i [den här](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) artikeln. 
    
- Anvisningar för Powershell finns i [den här artikeln](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) om hur du använder Add-PublicFolderClientPermission-kommandoleten. Om du behöver anvisningar för att ansluta till Exchange Powershell klickar du [här](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).
    
Om **externa användare inte kan skicka e-postmeddelanden** till en e-postaktiverad offentlig mapp, kan orsaken vara att den gemensamma mappen saknar de behörigheter som krävs för extern e-postleverans. Du kan åtgärda detta med hjälp av [Outlook-instruktionerna här](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), eller PowerShell-instruktionerna [här](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).
  

