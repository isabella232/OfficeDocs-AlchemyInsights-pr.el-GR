---
title: Περιορισμός πρόσβασης σε SharePoint ή OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: fc6731d5a7747bb4fc8d6cef1b6ac0045d11917d7f97abbb21eea9613b1b1aa2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093829"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Περιορισμός πρόσβασης σε SharePoint ή OneDrive

Υπάρχουν πολλοί τρόποι για να περιορίσετε την πρόσβαση σε SharePoint online/OneDrive υπηρεσιών. Αυτές οι διάφορες μέθοδοι περιορισμού πρόσβασης περιγράφονται παρακάτω. 

**Περιορισμός δικαιωμάτων**

Στο SharePoint Online και OneDrive για επιχειρήσεις, περιορίζουμε την πρόσβαση σε στοιχεία όπως τοποθεσίες, αρχεία και φακέλους, παραχωρώντας πρόσβαση μόνο σε αυτές τις ομάδες/άτομα που θα πρέπει να έχουν πρόσβαση.

- [Προσαρμογή δικαιωμάτων για μια SharePoint ή βιβλιοθήκη](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Προσαρμογή SharePoint τοποθεσίας](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Αλλαγή των δικαιωμάτων σε έναν υποφάκελο](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Έλεγχος πρόσβασης από μη διαχειριζόμενες συσκευές](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Ως διαχειριστής SharePoint ή καθολικός διαχειριστής, μπορείτε να αποκλείσετε ή να περιορίσετε την πρόσβαση σε περιεχόμενο SharePoint και OneDrive από μη διαχειριζόμενες συσκευές (αυτές που δεν είναι υβριδικές ad συνδεδεμένες ή συμβατές με το Intune).

**Περιορισμός θέσης δικτύου**

Ως διαχειριστής IT, μπορείτε να ελέγχετε την πρόσβαση σε SharePoint και OneDrive με βάση καθορισμένες θέσεις δικτύου που εμπιστεύεστε. Αυτό είναι επίσης γνωστό ως πολιτική βάσει τοποθεσίας. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Έλεγχος πρόσβασης σε SharePoint Online και OneDrive δεδομένων με βάση τη θέση δικτύου](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Περιορισμός κλειδώματος τοποθεσίας** 

Μέσα SharePoint Online έχετε τη δυνατότητα να κλειδώσετε μια συλλογή τοποθεσιών, ώστε να μην έχει κανείς πρόσβαση. Αυτό ορίζεται μέσω του PowerShell και [του κελύφους SharePoint online διαχείρισης](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) χρησιμοποιώντας την ιδιότητα [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Περιορισμός χρηστών από τη δημιουργία τοποθεσιών ή δευτερευών τοποθεσιών**

Ως διαχειριστής SharePoint ή καθολικός διαχειριστής, μπορείτε να επιτρέψετε στους χρήστες σας να δημιουργούν και να διαχειρίζονται τις δικές τους τοποθεσίες του SharePoint, να καθορίζουν το είδος των τοποθεσιών που μπορούν να δημιουργούν και να καθορίζουν τη θέση των τοποθεσιών. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Διαχείριση δημιουργίας τοποθεσίας στο SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

