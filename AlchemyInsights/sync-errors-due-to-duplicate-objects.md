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
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: ce7eeb07cfde16e6d6856a9369c042dcf4f05b63
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420881"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Τα σφάλματα συγχρονισμού λόγω Διπλασιασμός αντικειμένων

Κατά την ολοκλήρωση του συγχρονισμού καταλόγου, ενδέχεται να λάβετε ένα από τα ακόλουθα μηνύματα λάθους:

- Δεν είναι δυνατή η ενημέρωση αυτού του αντικειμένου στη Microsoft Online Services, επειδή τα ακόλουθα χαρακτηριστικά που σχετίζονται με αυτό το αντικείμενο έχει τιμές που μπορεί να είναι ήδη συσχετισμένη με άλλο αντικείμενο στον κατάλογο του τοπικού σας.

- Υπάρχει ήδη ένα αντικείμενο συγχρονισμένοι με την ίδια διεύθυνση διακομιστή μεσολάβησης στον κατάλογο ηλεκτρονικές υπηρεσίες της Microsoft.

- Δεν είναι δυνατή η ενημέρωση αυτού του αντικειμένου, επειδή τα ακόλουθα χαρακτηριστικά που σχετίζονται με αυτό το αντικείμενο έχει τιμές που μπορεί να είναι ήδη συσχετισμένη με άλλο αντικείμενο σε υπηρεσίες σας τοπικό κατάλογο: UserPrincipalName.

Για να εντοπίσετε και να διορθώσετε το ζήτημα, κάντε λήψη και εκτελέστε το [Εργαλείο αποκατάστασης εύρυθμης λειτουργίας σφάλμα Dirsync που είναι IdFix](https://www.microsoft.com/download/details.aspx?id=36832).

Για περισσότερες πληροφορίες, ανατρέξτε στην ενότητα [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
