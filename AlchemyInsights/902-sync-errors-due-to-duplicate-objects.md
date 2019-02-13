---
title: 902 (σφάλματα συγχρονισμού λόγω διπλά αντικείμενα)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f576460547110e0e599a9062ae03f690792fe635
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29919872"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="3b045-102">Τα σφάλματα συγχρονισμού λόγω Διπλασιασμός αντικειμένων</span><span class="sxs-lookup"><span data-stu-id="3b045-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="3b045-103">Κατά την ολοκλήρωση του συγχρονισμού καταλόγου, ενδέχεται να λάβετε ένα από τα ακόλουθα μηνύματα λάθους:</span><span class="sxs-lookup"><span data-stu-id="3b045-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>
  
- <span data-ttu-id="3b045-104">Δεν είναι δυνατή η ενημέρωση αυτού του αντικειμένου στη Microsoft Online Services, επειδή τα ακόλουθα χαρακτηριστικά που σχετίζονται με αυτό το αντικείμενο έχει τιμές που μπορεί να είναι ήδη συσχετισμένη με άλλο αντικείμενο στον κατάλογο του τοπικού σας.</span><span class="sxs-lookup"><span data-stu-id="3b045-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>
    
- <span data-ttu-id="3b045-105">Υπάρχει ήδη ένα αντικείμενο συγχρονισμένοι με την ίδια διεύθυνση διακομιστή μεσολάβησης στον κατάλογο ηλεκτρονικές υπηρεσίες της Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3b045-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>
    
- <span data-ttu-id="3b045-106">Δεν είναι δυνατή η ενημέρωση αυτού του αντικειμένου, επειδή τα ακόλουθα χαρακτηριστικά που σχετίζονται με αυτό το αντικείμενο έχει τιμές που μπορεί να είναι ήδη συσχετισμένη με άλλο αντικείμενο σε υπηρεσίες σας τοπικό κατάλογο: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="3b045-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>
    
<span data-ttu-id="3b045-107">Για να εντοπίσετε και να διορθώσετε το ζήτημα, κάντε λήψη και εκτελέστε το [Εργαλείο αποκατάστασης εύρυθμης λειτουργίας σφάλμα Dirsync που είναι IdFix](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="3b045-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>
  
<span data-ttu-id="3b045-108">Για περισσότερες πληροφορίες, ανατρέξτε στην ενότητα [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="3b045-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
  

