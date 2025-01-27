---
title: το ίδιο με το όνομα αρχείου είναι καλύτερο
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: b6fbaf3f2ab30888d7a8f9d6f5aeccb65b5cfd0b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312825"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Απαιτείται Κεφαλίδα Alchemy H1, τα H2 δεν λειτουργούν".
Βέλτιστες πρακτικές και οδηγίες για τη σύνταξη του Alchemy:

1. **Μην κάνετε ένθεση του Alchemy Πληροφορίες φακέλους**- αυτό θα διακόψει τη δομή της διεύθυνσης URL. Προσπαθούμε να το διορθώσει αυτό.
1. Τα αρχεία στο **φάκελο AlchemyInsights** πρέπει να έχουν πεζά ονόματα αρχείων με ενωτικό για διαστήματα, π.χ. **_how-to-enable-litigation-hold._**
    1. Συμπεριλάβετε το αναγνωριστικό κανόνα ή το αναγνωριστικό κάδου από την πύλη [συνεργατών Alchemy](https://alchemyportal.azurewebsites.net) στο πεδίο ms.custom. π.χ. ***ms.custom: 100021***
1. Χρησιμοποιήστε τα υπόλοιπα μετα-δεδομένα στο επάνω μέρος αυτού του αρχείου ως πρότυπο.
1. Στην πύλη [συνεργατών της Alchemy,](https://alchemyportal.azurewebsites.net)μεταβείτε προς τα κάτω στην ενότητα Τίτλος **του Customer Insight:** και χρησιμοποιήστε την ως σημείο εκκίνησης για τον τίτλο H1 για να δείτε τις πληροφορίες. 

**Σημείωση:** Η alchemy Πληροφορίες ΠΡΕΠΕΙ να έχει μόνο ένα H1 στο επάνω μέρος ή θα διακόψει την παραγωγή. Τα H2 δεν αποδίδονται, επομένως χρησιμοποιήστε έντονη **γραφή** ή άλλες συμβάσεις για να υπογράψετε ξεχωριστές ενότητες.
1. Στη συνέχεια, συμπληρώστε το σώμα κειμένου χρησιμοποιώντας το πρόχειρο υλικό στην Πληροφορίες πελατών της σελίδας "Κανόνας Alchemy"
    1. Οι λίστες με κουκκίδες είναι εντάξει
    1. Επίσης, οι λίστες με αρίθμηση
    1. **Η** έντονη *γραφή και η πλάγια* γραφή είναι εντάξει
    1. Οι συνδέσεις θα πρέπει πάντα **να είναι "συνδέσεις στο web"/εξωτερικές** ή **βαθιές συνδέσεις σε στοιχεία περιβάλλοντος εργασίας χρήστη** και όχι εσωτερικές συνδέσεις.
    1. Οι εικόνες δεν υποστηρίζονται επίσημα αυτήν τη στιγμή, αλλά βρίσκονται στον χάρτη.

Και αυτό είναι πραγματικά πάρα πολύ μεγάλο. Η βέλτιστη πρακτική είναι περίπου 400 χαρακτήρες ---------------------------------

Όταν το περιεχόμενό σας είναι έτοιμο, τραβήξτε το στο ζωντανό κλάδο. Στη συνέχεια, μεταβείτε στην [πύλη συνεργατών alchemy και](https://alchemyportal.azurewebsites.net) εισαγάγετε το όνομα αρχείου στο πεδίο διεύθυνσης URL. 