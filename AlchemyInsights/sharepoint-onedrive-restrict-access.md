---
title: Περιορισμός της πρόσβασης στο SharePoint ή OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 84f2d4b6e5fd2380a2fa96e30953c68aab203cd3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559877"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Περιορισμός της πρόσβασης στο SharePoint ή OneDrive

Υπάρχουν πολλοί τρόποι για να περιορίσετε την πρόσβαση σε υπηρεσίες SharePoint Online/OneDrive. Αυτές οι διάφορες μέθοδοι περιορισμού πρόσβασης περιγράφονται παρακάτω. 

**Περιορισμός δικαιωμάτων**

Στην ηλεκτρονική SharePoint και OneDrive για την επιχείρηση, μας περιορίσετε την πρόσβαση σε στοιχεία όπως τοποθεσίες, αρχεία και φακέλους παρέχοντας πρόσβαση σε αυτές τις ομάδες/άτομα που θα πρέπει να έχουν πρόσβαση μόνο.

- [Προσαρμογή των δικαιωμάτων για μια λίστα ή βιβλιοθήκη SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Προσαρμογή των δικαιωμάτων τοποθεσίας του SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Αλλάξτε τα δικαιώματα σε έναν υποφάκελο](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Έλεγχος της πρόσβασης από μη διαχειριζόμενη συσκευές](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Ως καθολικής διαχείρισης του Office 365 ή του SharePoint, μπορείτε να αποκλείσετε ή να περιορίσετε την πρόσβαση στο περιεχόμενο του SharePoint και OneDrive από μη διαχειριζόμενη συσκευές (αυτών υβριδική AD συνδεδεμένα ή συμβατός με στο Intune).

**Περιορισμός θέση δικτύου**

Ως ένας διαχειριστής IT, μπορείτε να ελέγξετε την πρόσβαση σε πόρους του SharePoint και OneDrive που βασίζονται σε αξιόπιστες τοποθεσίες δικτύου ορίζεται. Αυτό είναι επίσης γνωστό ως πολιτική που βασίζεται σε θέση. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Έλεγχος της πρόσβασης σε ηλεκτρονική SharePoint και OneDrive δεδομένα με βάση τη θέση δικτύου](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Περιορισμού κλείδωμα τοποθεσίας** 

Εντός του SharePoint Online, έχετε τη δυνατότητα να κλειδώσετε μια συλλογή τοποθεσιών, ώστε κανείς να έχει πρόσβαση. Αυτό ορίζεται μέσω του PowerShell και το [SharePoint Online κέλυφος διαχείρισης](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) χρησιμοποιώντας την ιδιότητα - LockState [Σύνολο SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) .

**Περιορισμός των χρηστών από τη δημιουργία τοποθεσιών και δευτερευουσών τοποθεσιών**

Ως διαχειριστής SharePoint ή καθολικής διαχείρισης του Office 365, μπορείτε να επιτρέψετε στους χρήστες σας να δημιουργήσετε και να διαχειριστείτε τις δικές τους τοποθεσίες του SharePoint, καθορίζουν το είδος των τοποθεσιών μπορούν να δημιουργήσουν, και καθορίστε τη θέση των τοποθεσιών. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Διαχείριση δημιουργίας τοποθεσίας στο SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

