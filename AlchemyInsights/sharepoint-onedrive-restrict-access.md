---
title: Περιορισμός πρόσβασης στο SharePoint ή στο OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750664"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Περιορισμός πρόσβασης στο SharePoint ή στο OneDrive

Υπάρχουν πολλοί τρόποι για να περιορίσετε την πρόσβαση στις υπηρεσίες του SharePoint Online/OneDrive. Αυτές οι διάφορες μέθοδοι περιορισμού πρόσβασης περιγράφονται παρακάτω. 

**Περιορισμός δικαιωμάτων**

Στο SharePoint Online και OneDrive για την επιχείρηση, περιορίζουμε την πρόσβαση σε στοιχεία, όπως τοποθεσίες, αρχεία και φακέλους, παρέχοντας πρόσβαση μόνο σε αυτές τις ομάδες/άτομα που θα πρέπει να έχουν πρόσβαση.

- [Προσαρμογή δικαιωμάτων για μια λίστα ή βιβλιοθήκη του SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Προσαρμογή δικαιωμάτων τοποθεσίας SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Αλλαγή των δικαιωμάτων σε έναν υποφάκελο](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Έλεγχος πρόσβασης από μη διαχειριζόμενες συσκευές](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Ως ένα SharePoint ή καθολικό διαχειριστή στο Office 365, μπορείτε να αποκλείσετε ή να περιορίσετε την πρόσβαση σε περιεχόμενο του SharePoint και OneDrive από μη διαχειριζόμενες συσκευές (αυτές δεν είναι υβριδική AD συμμετέχει ή συμμορφώνεται με Intune).

**Περιορισμός θέσης δικτύου**

Ως διαχειριστής ΠΛΗΡΟΦΟΡΙΚΉς, μπορείτε να ελέγχετε την πρόσβαση σε πόρους του SharePoint και του OneDrive με βάση καθορισμένες θέσεις δικτύου που εμπιστεύεστε. Αυτό είναι επίσης γνωστό ως πολιτική βάσει τοποθεσίας. Για περισσότερες πληροφορίες, ανατρέξτε στο [στοιχείο Έλεγχος πρόσβασης στα δεδομένα του SharePoint Online και OneDrive με βάση τη θέση δικτύου](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Περιορισμός κλειδώματος τοποθεσίας** 

Στο SharePoint Online έχετε τη δυνατότητα να κλειδώσετε μια συλλογή τοποθεσιών, ώστε να μην έχει πρόσβαση κανείς. Αυτό ορίζεται μέσω PowerShell και το [κέλυφος διαχείρισης του SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) χρησιμοποιώντας την ιδιότητα [set-τοποθεσία](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -κλείδωμα κατάστασης.

**Περιορισμός των χρηστών από τη δημιουργία τοποθεσιών ή δευτερευουσών τοποθεσιών**

Ως διαχειριστής του SharePoint ή καθολικός διαχειριστής του Office 365, μπορείτε να αφήσετε τους χρήστες να δημιουργήσουν και να διαχειριστούν τις δικές τους τοποθεσίες του SharePoint, να καθορίσουν το είδος των τοποθεσιών που μπορούν να δημιουργήσουν και να καθορίσουν τη θέση των τοποθεσιών. Για περισσότερες πληροφορίες, ανατρέξτε [στο στοιχείο Διαχείριση δημιουργίας τοποθεσίας στο SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

