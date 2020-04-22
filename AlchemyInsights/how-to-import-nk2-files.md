---
title: hur-till-importera-nk2-filer
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 83d30b2d62908db791f21ec5ed7fd5537e7a0944
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759350"
---
# <a name="how-to-import-nk2-files"></a>Importera 1,nk2-filer 

När du startar Microsoft Outlook 2013, Outlook 2016, Outlook 2019 eller Outlook för Microsoft 365 för första gången importeras din smeknamnscache (lagrad i profilename.nk2-filen) till ett dolt meddelande i standardmeddelandearkivet. *profilename*

Om du vill importera NK2-filer till Outlook 2013, Outlook 2016, Outlook 2019 eller Outlook för Microsoft 365 kontrollerar du att NK2-filen finns i följande mapp: %appdata%\Microsoft\Outlook

**Note**196-filen måste ha samma namn som din nuvarande Outlook 2013- eller Outlook 2016-profil. Som standard är profilnamnet "Outlook". Så här kontrollerar du profilnamnet: 
1. Klicka på **Start**och sedan på **Kontrollpanelen**.
2. Dubbelklicka på **E-post**.
3. Välj **Visa profiler**i dialogrutan Inställningar för e-post .
4. Välj **Startkörning** > **Run**.
5. Skriv *outlook.exe /importnk2*i rutan **Öppna** och välj sedan **OK**. 

När du har importerat NK2-filen sammanfogas innehållet i filen till den befintliga smeknamnscachen som lagras i postlådan.

**Note**Nk2-filen har bytt namn till filnamnstillägget nästa gång du startar Outlook 2013, Outlook 2016, Outlook 2019 eller Outlook för Microsoft 365. Om du vill importera NK2-filen igen tar du först bort filnamnstillägget .old.

Mer information finns i [Importera eller kopiera listan Komplettera](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%)automatiskt till en annan dator .