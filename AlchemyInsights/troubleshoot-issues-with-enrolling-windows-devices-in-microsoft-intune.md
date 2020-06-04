---
title: Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών Των Windows στο Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665832"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών Των Windows στο Microsoft Intune

Εξετάστε τους πόρους που παρατίθενται παρακάτω για να επιλύσετε το ζήτημά σας τώρα.
  
Ορισμένα συνηθισμένα μηνύματα σφάλματος και βήματα επίλυσης:
  
 **Δεν είναι δυνατή η εγκατάσταση του λογισμικού, 0x80cf4017:** Το πιστοποιητικό του λογαριασμού σας έχει λήξει. Κάντε ξανά λήψη του πακέτου λογισμικού υπολογιστή-πελάτη στην κονσόλα διαχείρισης Intune. Εξετάστε αυτήν την τεκμηρίωση για περισσότερες πληροφορίες.
  
 **Κωδικός σφάλματος 0x801c0003:** Το σφάλμα μπορεί να παρουσιαστεί στα ακόλουθα σενάρια:
  
-  Ο χρήστης έχει περισσότερες συσκευές εγγεγραμμένες από το όριο της συσκευής. Εξετάστε αυτά τα έγγραφα για να [καταργήσετε μια συσκευή](https://docs.microsoft.com/intune/devices-wipe) ή [να αλλάξετε το όριο της συσκευής](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Οι χρήστες μπορούν να ενώσουν συσκευές σε Azure AD" έχει οριστεί σε "καμία". Ορίστε το σε όλους ή επιλέξτε χρήστες. Εξετάστε [αυτήν την τεκμηρίωση](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) για περισσότερες πληροφορίες.

-  Η συσκευή έχει ήδη εγγραφεί από άλλο χρήστη. Σε αυτήν την περίπτωση, καταργήστε τη συσκευή από την κονσόλα Azure Intune ή καταργήστε την εγγραφή της συσκευής με μη αυτόματο τρόπο πριν προσπαθήσετε ξανά.

-  Η συσκευή είναι Windows 10 Home. Μόνο τα Windows 10 Pro, εκπαιδευτικά και εταιρικά SKU μπορούν να συμμετάσχουν στην υπηρεσία καταλόγου Azure Active Directory.

Πρόσθετοι πόροι που θα σας βοηθήσουν να επιλύσετε το ζήτημά σας:
  
-  Χρησιμοποιήστε την [πύλη αντιμετώπισης προβλημάτων intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) για να διαγνώσετε και να επιλύσετε συνήθεις αποτυχίες εγγραφής. Εξετάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/help-desk-operators) για περισσότερες λεπτομέρειες.

-  Εξετάστε αυτά τα έγγραφα για μια λίστα συνηθισμένων σφαλμάτων που εμποδίζουν την εγγραφή και τις λύσεις σε κάθε ένα: [Οδηγός αντιμετώπισης προβλημάτων](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) και [Αντιμετώπιση προβλημάτων εγγράφου](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Μάθετε πώς μπορείτε να εγγράψετε συσκευές Windows στο Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
