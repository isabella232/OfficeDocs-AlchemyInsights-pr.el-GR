---
title: Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών Windows στο Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658878"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών Windows στο Microsoft Intune

Εξετάστε τους πόρους που παρατίθενται παρακάτω για να επιλύσετε το ζήτημά σας τώρα.
  
Ορισμένα συνηθισμένα μηνύματα σφάλματος και βήματα επίλυσης:
  
 **Δεν είναι δυνατή η εγκατάσταση του λογισμικού, 0x80cf4017:** Το πιστοποιητικό του λογαριασμού σας έχει λήξει. Επαναλάβετε τη λήψη του πακέτου λογισμικού υπολογιστή-πελάτη υπολογιστή στην κονσόλα διαχείρισης του Intune. Εξετάστε αυτή την τεκμηρίωση για περισσότερες πληροφορίες.
  
 **Κωδικός σφάλματος 0x801c0003:** Το σφάλμα μπορεί να προκύψει στα ακόλουθα σενάρια:
  
-  Ο χρήστης έχει περισσότερες συσκευές που έχουν εγγραφεί από το όριο της συσκευής. Εξετάστε αυτά τα έγγραφα για να [καταργήσετε μια συσκευή](https://docs.microsoft.com/intune/devices-wipe) ή να [αλλάξετε το όριο της συσκευής](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Οι χρήστες μπορούν να συμμετέχουν σε συσκευές στο Azure AD" έχει την τιμή "καμία". Ορίστε την σε όλους ή επιλέξτε χρήστες. Εξετάστε [αυτή την τεκμηρίωση](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) για περισσότερες πληροφορίες.

-  Η συσκευή έχει ήδη εγγραφεί από άλλο χρήστη. Εάν αυτή είναι η περίπτωση, καταργήστε τη συσκευή από την κονσόλα Azure Intune ή καταργήστε την εγγραφή της συσκευής με μη αυτόματο τρόπο, πριν να προσπαθήσετε ξανά.

-  Η συσκευή είναι η αρχική σελίδα των Windows 10. Μόνο τα Windows 10 Pro, εκπαιδευτικά και εταιρικά SKU μπορούν να συμμετέχουν στο Azure Active Directory.

Πρόσθετοι πόροι που θα σας βοηθήσουν να επιλύσετε το πρόβλημα:
  
-  Χρησιμοποιήστε την [πύλη αντιμετώπισης προβλημάτων του Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) για να διαγνώσετε και να επιλύσετε συνηθισμένες αποτυχίες εγγραφής. Εξετάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/help-desk-operators) για περισσότερες λεπτομέρειες.

-  Εξετάστε αυτά τα έγγραφα για μια λίστα με συνηθισμένα σφάλματα που εμποδίζουν την εγγραφή και τις αναλύσεις σε κάθε: [Οδηγός αντιμετώπισης προβλημάτων](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) και [Αντιμετώπιση προβλημάτων doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Μάθετε πώς μπορείτε να εγγράψετε συσκευές Windows στο Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
