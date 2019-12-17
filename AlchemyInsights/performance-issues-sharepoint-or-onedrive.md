---
title: Ζητήματα επιδόσεων-SharePoint ή OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068402"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>Το SharePoint ή το OneDrive αργή, απρόσιτη ή μη διαθέσιμη για πολλούς χρήστες

Το SharePoint ή το OneDrive ενδέχεται να είναι αργή, απρόσιτη ή μη διαθέσιμη ή μπορεί να εμφανίσει μη διαθέσιμα ή 503 σφάλματα υπηρεσίας, για διάφορους λόγους:
  
- Εάν η τοποθεσία του SharePoint ή του OneDrive είναι αργή ή καθυστερεί για πολλούς χρήστες, ενδέχεται να υπάρχει ένα ζήτημα προσωρινής υπηρεσίας όπου οι χρήστες αντιμετωπίζουν διακοπτόμενες καθυστερήσεις ή σφάλματα περιήγησης κατά την πρόσβαση σε τοποθεσίες του SharePoint ή περιεχόμενο OneDrive. Ελέγξτε τον [πίνακα εργαλείων εύρυθμης λειτουργίας της υπηρεσίας](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , για να δείτε αν επηρεάζεται ο οργανισμός σας.
  
- Οι χρήστες ενδέχεται να λάβετε ένα *503 διακομιστή είναι απασχολημένος* σφάλμα κατά την προσπάθεια περιήγησης σε τοποθεσίες του SharePoint ή OneDrive. Αυτό το σφάλμα μπορεί να προκληθεί από επιτάχυνση εντός της υπηρεσίας SharePoint. Ηλεκτρονική SharePoint χρησιμοποιεί επιτάχυνσης για να διατηρήσετε τη βέλτιστη απόδοση και την αξιοπιστία της υπηρεσίας SharePoint Online. Ο περιορισμός περιορίζει τον αριθμό των ενεργειών χρήστη ή των ταυτόχρονων κλήσεων (με δέσμη ενεργειών ή κώδικα) για την αποτροπή της υπερβολικής χρήσης πόρων. Για περισσότερες πληροφορίες σχετικά με την επιτάχυνση δείτε, [Αποφύγετε να έχετε επιβραδύνει ή να αποκλειστεί στο SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Εάν αντιμετωπίζετε χαμηλές επιδόσεις με μια **κλασική** ή **σύγχρονη** τοποθεσία ή σελίδα του SharePoint, χρησιμοποιήστε το [διαγνωστικό εργαλείο σελίδας](https://aka.ms/perftool) για να αναλύσετε τις σελίδες.
  
- Εάν εξακολουθείτε να αντιμετωπίζετε γενικές χαμηλές επιδόσεις, ελέγξτε τους πόρους στο κάτω μέρος αυτού του άρθρου: [Εισαγωγή στο συντονισμό επιδόσεων για το SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  