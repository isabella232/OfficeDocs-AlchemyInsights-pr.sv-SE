---
title: Start Inställningar i Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751153"
---
# <a name="startup-settings-in-windows-10"></a>Start Inställningar i Windows 10

**Ändra vilka appar som körs automatiskt vid start**

1. Gå till [inställningar > appar > start](ms-settings:startupapps?activationSource=GetHelp).

2. Se till att alla program du vill köra vid **Start är aktiverat.**

**Lägga till ett program som ska köras automatiskt vid start**

1. Klicka eller tryck på **Start** och leta reda på det program du vill köra vid start.

2. Högerklicka på appen, klicka på **mer**och sedan på **Öppna fil Sök väg**. Då öppnas platsen där genvägen till programmet har sparats. Om det inte finns något alternativ för att öppna fil Sök vägen innebär det att appen inte kan köras vid start.

3. Öppna fil platsen och tryck på Windows- **tangenten + R**, Skriv **Shell: Start**och klicka sedan på **OK**. Då öppnas startmappen.

4. Kopiera och klistra in genvägen till appen från fil platsen till mappen Start.

**Avancerade start alternativ (inklusive fel säkert läge, UEFI-inställningar och start från en annan enhet)**

1. Spara ditt arbete och Stäng alla öppna dokument eftersom de här anvisningarna startar om datorn.

2. Gå till [inställningar > uppdatering & säkerhets > återställning](ms-settings:recovery?activationSource=GetHelp).

3. Klicka på **starta om nu**under **Avancerad start**. 

4. När du har startat om datorn på skärmen Välj ett alternativ:

    - Om du vill starta från en enhet som en USB-enhet klickar du på **Använd en enhet**.

    - Om du vill ange UEFI-inställningar (kallas ibland BIOS-konfiguration) klickar du på **felsöka > avancerade alternativ > UEFI-inställningar**. 

    - Om du vill öppna fel säkert läge eller ändra avancerade Start Inställningar klickar du på **felsöka > avancerade alternativ > Start Inställningar**och klickar sedan på **starta om**. Du kan uppmanas att ange din [återställnings nyckel för BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). När datorn har startat om klickar du på den Start inställning du vill använda.