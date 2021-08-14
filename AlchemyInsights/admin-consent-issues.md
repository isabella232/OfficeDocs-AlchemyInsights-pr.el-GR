---
title: Ζητήματα συγκατάθεσης διαχειριστή
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 08d3bfa84fd5ab31d7165090c392866d863898545ade7631e820a100eef89dea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952573"
---
# <a name="admin-consent-issues"></a>Ζητήματα συγκατάθεσης διαχειριστή

1. Ενεργοποιήστε τη [ροή εργασίας συγκατάθεσης](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) διαχειριστή για να επιτρέψετε στους χρήστες να ζητούν έγκριση διαχειριστή απευθείας από την οθόνη συγκατάθεσης.

1. Εάν εσείς ή οι χρήστες της εφαρμογής σας βλέπετε μη αναμενόμενα σφάλματα κατά τη διαδικασία συγκατάθεσης, ανατρέξτε σε αυτό το άρθρο για τα βήματα αντιμετώπισης προβλημάτων: Μη αναμενόμενο σφάλμα κατά την εκτέλεση [συγκατάθεσης σε μια εφαρμογή.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)

1. Μάθετε περισσότερα σχετικά με τη συγκατάθεση διαχειριστή [](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) [για Πλατφόρμα ταυτοτήτων της Microsoft,](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)τον τρόπο με τον οποίο λειτουργεί το μήνυμα συγκατάθεσης και τον τρόπο αξιολόγησης μιας αίτησης για συγκατάθεση διαχειριστή σε επίπεδο [μισθωτή.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)

1. Οι εφαρμογές που ενοποιούνται με Πλατφόρμα ταυτοτήτων της Microsoft ακολουθούν ένα μοντέλο εξουσιοδότησης που παρέχει στους χρήστες και τους διαχειριστές τον έλεγχο του πώς μπορούν να έχουν πρόσβαση στα δεδομένα. Η υλοποίηση του μοντέλου εξουσιοδότησης έχει ενημερωθεί στο τελικό Πλατφόρμα ταυτοτήτων της Microsoft και αλλάζει τον τρόπο με τον οποίο μια εφαρμογή πρέπει να αλληλεπιδρά με το Πλατφόρμα ταυτοτήτων της Microsoft. Ανατρέξτε [στο θέμα "Δικαιώματα και συγκατάθεση" Πλατφόρμα ταυτοτήτων της Microsoft τελικό](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) σημείο για μια επισκόπηση αυτού του μοντέλου εξουσιοδότησης, συμπεριλαμβανομένων των εμβέλειων, των δικαιωμάτων και της συγκατάθεσης.