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
description: Εάν λαμβάνετε ένα μήνυμα σφάλματος κατά την ενεργοποίηση του Office 2013 σε αναπτύξεις υπηρεσιών απομακρυσμένης επιφάνειας εργασίας (RDS), εξετάστε το ενδεχόμενο να ενεργοποιήσετε το ADAL με την επεξεργασία του μητρώου.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709187"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Σφάλμα κατά την ενεργοποίηση του Office 2013 σε υπηρεσίες απομακρυσμένης επιφάνειας εργασίας

Εάν λαμβάνετε ένα μήνυμα σφάλματος κατά την ενεργοποίηση του Office 2013 σε αναπτύξεις υπηρεσιών απομακρυσμένης επιφάνειας εργασίας (RDS), εξετάστε το ενδεχόμενο να ενεργοποιήσετε το ADAL με την επεξεργασία του μητρώου.
  
|**Κλειδί μητρώου**|**Τύπος**|**Τιμή**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Ενεργοποίηση σύγχρονου ελέγχου ταυτότητας για το Office 2013 σε συσκευές Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  Το ADAL είναι ενεργοποιημένο από προεπιλογή στο Microsoft 365 apps για επιχειρήσεις και το Office 2016. Οι υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS) ονομάστηκαν προηγουμένως Terminal Services.
  