---
title: Πρόβλημα με τη συμμετοχή στο ΣΠΣ
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
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885211"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="a2805-102">Πρόβλημα με τη συμμετοχή στο ΣΠΣ</span><span class="sxs-lookup"><span data-stu-id="a2805-102">Issue joining VMs</span></span>

<span data-ttu-id="a2805-103">Για να επιλύσετε ζητήματα που προκύπτουν κατά την προσπάθεια συμμετοχής στο ΣΠΣ, εκτελέστε τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="a2805-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="a2805-104">Προσπαθήστε να συνδεθείτε χρησιμοποιώντας τη μορφή **UPN** (για παράδειγμα, "JoeUser@contoso.com") αντί για τη μορφή **sAMAccountName** (' CONTOSO\joeuser ').</span><span class="sxs-lookup"><span data-stu-id="a2805-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="a2805-105">Βεβαιωθείτε ότι έχετε ενεργοποιήσει το συγχρονισμό κωδικών πρόσβασης σύμφωνα με τα βήματα που περιγράφονται στον οδηγό " *γρήγορα αποτελέσματα* ".</span><span class="sxs-lookup"><span data-stu-id="a2805-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="a2805-106">Βεβαιωθείτε ότι ο λογαριασμός χρήστη που επηρεάζεται δεν είναι εξωτερικός λογαριασμός στον μισθωτή AD Azure.</span><span class="sxs-lookup"><span data-stu-id="a2805-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="a2805-107">Οι εξωτερικοί χρήστες δεν μπορούν να εισέλθετε στον διαχειριζόμενο τομέα, επειδή οι υπηρεσίες τομέα AD Azure δεν έχουν διαπιστευτήρια για τέτοιους λογαριασμούς χρηστών.</span><span class="sxs-lookup"><span data-stu-id="a2805-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="a2805-108">Εάν ο λογαριασμός χρήστη που επηρεάζεται είναι ένας λογαριασμός χρήστη μόνο στο cloud, βεβαιωθείτε ότι οι χρήστες έχουν αλλάξει τον κωδικό πρόσβασής τους μετά την ενεργοποίηση των υπηρεσιών τομέα AD Azure.</span><span class="sxs-lookup"><span data-stu-id="a2805-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="a2805-109">Αυτό το βήμα προκαλεί τους κατακερματισμούς διαπιστευτηρίων που απαιτούνται για τις υπηρεσίες τομέα AD Azure που θα δημιουργηθούν.</span><span class="sxs-lookup"><span data-stu-id="a2805-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="a2805-110">Εάν οι λογαριασμοί χρηστών που επηρεάζονται συγχρονίζονται από έναν κατάλογο εσωτερικής εγκατάστασης, βεβαιωθείτε ότι η συνιστώμενη κυκλοφορία του Azure AD Connect έχει ρυθμιστεί ώστε να εκτελεί έναν πλήρη συγχρονισμό.</span><span class="sxs-lookup"><span data-stu-id="a2805-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="a2805-111">Εάν τα προβλήματα επιμένουν μετά την επιβεβαίωση του βήματος 4, εκτελέστε τις ακόλουθες εντολές από τον υπολογιστή συγχρονισμού:</span><span class="sxs-lookup"><span data-stu-id="a2805-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="a2805-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="a2805-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>