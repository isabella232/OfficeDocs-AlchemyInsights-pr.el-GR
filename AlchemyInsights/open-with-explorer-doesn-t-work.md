---
title: Άνοιγμα με την Εξερεύνηση δεν λειτουργεί
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: b55fc7bd5670e655334ef7be368b245c8899633a
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28290367"
---
# <a name="open-with-explorer-isnt-working"></a>Άνοιγμα με την Εξερεύνηση δεν λειτουργεί

Εάν δεν λειτουργεί η **προβολή στην Εξερεύνηση αρχείου** ή **Άνοιγμα με την Εξερεύνηση** βεβαιωθείτε ότι η υπηρεσία WebClient έχει οριστεί να **εκτελεί** , ακολουθώντας τα παρακάτω βήματα. Για παράδειγμα, ίσως χρειαστούν πολύ χρόνο για να ανοίξετε μια βιβλιοθήκη του SharePoint ή OneDrive, όταν δεν εκτελείται η υπηρεσία. 
  
1. Στο πλαίσιο αναζήτησης των Windows, πληκτρολογήστε εκτέλεση, επιλέξτε το app επιφάνειας εργασίας εκτέλεση, πληκτρολογήστε services.msc και, στη συνέχεια, επιλέξτε **Enter**.
    
2. Κάντε κύλιση έως την υπηρεσία WebClient και ελέγξτε τη στήλη **κατάστασης** . Εάν η κατάσταση της υπηρεσίας WebClient δεν **εκτελείται**, κάντε διπλό κλικ στην υπηρεσία, κάντε κλικ στο κουμπί **Έναρξη**και στη συνέχεια κάντε κλικ στο κουμπί **OK**. Ενεργοποίηση της υπηρεσίας, εάν χρειάζεται, με την επιλογή **μη αυτόματη** ή **Αυτόματη** στο πλαίσιο **Τύπος εκκίνησης** . 
    
> [!NOTE]
> Για την αντιμετώπιση ζητημάτων ανοίγοντας στην Εξερεύνηση αρχείων, ανατρέξτε στην ενότητα [Άνοιγμα στην Εξερεύνηση](https://go.microsoft.com/fwlink/?linkid=871665). Εξερευνήστε συγχρονισμού ως μια καλύτερη εναλλακτική λύση: [αρχεία συγχρονισμού του SharePoint με το πρόγραμμα-πελάτης συγχρονισμού νέα OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

