---
title: 902 (Σφάλματα συγχρονισμού λόγω διπλότυπων αντικειμένων)
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
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708062"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="854e1-102">Σφάλματα συγχρονισμού λόγω διπλότυπων αντικειμένων</span><span class="sxs-lookup"><span data-stu-id="854e1-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="854e1-103">Ενδέχεται να λάβετε ένα από τα ακόλουθα μηνύματα σφάλματος όταν ολοκληρωθεί ο συγχρονισμός καταλόγου στο Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="854e1-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="854e1-104">Δεν είναι δυνατή η ενημέρωση αυτού του αντικειμένου στις υπηρεσίες Microsoft Online Services, επειδή τα παρακάτω χαρακτηριστικά που σχετίζονται με αυτό το αντικείμενο έχουν τιμές που μπορεί να σχετίζονται ήδη με ένα άλλο αντικείμενο στον τοπικό κατάλογο.</span><span class="sxs-lookup"><span data-stu-id="854e1-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="854e1-105">Ένα συγχρονισμένο αντικείμενο με την ίδια διεύθυνση διακομιστή μεσολάβησης υπάρχει ήδη στον κατάλογο των υπηρεσιών Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="854e1-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="854e1-106">Δεν είναι δυνατή η ενημέρωση αυτού του αντικειμένου, επειδή τα παρακάτω χαρακτηριστικά που σχετίζονται με αυτό το αντικείμενο έχουν τιμές που μπορεί να σχετίζονται ήδη με ένα άλλο αντικείμενο στις τοπικές υπηρεσίες καταλόγου: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="854e1-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="854e1-107">Για να εντοπίσετε και να διορθώσετε το πρόβλημα, κάντε λήψη και εκτελέστε το Εργαλείο [αποκατάστασης σφαλμάτων DirSync του IdFix.](https://github.com/Microsoft/idfix)</span><span class="sxs-lookup"><span data-stu-id="854e1-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://github.com/Microsoft/idfix).</span></span>

<span data-ttu-id="854e1-108">Για περισσότερες πληροφορίες, ανατρέξτε [στο KB2647098.](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)</span><span class="sxs-lookup"><span data-stu-id="854e1-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
