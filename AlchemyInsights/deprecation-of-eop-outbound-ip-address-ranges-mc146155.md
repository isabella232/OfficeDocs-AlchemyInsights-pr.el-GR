---
title: 1065 Deprecation of EOP outbound IP address rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031262"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Απόσβεση των τιμών διευθύνσεων IP εξερχομένων EOP

Εντοπίσαμε ένα πιθανό πρόβλημα με τον οργανισμό σας το οποίο (εάν δεν διορθωθεί έως τις 26 Οκτωβρίου 2018) ενδέχεται να διακόψει τη ροή αλληλογραφίας προς τους προορισμούς εσωτερικής εγκατάστασης ή εξωτερικούς προορισμούς σας. Όπως αναφέρθηκε προηγουμένως, για να απλοποιήσουμε τη διαχείριση της περιοχής διευθύνσεων IP, ενοποιούμε τις περιοχές διευθύνσεων IP του Exchange Online Protection (EOP) που χρησιμοποιούνται για την αποστολή και λήψη μηνυμάτων ηλεκτρονικού ταχυδρομείου εκτός των Microsoft 365. Η ανάλυσή μας υποδεικνύει ότι μία ή περισσότερες από τις εξωτερικές προελεύσεις ή προορισμούς ηλεκτρονικού ταχυδρομείου που έχετε ρυθμίσει στις γραμμές σύνδεσης ροής αλληλογραφίας δεν αποδέχονται συνδέσεις από τις περιοχές διευθύνσεων IP που εμφανίζονται [εδώ.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Ενεργείστε πριν από τις 26 Οκτωβρίου για να εξασφαλίσετε ότι αυτές οι πηγές και οι προορισμοί θα αποδέχονται συνδέσεις από και προς όλες [τις δημοσιευμένες διευθύνσεις IP του EOP.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Για περισσότερες πληροφορίες σχετικά με αυτή την αλλαγή, ανατρέξτε στις δημοσιεύσεις ΤΟΥ Κέντρου μηνυμάτων [MC146155,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155) [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ή [MC149274.](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)

**Σημείωση:** Εάν είχατε χρησιμοποιήσει προηγουμένως τη δημοσίευση διευθύνσεων IP ή ΔΙΕΎΘΥΝΣΗς URL μέσω HTML, XML και RSS για ενημερώσεις τελικού σημείου, θα πρέπει επίσης να κάνετε μετεγκατάσταση στις νέες υπηρεσίες Web για την αυτοματοποίηση αυτών των τύπων ενημερώσεων. Για περισσότερες πληροφορίες, ανατρέξτε [Microsoft 365 κατηγορίες τελικού σημείου και Microsoft 365 διεύθυνση IP και υπηρεσία Web διευθύνσεων URL.](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)
