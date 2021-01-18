---
title: Εικονική ρύθμιση παραμέτρων με τις υπηρεσίες τομέα AAD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885202"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Εικονική ρύθμιση παραμέτρων με τις υπηρεσίες τομέα AAD

Η εικονική ρύθμιση παραμέτρων με τις υπηρεσίες τομέα του AAD περιλαμβάνει τα παρακάτω βήματα: 

1. Έλεγχος της εύρυθμης λειτουργίας του τομέα σας στην πύλη Azure https://aka.ms/aadds-health
2. Έλεγχος του NSG για κανόνες που εμποδίζουν τις θύρες που απαιτούνται για το συγχρονισμό στις υπηρεσίες τομέα AD Azure στην πύλη https://aka.ms/aadds-networking
3. Διασφάλιση ότι το εικονικό σας δίκτυο αναπτύσσεται στην ίδια περιοχή Azure με τις υπηρεσίες τομέα AD Azure-διαχειριζόμενο τομέα.
4. Βεβαιωθείτε ότι δεν διαθέτετε τομέα με το ίδιο όνομα τομέα που είναι διαθέσιμο στο εικονικό δίκτυο.

Για περισσότερες λεπτομέρειες σχετικά με την εξέταση του σχεδιασμού στο εικονικό δίκτυο Azure για την υποστήριξη των υπηρεσιών τομέα AAD, ανατρέξτε στο θέμα [εικονικό δίκτυο εξέτασης](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).

