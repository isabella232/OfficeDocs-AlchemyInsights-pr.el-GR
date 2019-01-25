---
title: Κωδικός σφάλματος 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Αν λαμβάνετε ένα σφάλμα κατά την ενεργοποίηση του Office 2013 σε υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS) αναπτύξεις, εξετάστε το ενδεχόμενο να Ενεργοποίηση ADAL με επεξεργασία του μητρώου.
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499382"
---
Αν λαμβάνετε ένα σφάλμα κατά την ενεργοποίηση του Office 2013 σε υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS) αναπτύξεις, εξετάστε το ενδεχόμενο να Ενεργοποίηση ADAL με επεξεργασία του μητρώου. 
  
|**Κλειδί μητρώου**| πληκτρολογήστε |Τιμή|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |
   
Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Ενεργοποίηση σύγχρονη ελέγχου ταυτότητας για το Office 2013 σε συσκευές των Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL είναι ενεργοποιημένη από προεπιλογή στο Office 365 ProPlus και Office 2016. > Υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS) ήταν προηγουμένως με το όνομα των υπηρεσιών Terminal Services. 
  

