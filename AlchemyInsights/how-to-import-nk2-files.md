---
title: how-to-import-nk2-files
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: f2b034926ec165b819119b5c4e060f10022d6017ec5dba8794d18ee3e96c709a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54043224"
---
# <a name="how-to-import-nk2-files"></a>Importera .nk2-filer 

När du startar Microsoft Outlook 2013, Outlook 2016, Outlook 2019 eller Outlook för Microsoft 365 för första gången importeras ditt smeknamnscache (som finns i *profilename*.nk2-filen) till ett dolt meddelande i standardmeddelandelagringsplatsen.

Om du vill importera .nk2-filer till Outlook 2013, Outlook 2016, Outlook 2019 eller Outlook för Microsoft 365 kontrollerar du att .nk2-filen finns i följande mapp: %appdata%\Microsoft\Outlook

**Obs!** Filen .nk2 måste ha samma namn som din aktuella Outlook 2013- Outlook 2016 profil. Som standard är profilnamnet "Outlook". Om du vill kontrollera profilnamnet gör du så här: 
1. Klicka på **Start** och klicka sedan på **Kontrollpanelen**.
2. Dubbelklicka på **E-post.**
3. I dialogrutan Konfigurera e-post väljer du **Visa profiler.**
4. Klicka på **Start** > **Kör**.
5. I rutan **Öppna** skriver du *outlook.exe /importnk2* och väljer sedan **OK.** 

När du har importerat .nk2-filen slås innehållet i filen ihop med den befintliga smeknamnscache som finns i postlådan.

**Obs!**.nk2-filen får ett nytt namn med filnamnstillägget .old nästa gång du startar Outlook 2013, Outlook 2016, Outlook 2019 eller Outlook för Microsoft 365. Om du vill importera om .nk2-filen tar du först bort filnamnstillägget .old.

Mer information finns i Importera [eller kopiera listan Komplettera automatiskt till en annan dator.](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%)