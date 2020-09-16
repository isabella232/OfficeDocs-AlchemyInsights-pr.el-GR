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
# <a name="sync-errors-due-to-duplicate-objects"></a>Σφάλματα συγχρονισμού λόγω διπλότυπων αντικειμένων

Ενδέχεται να εμφανιστεί ένα από τα ακόλουθα μηνύματα σφάλματος, όταν ολοκληρωθεί ο συγχρονισμός καταλόγου στο Microsoft 365:

- Δεν είναι δυνατή η ενημέρωση αυτού του αντικειμένου στις υπηρεσίες Microsoft Online Services, επειδή τα ακόλουθα χαρακτηριστικά που σχετίζονται με αυτό το αντικείμενο έχουν τιμές που μπορεί να έχουν ήδη συσχετιστεί με κάποιο άλλο αντικείμενο στον τοπικό σας κατάλογο.

- Ένα συγχρονισμένο αντικείμενο με την ίδια διεύθυνση διακομιστή μεσολάβησης υπάρχει ήδη στον κατάλογο των υπηρεσιών Microsoft Online Services.

- Δεν είναι δυνατή η ενημέρωση αυτού του αντικειμένου, επειδή τα ακόλουθα χαρακτηριστικά που σχετίζονται με αυτό το αντικείμενο έχουν τιμές που μπορεί να έχουν ήδη συσχετιστεί με ένα άλλο αντικείμενο στις τοπικές υπηρεσίες καταλόγου: UserPrincipalName.

Για να εντοπίσετε και να διορθώσετε το πρόβλημα, κάντε λήψη και εκτελέστε το [εργαλείο αποκατάστασης σφαλμάτων του IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).

Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
