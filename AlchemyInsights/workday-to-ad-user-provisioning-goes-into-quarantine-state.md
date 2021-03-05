---
title: Οι εργάσιμες ημέρες έως ad user provisioning πηγαίνουν σε κατάσταση καραντίνας
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481358"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="a026a-102">Οι εργάσιμες ημέρες έως ad user provisioning πηγαίνουν σε κατάσταση καραντίνας</span><span class="sxs-lookup"><span data-stu-id="a026a-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="a026a-103">**Οι εργάσιμες ημέρες έως ad user provisioning πηγαίνουν σε κατάσταση καραντίνας και δεν δημιουργούνται χρήστες στο AD**</span><span class="sxs-lookup"><span data-stu-id="a026a-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="a026a-104">Η εργασία "Εργάσιμη ημέρα σε παροχή χρήστη AD" έχει τεθεί σε κατάσταση καραντίνας και τα αρχεία καταγραφής ελέγχου εμφανίζουν συμβάντα αποτυχίας εξαγωγής με το μήνυμα **σφάλματος: OperationsError-SvcErr: Παρουσιάστηκε σφάλμα λειτουργίας. Δεν έχει ρυθμιστεί καμία ανώτερη αναφορά για την υπηρεσία καταλόγου. Επομένως, η υπηρεσία καταλόγου δεν είναι σε θέση να εκδώσει συστάσεις σε αντικείμενα εκτός αυτού του δάσους.**</span><span class="sxs-lookup"><span data-stu-id="a026a-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="a026a-105">Αυτό το σφάλμα εμφανίζεται συνήθως εάν η OU κοντέινερ της υπηρεσίας καταλόγου Active Directory δεν έχει οριστεί σωστά ή εάν υπάρχουν ζητήματα με την αντιστοίχιση παραστάσεων που χρησιμοποιείται για **το parentDistinguishedName.**</span><span class="sxs-lookup"><span data-stu-id="a026a-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="a026a-106">Ελέγξτε την προεπιλεγμένη OU για την **παράμετρο New Users** για λάθη κατά τη δημιουργία λάθη.</span><span class="sxs-lookup"><span data-stu-id="a026a-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="a026a-107">Βεβαιωθείτε ότι η καθορισμένη OU υπάρχει ήδη στο AD σας.</span><span class="sxs-lookup"><span data-stu-id="a026a-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="a026a-108">Εάν χρησιμοποιείτε το **parentDistinguishedName** στην αντιστοίχιση χαρακτηριστικών, βεβαιωθείτε ότι αυτό πάντα αξιολογείται σε ένα γνωστό κοντέινερ μέσα στον τομέα AD.</span><span class="sxs-lookup"><span data-stu-id="a026a-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="a026a-109">Ελέγξτε το συμβάν Export στα αρχεία καταγραφής ελέγχου για να δείτε την τιμή που δημιουργήθηκε.</span><span class="sxs-lookup"><span data-stu-id="a026a-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="a026a-110">Για περισσότερες λεπτομέρειες σχετικά με τη ρύθμιση παραμέτρων της εργάσιμης ημέρας για την αυτοματοποιημένη παροχή, ανατρέξτε στο πρόγραμμα εκμάθησης: Ρύθμιση [παραμέτρων εργάσιμης ημέρας για αυτόματη προμήθεια από χρήστες.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="a026a-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>

