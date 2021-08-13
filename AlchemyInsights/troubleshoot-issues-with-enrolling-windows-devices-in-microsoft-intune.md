---
title: Αντιμετώπιση προβλημάτων με την εγγραφή Windows συσκευών σε Microsoft Intune
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
ms.openlocfilehash: a2abb4d0ef5504c496afefe62a80f3fa21c7ec85536e822e402be33b3617b59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981041"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Αντιμετώπιση προβλημάτων με την εγγραφή Windows συσκευών σε Microsoft Intune

Εξετάστε τους πόρους που αναφέρονται παρακάτω για να επιλύσετε το πρόβλημά σας τώρα.
  
Ορισμένα συνηθισμένα μηνύματα σφάλματος και βήματα επίλυσης:
  
 **Δεν είναι δυνατή η εγκατάσταση του λογισμικού, 0x80cf4017:** Το πιστοποιητικό του λογαριασμού σας έχει λήξει. Πραγματοποιήστε ξανά λήψη του πακέτου λογισμικού υπολογιστή-πελάτη στην Κονσόλα διαχείρισης Intune. Διαβάστε αυτή την τεκμηρίωση για περισσότερες πληροφορίες.
  
 **Κωδικός σφάλματος 0x801c0003:** Το σφάλμα μπορεί να παρουσιαστεί στα ακόλουθα σενάρια:
  
-  Ο χρήστης έχει περισσότερες συσκευές εγγεγραμμένες από το όριο της συσκευής. Εξετάστε αυτά τα έγγραφα για να [καταργήσετε μια συσκευή ή](https://docs.microsoft.com/intune/devices-wipe) [να αλλάξετε το όριο της συσκευής.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  Η ρύθμιση "Οι χρήστες μπορούν να συμμετέχουν σε συσκευές στο Azure AD" έχει οριστεί σε "καμία". Ορίστε το σε όλους ή επιλέξτε χρήστες. Διαβάστε [αυτή την τεκμηρίωση](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) για περισσότερες πληροφορίες.

-  Η συσκευή έχει ήδη εγγραφεί από άλλο χρήστη. Σε αυτή την περίπτωση, καταργήστε τη συσκευή από την κονσόλα Azure Intune ή καταργήστε τη επαναφορά της συσκευής με μη αυτόματο τρόπο προτού δοκιμάσετε ξανά.

-  Η συσκευή είναι Windows 10 Home. Μόνο Windows 10 Pro, οι SKUs για εκπαιδευτικά ιδρύματα και μεγάλες επιχειρήσεις μπορούν να Azure Active Directory.

Πρόσθετοι πόροι για την επίλυση του προβλήματος:
  
-  Χρησιμοποιήστε [την Πύλη αντιμετώπισης προβλημάτων intune για](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) να διαγνώσετε και να επιλύσετε συνηθισμένες αποτυχίες εγγραφής. Διαβάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/help-desk-operators) για περισσότερες λεπτομέρειες.

-  Εξετάστε αυτά τα έγγραφα για μια λίστα με συνήθη σφάλματα που εμποδίζουν την εγγραφή και τις λύσεις σε καθένα: [Οδηγός αντιμετώπισης προβλημάτων και](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) [έγγραφο αντιμετώπισης προβλημάτων.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

[Μάθετε πώς μπορείτε να εγγράψετε Windows συσκευές στο Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)
