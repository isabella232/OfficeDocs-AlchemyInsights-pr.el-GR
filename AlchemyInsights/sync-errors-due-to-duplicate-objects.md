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
# <a name="sync-errors-due-to-duplicate-objects"></a>Σφάλματα συγχρονισμού λόγω διπλότυπων αντικειμένων

Ενδέχεται να λάβετε ένα από τα ακόλουθα μηνύματα λάθους όταν ολοκληρωθεί ο συγχρονισμός καταλόγου στο Microsoft 365:

- Δεν είναι δυνατή η ενημέρωση αυτού του αντικειμένου στις ηλεκτρονικές υπηρεσίες της Microsoft,επειδή τα ακόλουθα χαρακτηριστικά που σχετίζονται με αυτό το αντικείμενο έχουν τιμές που ενδέχεται να σχετίζονται ήδη με ένα άλλο αντικείμενο στον τοπικό σας κατάλογο.

- Υπάρχει ήδη ένα συγχρονισμένο αντικείμενο με την ίδια διεύθυνση διακομιστή μεσολάβησης στον κατάλογο των υπηρεσιών Microsoft Online Services.

- Δεν είναι δυνατή η ενημέρωση αυτού του αντικειμένου, επειδή τα ακόλουθα χαρακτηριστικά που σχετίζονται με αυτό το αντικείμενο έχουν τιμές που ενδέχεται να σχετίζονται ήδη με ένα άλλο αντικείμενο στις τοπικές υπηρεσίες καταλόγου: UserPrincipalName.

Για να εντοπίσετε και να διορθώσετε το ζήτημα, κάντε λήψη και εκτελέστε το [εργαλείο αποκατάστασης σφαλμάτων IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).

Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
