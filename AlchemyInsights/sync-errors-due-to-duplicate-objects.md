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
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998794"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Σφάλματα συγχρονισμού λόγω διπλότυπων αντικειμένων

Ενδέχεται να λάβετε ένα από τα ακόλουθα μηνύματα σφάλματος όταν ολοκληρωθεί ο συγχρονισμός καταλόγου Microsoft 365:

- Δεν είναι δυνατή η ενημέρωση αυτού του αντικειμένου στις υπηρεσίες Microsoft Online Services, επειδή τα ακόλουθα χαρακτηριστικά που σχετίζονται με αυτό το αντικείμενο έχουν τιμές που μπορεί να σχετίζονται ήδη με ένα άλλο αντικείμενο στον τοπικό κατάλογο.

- Ένα συγχρονισμένο αντικείμενο με την ίδια διεύθυνση διακομιστή μεσολάβησης υπάρχει ήδη στον κατάλογο των υπηρεσιών Microsoft Online Services.

- Δεν είναι δυνατή η ενημέρωση αυτού του αντικειμένου, επειδή τα ακόλουθα χαρακτηριστικά που σχετίζονται με αυτό το αντικείμενο έχουν τιμές που μπορεί να σχετίζονται ήδη με ένα άλλο αντικείμενο στις τοπικές υπηρεσίες καταλόγου: UserPrincipalName.

Για να προσδιορίσετε και να διορθώσετε το πρόβλημα, κάντε λήψη και εκτελέστε το [Εργαλείο αποκατάστασης σφαλμάτων IdFix DirSync.](https://github.com/Microsoft/idfix)

Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα KB2647098.](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)
