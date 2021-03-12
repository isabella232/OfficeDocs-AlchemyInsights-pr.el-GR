---
title: Σύνολο ρεπλίκας
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50713749"
---
# <a name="replica-set"></a><span data-ttu-id="2b40f-102">Σύνολο ρεπλίκας</span><span class="sxs-lookup"><span data-stu-id="2b40f-102">Replica set</span></span>

<span data-ttu-id="2b40f-103">Το AADDS ονομάζεται επίσης διαχειριζόμενος τομέας.</span><span class="sxs-lookup"><span data-stu-id="2b40f-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="2b40f-104">Στην πραγματικότητα είναι δύο ελεγκτές τομέα που εκτελούνται και διατηρούνται από το backend.</span><span class="sxs-lookup"><span data-stu-id="2b40f-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="2b40f-105">Οι δύο DCs περιλαμβάνουν έναν κύριο DC και έναν dc αναπαραγωγής.</span><span class="sxs-lookup"><span data-stu-id="2b40f-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="2b40f-106">Τα αντίγραφα ασφαλείας στο AADDS (διαχειριζόμενος τομέας) είναι μια αυτοματοποιημένη διαδικασία που διαχειρίζεται η πλατφόρμα Azure.</span><span class="sxs-lookup"><span data-stu-id="2b40f-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="2b40f-107">Σε περίπτωση προβλήματος με τον διαχειριζόμενο τομέα σας, η υποστήριξη του Azure μπορεί να σας βοηθήσει στην επαναφορά από το αντίγραφο ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="2b40f-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="2b40f-108">Μπορείτε να δημιουργήσετε κάθε σύνολο ρεπλίκας σε ένα εικονικό δίκτυο.</span><span class="sxs-lookup"><span data-stu-id="2b40f-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="2b40f-109">Κάθε εικονικό δίκτυο πρέπει να είναι ομότιμο με κάθε άλλο εικονικό δίκτυο που φιλοξενεί το σύνολο ρεπλίκας ενός διαχειριζόμενου τομέα.</span><span class="sxs-lookup"><span data-stu-id="2b40f-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="2b40f-110">Αυτή η ρύθμιση παραμέτρων δημιουργεί μια τοπολογία δικτύου πλέγματος που υποστηρίζει την αναπαραγωγή καταλόγου.</span><span class="sxs-lookup"><span data-stu-id="2b40f-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="2b40f-111">Ένα εικονικό δίκτυο μπορεί να υποστηρίζει πολλά σύνολα ρεπλίκας, υπό την προϋπόθεση ότι κάθε σύνολο ρεπλίκας βρίσκεται σε διαφορετικό εικονικό υποδίκτυο.</span><span class="sxs-lookup"><span data-stu-id="2b40f-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="2b40f-112">Για περισσότερες λεπτομέρειες σχετικά με το σύνολο ρεπλίκας, ανατρέξτε στο θέμα [Σύνολα εννοιών ρεπλίκας.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)</span><span class="sxs-lookup"><span data-stu-id="2b40f-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
