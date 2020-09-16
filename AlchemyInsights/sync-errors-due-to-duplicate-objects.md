---
title: 902 (σφάλματα συγχρονισμού λόγω διπλότυπων αντικειμένων)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737341"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="5cdb3-102">Σφάλματα συγχρονισμού λόγω διπλότυπων αντικειμένων</span><span class="sxs-lookup"><span data-stu-id="5cdb3-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="5cdb3-103">Ενδέχεται να εμφανιστεί ένα από τα ακόλουθα μηνύματα σφάλματος, όταν ολοκληρωθεί ο συγχρονισμός καταλόγου στο Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="5cdb3-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="5cdb3-104">Δεν είναι δυνατή η ενημέρωση αυτού του αντικειμένου στις υπηρεσίες Microsoft Online Services, επειδή τα ακόλουθα χαρακτηριστικά που σχετίζονται με αυτό το αντικείμενο έχουν τιμές που μπορεί να έχουν ήδη συσχετιστεί με κάποιο άλλο αντικείμενο στον τοπικό σας κατάλογο.</span><span class="sxs-lookup"><span data-stu-id="5cdb3-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="5cdb3-105">Ένα συγχρονισμένο αντικείμενο με την ίδια διεύθυνση διακομιστή μεσολάβησης υπάρχει ήδη στον κατάλογο των υπηρεσιών Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="5cdb3-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="5cdb3-106">Δεν είναι δυνατή η ενημέρωση αυτού του αντικειμένου, επειδή τα ακόλουθα χαρακτηριστικά που σχετίζονται με αυτό το αντικείμενο έχουν τιμές που μπορεί να έχουν ήδη συσχετιστεί με ένα άλλο αντικείμενο στις τοπικές υπηρεσίες καταλόγου: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="5cdb3-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="5cdb3-107">Για να εντοπίσετε και να διορθώσετε το πρόβλημα, κάντε λήψη και εκτελέστε το [εργαλείο αποκατάστασης σφαλμάτων του IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="5cdb3-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="5cdb3-108">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="5cdb3-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
