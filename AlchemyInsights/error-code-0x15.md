---
title: Κωδικός σφάλματος 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Εάν λαμβάνετε ένα σφάλμα κατά την ενεργοποίηση του Office 2013 σε αναπτύξεις υπηρεσιών απομακρυσμένης επιφάνειας εργασίας (RDS), εξετάστε το ενδεχόμενο να ενεργοποιήσετε το ADAL με επεξεργασία του μητρώου.
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506846"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Σφάλμα κατά την ενεργοποίηση του Office 2013 στις υπηρεσίες απομακρυσμένης επιφάνειας εργασίας

Εάν λαμβάνετε ένα σφάλμα κατά την ενεργοποίηση του Office 2013 σε αναπτύξεις υπηρεσιών απομακρυσμένης επιφάνειας εργασίας (RDS), εξετάστε το ενδεχόμενο να ενεργοποιήσετε το ADAL με επεξεργασία του μητρώου.
  
|**Κλειδί μητρώου**|**Πληκτρολογήστε**|**Τιμή**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Λογισμικό\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |Reg_dword  <br/> |1  <br/> |

Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Ενεργοποίηση σύγχρονου ελέγχου ταυτότητας για το Office 2013 σε συσκευές Των Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  Το ADAL είναι ενεργοποιημένο από προεπιλογή στις Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις και στο Office 2016. Οι υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS) είχαν ονομαστεί προηγουμένως υπηρεσίες τερματικού.
  