---
title: Παραχωρήσετε στους χρήστες πρόσβαση στο SharePoint και OneDrive
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9326932e93970edc96396a141c9b36b14e7b4d4d
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736648"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a>Παραχωρήσετε στους χρήστες πρόσβαση στο SharePoint και OneDrive

Αυτό το ζήτημα προκύπτει πιο συχνά όταν ο χρήστης έχει διαγραφεί και να δημιουργηθεί εκ νέου με το ίδιο κύριο όνομα χρήστη (UPN). Ο νέος λογαριασμός δημιουργείται χρησιμοποιώντας μια διαφορετική τιμή PUID (μοναδικό Αναγνωριστικό Passport). Όταν ο χρήστης προσπαθήσει να αποκτήσει πρόσβαση σε μια συλλογή τοποθεσιών ή τους OneDrive, ο χρήστης έχει μια εσφαλμένη PUID. Ένα δεύτερο σενάριο περιλαμβάνει συγχρονισμού καταλόγου με μια υπηρεσία καταλόγου Active Directory οργανική μονάδα (OU). Εάν οι χρήστες έχουν ήδη εισέλθει στο SharePoint, και στη συνέχεια θα μετακινηθεί σε μια διαφορετική OU και resynced με το SharePoint, αυτά ενδέχεται να αντιμετωπίσετε αυτό το ζήτημα.

Για να επιλύσετε αυτό το ζήτημα θα πρέπει να επαναφέρετε το αρχικό UPN ακολουθώντας τα βήματα στο άρθρο,[επαναφέρετε ένα χρήστη στο Office 365](https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide).

Αφού το κάνετε αυτό, μπορείτε να επαληθεύσετε ο χρήστης διαθέτει δικαιώματα διαχείρισης στην τοποθεσία του OneDrive, ακολουθώντας τα βήματα για την [Προσθήκη admin του για OneDrive του χρήστη](https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Για περισσότερες πληροφορίες σχετικά με τα επίπεδα δικαιωμάτων, ανατρέξτε στο άρθρο, [Κατανόηση των επιπέδων δικαιωμάτων στο SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).
