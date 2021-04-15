---
title: Σφάλμα του Teams 4c7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786669"
---
# <a name="4c7-error-in-microsoft-teams"></a>Σφάλμα 4c7 στο Microsoft Teams

Αυτό το σφάλμα παρουσιάζεται επειδή το Microsoft Teams απαιτεί έλεγχο ταυτότητας forms. Όταν αναπτύσσετε τις υπηρεσίες Active Directory Federation Services (AD FS), ο έλεγχος ταυτότητας φορμών δεν ενεργοποιείται για το intranet από προεπιλογή. Εάν αποτύχει ο ενσωματωμένος έλεγχος ταυτότητας των Windows, θα σας ζητηθεί να εισέλθετε χρησιμοποιώντας τον έλεγχο ταυτότητας φορμών.

Για να επιλύσετε αυτό το πρόβλημα, ενεργοποιήστε τον έλεγχο ταυτότητας φορμών χρησιμοποιώντας το συμπληρωματικό πρόγραμμα AD FS Microsoft Management Console (MMC) στον υπολογιστή που διαθέτει το τοπικό αντίγραφο της υπηρεσίας καταλόγου Active Directory. Για να το κάνετε, ακολουθήστε αυτά τα βήματα: 

1. Στο παράθυρο περιήγησης, μεταβείτε στην επιλογή **"Πολιτικές ελέγχου ταυτότητας".**
2. Στην **περιοχή "Ενέργειες"** στο παράθυρο λεπτομερειών, επιλέξτε "Επεξεργασία **καθολικού πρωτεύοντος ελέγχου ταυτότητας".**
3. Στην καρτέλα **Intranet, επιλέξτε** "Έλεγχος **ταυτότητας φορμών".**
4. Επιλέξτε **OK** (ή **Εφαρμογή).**