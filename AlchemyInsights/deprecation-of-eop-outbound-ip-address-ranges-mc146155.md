---
title: 1065 αποδοκιμασία του EOP εξερχόμενων IP διεύθυνση rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 0def0a93c61ea762918f1c9e6edb2e9b04446851
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30777272"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Αποδοκιμασία του EOP εξερχόμενων περιοχές διευθύνσεων IP

Μας έχετε εντοπίσει ένα πιθανό ζήτημα με τον οργανισμό σας που (αν δεν διορθωθεί με την εικοστή Οκτωβρίου 2018), ενδέχεται να καταστρέψετε ροή αλληλογραφίας σας εσωτερικής εγκατάστασης ή εξωτερικούς προορισμούς. Ως γνωστοποιείται προηγουμένως, για να απλοποιήσετε τη Διαχείριση περιοχής διευθύνσεων IP, εμείς συναθροίζετε τις περιοχές διευθύνσεων IP του Exchange Online προστασίας (EOP) που χρησιμοποιούνται για την αποστολή και λήψη ηλεκτρονικού ταχυδρομείου εκτός του Office 365. Την ανάλυση δηλώνει ότι μία ή περισσότερες από τις πηγές εξωτερικής ηλεκτρονικού ταχυδρομείου ή προορισμούς που ορίσατε στο συνδέσεις ροή αλληλογραφίας δεν δέχεται συνδέσεις από το IP διεύθυνση περιοχές εμφανίζονται [εδώ](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
  
Ενεργεί πριν από την εικοστή Οκτωβρίου, για τη διασφάλιση αυτών των πηγών και τους προορισμούς θα αποδεχτεί τις συνδέσεις προς και από όλα [δημοσιευτεί διευθύνσεις EOP IP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
  
Για περισσότερες πληροφορίες σχετικά με αυτήν την αλλαγή, δείτε καταχωρεί το Κέντρο μηνυμάτων [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ή [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).
  
 **Σημείωση**: Εάν χρησιμοποιούσατε προηγουμένως IP ή τη διεύθυνση URL δημοσίευσης μέσω HTML, XML και RSS για ενημερωμένες εκδόσεις του τελικού σημείου, μπορείτε επίσης θα πρέπει να μετεγκαταστήσετε των νέων υπηρεσιών web για την αυτοματοποίηση των αυτοί οι τύποι ενημερώσεων. Για περισσότερες πληροφορίες, ανατρέξτε στην ενότητα [κατηγορίες τελικού σημείου Office 365 και Office 365 IP διεύθυνση και διεύθυνση URL υπηρεσίας web](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
  

