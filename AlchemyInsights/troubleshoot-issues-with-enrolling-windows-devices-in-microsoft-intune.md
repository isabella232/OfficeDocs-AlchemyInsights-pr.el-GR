---
title: Αντιμετώπιση προβλημάτων σχετικά με την εγγραφή συσκευών των Windows στα Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: be66135b80f32f78266ef2b6a7b3f5b30e24d5fc
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559661"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Αντιμετώπιση προβλημάτων σχετικά με την εγγραφή συσκευών των Windows στα Microsoft Intune

Εξετάστε τους πόρους που αναφέρονται παρακάτω για να επιλύσετε το θέμα σας τώρα.
  
Ορισμένα κοινά μηνύματα λάθους και τα βήματα επίλυσης:
  
 **Το λογισμικό δεν είναι εγκατεστημένο, 0x80cf4017:** Έχει λήξει το πιστοποιητικό του λογαριασμού σας. Εκ νέου λήψη του πακέτου λογισμικού PC υπολογιστή-πελάτη στην κονσόλα διαχείρισης του Intune. Εξετάστε αυτήν την τεκμηρίωση για περισσότερες πληροφορίες.
  
 **Κωδικός σφάλματος 0x801c0003:** Το σφάλμα μπορεί να προκύψει στα ακόλουθα σενάρια:
  
1. Ο χρήστης έχει περισσότερες συσκευές που συμμετέχουν από το όριο συσκευής. Εξετάστε αυτά τα έγγραφα για να [καταργήσετε μια συσκευή](https://docs.microsoft.com/intune/devices-wipe) ή να [αλλάξετε το όριο της συσκευής](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

2. "Οι χρήστες μπορούν να συμμετέχουν συσκευές σε Azure AD" έχει οριστεί σε "Κανένα". Ορίστε την σε όλους ή επιλέξτε χρήστες. Εξετάστε [αυτήν την τεκμηρίωση](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) για περισσότερες πληροφορίες.

3. Η συσκευή είναι ήδη συμμετέχουν από κάποιον άλλο χρήστη. Εάν συμβαίνει αυτό, καταργήστε τη συσκευή από την κονσόλα Azure Intune ή unenroll με μη αυτόματο τρόπο τη συσκευή πριν να προσπαθήσετε πάλι.

4. Η συσκευή είναι 10 Windows Home. Μόνο Windows 10 Pro, εκπαίδευση και Enterprise SKU να συμμετάσχετε Azure υπηρεσίας καταλόγου Active Directory.

Πρόσθετους πόρους για να σας βοηθήσουν να επιλύσετε το ζήτημα:
  
1. Χρησιμοποιήστε [Πύλη του Intune αντιμετώπιση προβλημάτων](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) για να διαγνώσετε και να επιλύσετε συνηθισμένα σφάλματα εγγραφής. Αναθεωρήστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/help-desk-operators) για περισσότερες λεπτομέρειες.

2. Εξετάστε αυτά τα έγγραφα για μια λίστα με συνηθισμένα σφάλματα που εμποδίζουν την εγγραφή και λύσεις σε κάθε: [Οδηγός αντιμετώπισης προβλημάτων](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) και [Αντιμετώπιση προβλημάτων doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Μάθετε πώς μπορείτε να εγγραφείτε συσκευές Windows Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
