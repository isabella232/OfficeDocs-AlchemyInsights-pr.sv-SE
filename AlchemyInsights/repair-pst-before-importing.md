---
title: Reparera. PST-fil före import
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
- "1226"
- "1800027"
ms.assetid: ''
ms.openlocfilehash: 1ed37192a6b054b745fd48fbc01a6b00fa7074ed
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799114"
---
# <a name="repair-pst-file-before-importing"></a>Reparera. PST-fil före import

Innan du importerar en PST-fil i Outlook bör du kontrol lera att filen inte är skadad genom att reparera filen:

1. Avsluta Outlook.

2. Hitta och kör `Scanpst.exe` i mappen Office-program (C:\Program Files (x86) \Microsoft Office\root\Office \<Version\> eller c:\Program\Microsoft Office\root\Office \<Version\> ).

3. I **reparations verktyget för Inkorgen för Microsoft Outlook**klickar du på **Bläddra** och letar reda på PST-filen (till exempel i C:\Users \\<username \> \AppData\Local\Microsoft\Outlook). Välj PST-filen och klicka på **Öppna**.

4. Klicka på **Start** för att starta genomsökningen.

5. Om fel hittas i filen klickar du på **Reparera**och sedan på **OK** när reparationen är klar.

6. Försök importera PST-filen i Outlook igen.

Mer information finns i [Reparera Outlook-datafiler](https://support.office.com/article/25663bc3-11ec-4412-86c4-60458afc5253) och [åtgärda problem med att importera en Outlook. PST-fil](https://support.office.com/article/2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).
