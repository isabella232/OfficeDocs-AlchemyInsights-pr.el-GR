---
title: Κωδικός σφάλματος 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Εάν λαμβάνετε ένα σφάλμα κατά την ενεργοποίηση του Office 2013 σε αναπτύξεις υπηρεσιών απομακρυσμένης επιφάνειας εργασίας (RDS), εξετάστε το ενδεχόμενο να ενεργοποιήσετε το ADAL με την επεξεργασία του μητρώου.
ms.openlocfilehash: ed3770c001461c162ff5bbe24dc400a29380a03b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316686"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Σφάλμα κατά την ενεργοποίηση Office 2013 στις υπηρεσίες απομακρυσμένης επιφάνειας εργασίας

Εάν λαμβάνετε ένα σφάλμα κατά την ενεργοποίηση του Office 2013 σε αναπτύξεις υπηρεσιών απομακρυσμένης επιφάνειας εργασίας (RDS), εξετάστε το ενδεχόμενο να ενεργοποιήσετε το ADAL με την επεξεργασία του μητρώου.
  
|**Κλειδί μητρώου**|**Τύπος**|**Τιμή**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα Ενεργοποίηση σύγχρονου ελέγχου ταυτότητας Office 2013 σε Windows συσκευές.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)
  
**Σημείωση:** Το ADAL είναι ενεργοποιημένο από προεπιλογή στις Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις και Office 2016. Οι υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS) ονομάζονταν προηγουμένως υπηρεσίες Terminal Services.
  