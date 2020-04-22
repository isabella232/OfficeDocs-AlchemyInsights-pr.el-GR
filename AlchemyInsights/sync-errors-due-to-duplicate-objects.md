---
title: 902 (Σφάλματα συγχρονισμού λόγω διπλότυπων αντικειμένων)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767127"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="167fc-102">Σφάλματα συγχρονισμού λόγω διπλότυπων αντικειμένων</span><span class="sxs-lookup"><span data-stu-id="167fc-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="167fc-103">Ενδέχεται να λάβετε ένα από τα ακόλουθα μηνύματα λάθους όταν ολοκληρωθεί ο συγχρονισμός καταλόγου στο Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="167fc-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="167fc-104">Δεν είναι δυνατή η ενημέρωση αυτού του αντικειμένου στις ηλεκτρονικές υπηρεσίες της Microsoft,επειδή τα ακόλουθα χαρακτηριστικά που σχετίζονται με αυτό το αντικείμενο έχουν τιμές που ενδέχεται να σχετίζονται ήδη με ένα άλλο αντικείμενο στον τοπικό σας κατάλογο.</span><span class="sxs-lookup"><span data-stu-id="167fc-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="167fc-105">Υπάρχει ήδη ένα συγχρονισμένο αντικείμενο με την ίδια διεύθυνση διακομιστή μεσολάβησης στον κατάλογο των υπηρεσιών Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="167fc-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="167fc-106">Δεν είναι δυνατή η ενημέρωση αυτού του αντικειμένου, επειδή τα ακόλουθα χαρακτηριστικά που σχετίζονται με αυτό το αντικείμενο έχουν τιμές που ενδέχεται να σχετίζονται ήδη με ένα άλλο αντικείμενο στις τοπικές υπηρεσίες καταλόγου: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="167fc-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="167fc-107">Για να εντοπίσετε και να διορθώσετε το ζήτημα, κάντε λήψη και εκτελέστε το [εργαλείο αποκατάστασης σφαλμάτων IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="167fc-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="167fc-108">Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="167fc-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
