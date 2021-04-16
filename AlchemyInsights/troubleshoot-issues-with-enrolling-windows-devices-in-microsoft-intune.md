---
title: Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών Windows στο Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808971"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών Windows στο Microsoft Intune

Εξετάστε τους πόρους που αναφέρονται παρακάτω για να επιλύσετε το πρόβλημά σας τώρα.
  
Ορισμένα συνηθισμένα μηνύματα σφάλματος και βήματα επίλυσης:
  
 **Δεν είναι δυνατή η εγκατάσταση του λογισμικού, 0x80cf4017:** Το πιστοποιητικό του λογαριασμού σας έχει λήξει. Πραγματοποιήστε ξανά λήψη του πακέτου λογισμικού υπολογιστή-πελάτη στην Κονσόλα διαχείρισης Intune. Διαβάστε αυτή την τεκμηρίωση για περισσότερες πληροφορίες.
  
 **Κωδικός σφάλματος 0x801c0003:** Το σφάλμα μπορεί να παρουσιαστεί στα ακόλουθα σενάρια:
  
-  Ο χρήστης έχει περισσότερες συσκευές εγγεγραμμένες από το όριο της συσκευής. Εξετάστε αυτά τα έγγραφα για να [καταργήσετε μια συσκευή ή](https://docs.microsoft.com/intune/devices-wipe) [να αλλάξετε το όριο της συσκευής.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  Η ρύθμιση "Οι χρήστες μπορούν να συμμετέχουν σε συσκευές στο Azure AD" έχει οριστεί σε "καμία". Ορίστε το σε όλους ή επιλέξτε χρήστες. Διαβάστε [αυτή την τεκμηρίωση](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) για περισσότερες πληροφορίες.

-  Η συσκευή έχει ήδη εγγραφεί από άλλο χρήστη. Σε αυτή την περίπτωση, καταργήστε τη συσκευή από την κονσόλα Azure Intune ή καταργήστε τη επαναφορά της συσκευής με μη αυτόματο τρόπο προτού δοκιμάσετε ξανά.

-  Η συσκευή είναι Windows 10 Home. Μόνο οι SKUs windows 10 Pro, Education και Enterprise μπορούν να συμμετάσχουν στο Azure Active Directory.

Πρόσθετοι πόροι για την επίλυση του προβλήματος:
  
-  Χρησιμοποιήστε [την Πύλη αντιμετώπισης προβλημάτων intune για](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) να διαγνώσετε και να επιλύσετε συνηθισμένες αποτυχίες εγγραφής. Διαβάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/help-desk-operators) για περισσότερες λεπτομέρειες.

-  Εξετάστε αυτά τα έγγραφα για μια λίστα με συνήθη σφάλματα που εμποδίζουν την εγγραφή και τις λύσεις σε καθένα: [Οδηγός αντιμετώπισης προβλημάτων και](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) [έγγραφο αντιμετώπισης προβλημάτων.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

[Μάθετε πώς μπορείτε να εγγράψετε συσκευές Windows στο Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)
