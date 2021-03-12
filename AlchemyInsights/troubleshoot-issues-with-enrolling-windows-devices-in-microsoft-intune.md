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
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708890"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών Windows στο Microsoft Intune

Εξετάστε τους πόρους που παρατίθενται παρακάτω για να επιλύσετε το πρόβλημά σας τώρα.
  
Ορισμένα συνήθη μηνύματα σφάλματος και βήματα επίλυσης:
  
 **Δεν είναι δυνατή η εγκατάσταση του λογισμικού, 0x80cf4017:** Το πιστοποιητικό του λογαριασμού σας έχει λήξει. Κάντε εκ ξανά λήψη του πακέτου λογισμικού προγράμματος-πελάτη υπολογιστή στην κονσόλα διαχείρισης Intune. Ανατρέξτε σε αυτή την τεκμηρίωση για περισσότερες πληροφορίες.
  
 **Κωδικός σφάλματος 0x801c0003:** Το σφάλμα μπορεί να προκύψει στα ακόλουθα σενάρια:
  
-  Ο χρήστης έχει εγγράψει περισσότερες συσκευές σε σχέση με το όριο συσκευών. Εξετάστε αυτά τα έγγραφα για να [καταργήσετε μια συσκευή ή](https://docs.microsoft.com/intune/devices-wipe) [να αλλάξετε το όριο συσκευών.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  Η ρύθμιση "Οι χρήστες μπορούν να συμμετάσχουν σε συσκευές στο Azure AD" ορίζεται σε "καμία". Ρυθμίστε το σε όλους ή επιλέξτε χρήστες. Ανατρέξτε [σε αυτή την](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) τεκμηρίωση για περισσότερες πληροφορίες.

-  Η συσκευή έχει ήδη εγγραφεί από άλλο χρήστη. Σε αυτή την περίπτωση, καταργήστε τη συσκευή από την κονσόλα Azure Intune ή καταργήστε τη μισθοδοσία της συσκευής με μη αυτόματο τρόπο πριν να δοκιμάσετε ξανά.

-  Η συσκευή είναι Windows 10 Home. Μόνο οι SKUs των Windows 10 Pro, Education και Enterprise μπορούν να συμμετάσχουν στο Azure Active Directory.

Πρόσθετοι πόροι που θα σας βοηθήσουν να επιλύσετε το πρόβλημα:
  
-  Χρησιμοποιήστε [την Πύλη αντιμετώπισης προβλημάτων του Intune για](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) τη διάγνωση και την επίλυση συνηθισμένων αποτυχιών εγγραφής. Ελέγξτε [αυτό το έγγραφο](https://docs.microsoft.com/intune/help-desk-operators) για περισσότερες λεπτομέρειες.

-  Εξετάστε αυτά τα έγγραφα για μια λίστα με συνηθισμένα σφάλματα που εμποδίζουν την εγγραφή και την επίλυση του [καθένα:](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) Οδηγός αντιμετώπισης προβλημάτων και [έγγραφο αντιμετώπισης προβλημάτων.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

[Μάθετε πώς μπορείτε να εγγράψετε συσκευές Windows στο Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)
