---
title: Σφάλμα 4c7 ομάδων
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
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700203"
---
# <a name="4c7-error-in-microsoft-teams"></a>σφάλμα 4c7 στο Microsoft teams

Αυτό το σφάλμα παρουσιάζεται επειδή το Microsoft teams απαιτεί έλεγχο ταυτότητας φορμών. Κατά την ανάπτυξη των υπηρεσιών Ομοσπονδία υπηρεσίας καταλόγου Active Directory (AD FS), ο έλεγχος ταυτότητας φορμών δεν είναι ενεργοποιημένος για το intranet από προεπιλογή. Εάν αποτύχει ο ενσωματωμένος έλεγχος ταυτότητας των Windows, θα σας ζητηθεί να πραγματοποιήσετε είσοδο χρησιμοποιώντας τον έλεγχο ταυτότητας φορμών.

Για να επιλύσετε αυτό το ζήτημα, ενεργοποιήστε τον έλεγχο ταυτότητας φορμών χρησιμοποιώντας το συμπληρωματικό πρόγραμμα της κονσόλας διαχείρισης της Microsoft (MMC) AD FS στον υπολογιστή που έχει το τοπικό αντίγραφο της υπηρεσίας καταλόγου Active Directory. Για να το κάνετε, ακολουθήστε αυτά τα βήματα: 

1. Στο παράθυρο περιήγησης, μεταβείτε στις **πολιτικές ελέγχου ταυτότητας**.
2. Στην περιοχή **ενέργειες** στο παράθυρο λεπτομερειών, επιλέξτε **Επεξεργασία καθολικού πρωτεύοντος ελέγχου ταυτότητας**.
3. Στην καρτέλα **intranet** , επιλέξτε **Έλεγχος ταυτότητας φορμών**.
4. Επιλέξτε **OK** (ή **Apply**).