---
title: Teams σφάλματος 4c7
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
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049308"
---
# <a name="4c7-error-in-microsoft-teams"></a>Σφάλμα 4c7 στο Microsoft Teams

Αυτό το σφάλμα παρουσιάζεται επειδή Microsoft Teams απαιτείται έλεγχος ταυτότητας φορμών. Όταν αναπτύσσετε τις υπηρεσίες Active Directory Federation Services (AD FS), ο έλεγχος ταυτότητας φορμών δεν ενεργοποιείται για το intranet από προεπιλογή. Εάν Windows ενοποιημένος έλεγχος ταυτότητας, θα σας ζητηθεί να εισέλθετε χρησιμοποιώντας τον έλεγχο ταυτότητας φορμών.

Για να επιλύσετε αυτό το πρόβλημα, ενεργοποιήστε τον έλεγχο ταυτότητας φορμών χρησιμοποιώντας το συμπληρωματικό πρόγραμμα AD FS Microsoft Management Console (MMC) στον υπολογιστή που διαθέτει το τοπικό αντίγραφο της υπηρεσίας καταλόγου Active Directory. Για να το κάνετε, ακολουθήστε αυτά τα βήματα: 

1. Στο παράθυρο περιήγησης, μεταβείτε στην επιλογή **"Πολιτικές ελέγχου ταυτότητας".**
2. Στην **περιοχή "Ενέργειες"** στο παράθυρο λεπτομερειών, επιλέξτε "Επεξεργασία **καθολικού πρωτεύοντος ελέγχου ταυτότητας".**
3. Στην καρτέλα **Intranet, επιλέξτε** "Έλεγχος **ταυτότητας φορμών".**
4. Επιλέξτε **OK** (ή **Εφαρμογή).**