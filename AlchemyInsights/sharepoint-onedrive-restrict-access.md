---
title: Περιορισμός πρόσβασης στο SharePoint ή στο OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700455"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Περιορισμός πρόσβασης στο SharePoint ή στο OneDrive

Υπάρχουν πολλοί τρόποι για να περιορίσετε την πρόσβαση στις υπηρεσίες του SharePoint Online/OneDrive. Αυτές οι διάφορες μέθοδοι περιορισμού πρόσβασης περιγράφονται παρακάτω. 

**Περιορισμός δικαιωμάτων**

Στο SharePoint Online και το OneDrive για την επιχείρηση, περιορίζουμε την πρόσβαση σε στοιχεία όπως τοποθεσίες, αρχεία και φακέλους, παρέχοντας μόνο πρόσβαση σε αυτές τις ομάδες/άτομα που πρέπει να έχουν πρόσβαση.

- [Προσαρμογή δικαιωμάτων για μια λίστα ή βιβλιοθήκη του SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Προσαρμογή δικαιωμάτων τοποθεσίας του SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Αλλαγή των δικαιωμάτων σε έναν υποφάκελο](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Έλεγχος της πρόσβασης από μη διαχειριζόμενες συσκευές](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Ως SharePoint ή καθολικός διαχειριστής, μπορείτε να αποκλείσετε ή να περιορίσετε την πρόσβαση σε περιεχόμενο του SharePoint και του OneDrive από μη διαχειριζόμενες συσκευές (αυτές που δεν είναι υβριδικές ΔΙΑΦΗΜΊΣΕΙς συνδεδεμένες ή συμβατές με το Intune).

**Περιορισμός θέσης δικτύου**

Ως διαχειριστής IT, μπορείτε να ελέγχετε την πρόσβαση σε πόρους του SharePoint και του OneDrive με βάση καθορισμένες θέσεις δικτύου που εμπιστεύεστε. Αυτό είναι επίσης γνωστό ως πολιτική βάσει τοποθεσίας. Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα Έλεγχος της πρόσβασης στα δεδομένα του SharePoint Online και του OneDrive με βάση τη θέση δικτύου](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Περιορισμός κλειδώματος τοποθεσίας** 

Στο SharePoint Online έχετε τη δυνατότητα να κλειδώσετε μια συλλογή τοποθεσιών, ώστε να μην έχει πρόσβαση κανείς. Αυτό έχει καθοριστεί μέσω του PowerShell και του [κελύφους διαχείρισης του SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) χρησιμοποιώντας την ιδιότητα [SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Περιορισμός χρηστών από τη δημιουργία τοποθεσιών ή δευτερευουσών τοποθεσιών**

Ως διαχειριστής του SharePoint ή ως καθολικός διαχειριστής, μπορείτε να επιτρέψετε στους χρήστες να δημιουργούν και να διαχειρίζονται τις δικές τους τοποθεσίες του SharePoint, να προσδιορίζουν το είδος των τοποθεσιών που μπορούν να δημιουργήσουν και να καθορίζουν τη θέση των τοποθεσιών. Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Διαχείριση δημιουργίας τοποθεσίας στο SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

