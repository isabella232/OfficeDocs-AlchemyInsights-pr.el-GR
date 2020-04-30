---
title: MC210173 - νέα προσαρμοσμένη δυνατότητα κατάργησης φόρμας του SharePoint Designer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 185e8fc94345b240667490b1ffc63af8459d8daf
ms.sourcegitcommit: a9e6b2fcce8bd12fd079ed967f426b67d5c6d239
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43928528"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a><span data-ttu-id="e2c86-102">MC210173 - νέα προσαρμοσμένη δυνατότητα κατάργησης φόρμας του SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="e2c86-102">MC210173 - SharePoint Designer new custom Form feature deprecation</span></span>

<span data-ttu-id="e2c86-103">Εντοπίσαμε ένα πρόβλημα που επηρεάζει τη λειτουργικότητα του SharePoint Designer σχετικά με τη [δημιουργία προσαρμοσμένων φορμών](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) στο SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="e2c86-103">We’ve identified an issue affecting SharePoint Designer functionality for [creating custom Forms](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) within SharePoint Online.</span></span> <span data-ttu-id="e2c86-104">Μετά από προσεκτική εξέταση, διαπιστώσαμε ότι δεν υπάρχει γνωστή επιδιόρθωση για αυτό το πρόβλημα και επιλέξαμε να απενεργοποιήσουμε τη δυνατότητα "Δημιουργία προσαρμοσμένης φόρμας" με ισχύ από το Σάββατο 25 Απριλίου 2020 στις 3:00 Π.Μ. UTC.</span><span class="sxs-lookup"><span data-stu-id="e2c86-104">After careful examination, we’ve determined that there is no known fix for this issue and have elected to disable the custom Form creation feature effective as of 3:00 AM UTC on Saturday, April 25, 2020.</span></span> <span data-ttu-id="e2c86-105">Αυτή η αλλαγή δεν επηρεάζει τη δυνατότητα επεξεργασίας φορμών που δημιουργήθηκαν στο παρελθόν ή άλλων υφιστάμενων δυνατοτήτων στο SharePoint Online Designer.</span><span class="sxs-lookup"><span data-stu-id="e2c86-105">This change does not impact the ability to edit previously created Forms or other existing features in SharePoint Online Designer.</span></span>

<span data-ttu-id="e2c86-106">Μετά από αυτή την αλλαγή, οι χρήστες ενδέχεται να έχουν λάβει το μήνυμα σφάλματος: "Δεν ήταν δυνατή η αποθήκευση των αλλαγών λίστας στο διακομιστή" κατά τη δημιουργία νέων φορμών.</span><span class="sxs-lookup"><span data-stu-id="e2c86-106">After this change was made, users may have received the error: "Could not save the list changes to the server," when creating new Forms.</span></span>

<span data-ttu-id="e2c86-107">Οι χρήστες που έχουν αξιοποιήσει το SharePoint Designer, στο παρελθόν, για να δημιουργήσουν προσαρμοσμένες φόρμες, μπορούν, για τον ίδιο σκοπό και αντί αυτού να χρησιμοποιούν το [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form).</span><span class="sxs-lookup"><span data-stu-id="e2c86-107">Users who have previously leveraged SharePoint Designer to create custom Forms are instead able to utilize [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) for this purpose.</span></span>

<span data-ttu-id="e2c86-108">Το PowerApps είναι ένα εύκολο και ισχυρό εργαλείο που επιτρέπει στους χρήστες που λειτουργούν με τη σύγχρονη εμπειρία του SharePoint Online να δημιουργούν και να επεξεργάζονται προσαρμοσμένες φόρμες για λίστες και βιβλιοθήκες εγγράφων SharePoint, απευθείας από ένα παράθυρο προγράμματος περιήγησης.</span><span class="sxs-lookup"><span data-stu-id="e2c86-108">PowerApps is an easy and powerful tool that allows users operating in the SharePoint Online Modern experience to create and edit custom Forms for SharePoint lists and document libraries right from a browser window.</span></span> <span data-ttu-id="e2c86-109">Το PowerApps δεν απαιτεί γνώσεις παραδοσιακής κωδικοποίησης ή τυχόν πρόσθετες λήψεις εφαρμογών, όπως το InfoPath.</span><span class="sxs-lookup"><span data-stu-id="e2c86-109">PowerApps does not require traditional coding knowledge or any additional app downloads such as InfoPath.</span></span>

<span data-ttu-id="e2c86-110">**Σημείωση**: οι χρήστες του SharePoint Online Classic θα πρέπει να στραφούν προσωρινά στη σύγχρονη εμπειρία για να αποκτήσουν πρόσβαση και να χρησιμοποιήσουν το PowerApps. Ωστόσο, όλες οι προσαρμοσμένες φόρμες που έχουν δημιουργηθεί στο PowerApps είναι προσβάσιμες από χρήστες του SharePoint Online Classic.</span><span class="sxs-lookup"><span data-stu-id="e2c86-110">**Note**: SharePoint Online Classic users will need to temporarily switch to the Modern experience to access and utilize PowerApps; though, all custom Forms created in PowerApps are accessible by SharePoint Online Classic experience users.</span></span>
