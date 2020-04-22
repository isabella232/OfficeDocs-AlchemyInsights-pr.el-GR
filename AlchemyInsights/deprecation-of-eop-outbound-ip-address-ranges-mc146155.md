---
title: 1065 Αποδοκιμασία της εξερχόμενης διεύθυνσης IP του EOP rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704597"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Αποδοκιμασία των περιοχών εξερχόμενων διευθύνσεων IP του EOP

Εντοπίσαμε ένα πιθανό πρόβλημα με τον οργανισμό σας το οποίο (αν δεν διορθωθεί έως τις 26 Οκτωβρίου 2018) ενδέχεται να διακόψει τη ροή αλληλογραφίας στους προορισμούς εσωτερικής εγκατάστασης ή εξωτερικούς προορισμούς σας. Όπως κοινοποιήθηκε προηγουμένως, για να απλοποιήσουμε τη διαχείριση εύρους διευθύνσεων IP, ενοποιούμε τις περιοχές διευθύνσεων IP της Ηλεκτρονικής προστασίας (EOP) του Exchange που χρησιμοποιούνται για την αποστολή και λήψη μηνυμάτων ηλεκτρονικού ταχυδρομείου εκτός του Microsoft 365. Η ανάλυσή μας δείχνει ότι μία ή περισσότερες από τις εξωτερικές πηγές ηλεκτρονικού ταχυδρομείου ή προορισμούς που έχετε ρυθμίσει σε συνδέσεις ροής αλληλογραφίας δεν δέχονται συνδέσεις από τις περιοχές διευθύνσεων IP που εμφανίζονται [εδώ](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Πράξη πριν από τις 26 Οκτωβρίου για να διασφαλίσετε ότι αυτές οι πηγές και οι προορισμοί θα δέχονται συνδέσεις από και [προς όλες τις δημοσιευμένες διευθύνσεις IP του ΕΟΠ](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Για περισσότερες πληροφορίες σχετικά με αυτήν την αλλαγή, ανατρέξτε στο θέμα Δημοσιεύσεις κέντρου μηνυμάτων [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ή [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Σημείωση:** Εάν χρησιμοποιήσατε προηγουμένως τη δημοσίευση IP ή URL μέσω HTML, XML και RSS για ενημερώσεις τελικού σημείου, θα πρέπει επίσης να κάνετε μετεγκατάσταση στις νέες υπηρεσίες web για την αυτοματοποίηση αυτών των τύπων ενημερωμένων εκδόσεων. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Κατηγορίες τελικού σημείου microsoft 365 και διεύθυνση IP microsoft 365 και υπηρεσία web URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
