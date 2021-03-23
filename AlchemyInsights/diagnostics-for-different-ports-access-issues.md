---
title: Διαγνωστικά για προβλήματα πρόσβασης σε διαφορετικές θύρες
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035784"
---
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="461fe-102">Διαγνωστικά για προβλήματα πρόσβασης σε διαφορετικές θύρες</span><span class="sxs-lookup"><span data-stu-id="461fe-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="461fe-103">Για να επιλύσετε τα διάφορα προβλήματα πρόσβασης σε θύρα, ακολουθήστε τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="461fe-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="461fe-104">Διακόψτε/διακόψτε την εκχώρηση της εικονικής μηχανής (VM) από την πύλη, επανεκκινήστε την εικονική μηχανή και ελέγξτε ξανά.</span><span class="sxs-lookup"><span data-stu-id="461fe-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="461fe-105">Ελέγξτε τις ρυθμίσεις δικτύου της εικονικής μηχανής για να προσδιορίσετε εάν έχετε ομάδες ασφαλείας δικτύου (NSG) που εμποδίζουν την κυκλοφορία.</span><span class="sxs-lookup"><span data-stu-id="461fe-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="461fe-106">Μπορείτε επίσης να χρησιμοποιήσετε το εργαλείο επαλήθευσης ροής [IP](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) παρακολούθησης δικτύου για να ελέγξετε για NSG που εμποδίζουν την κυκλοφορία, δρομολογήσεις του User-Defined (UDR) που δρομολογούν ξανά την κυκλοφορία σας στην εσωτερική εγκατάσταση ('Προεπιλεγμένη δρομολόγηση' 0.0.0.0/0) ή σε μια συσκευή δικτύου.</span><span class="sxs-lookup"><span data-stu-id="461fe-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="461fe-107">Εάν εξακολουθείτε να αντιμετωπίζετε προβλήματα αφού δοκιμάσετε τα παραπάνω βήματα, δώστε το όνομα της εικονικής μηχανής και τη θύρα TCP στην οποία προσπαθείτε να στείλετε αλληλογραφία για περαιτέρω διάγνωση.</span><span class="sxs-lookup"><span data-stu-id="461fe-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="461fe-108">**Προτεινόμενα έγγραφα**</span><span class="sxs-lookup"><span data-stu-id="461fe-108">**Recommended Documents**</span></span>

[<span data-ttu-id="461fe-109">Περιορισμοί και συστάσεις για την αποστολή εξερχόμενων μηνυμάτων ηλεκτρονικού ταχυδρομείου μέσω της θύρας 25</span><span class="sxs-lookup"><span data-stu-id="461fe-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)