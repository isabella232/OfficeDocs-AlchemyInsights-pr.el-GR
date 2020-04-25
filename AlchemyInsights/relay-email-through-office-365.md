---
title: Μεταγωγή ηλεκτρονικού ταχυδρομείου μέσω του Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 4b36caf1841c5292d269812f4ab5ca16a46fbc81
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43785195"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="5aa61-102">Ρύθμιση μιας συσκευής ή μιας εφαρμογής πολλαπλών λειτουργιών για την αποστολή μηνύματος ηλεκτρονικού ταχυδρομείου</span><span class="sxs-lookup"><span data-stu-id="5aa61-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="5aa61-103">Για να μάθετε σχετικά με τις επιλογές και τα βήματα, ανατρέξτε στο θέμα [Πώς μπορείτε να ρυθμίσετε μια συσκευή ή μια εφαρμογή πολλαπλών λειτουργιών για αποστολή ηλεκτρονικού ταχυδρομείου με χρήση του Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span><span class="sxs-lookup"><span data-stu-id="5aa61-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span></span>
  
<span data-ttu-id="5aa61-104">**Σημείωση:** Εάν έχετε μια συσκευή ή μια εφαρμογή που σταμάτησε πρόσφατα να λειτουργεί, λάβετε υπόψη ότι έχουμε ξεκινήσει πρόσφατα την [απενεργοποίηση της κρυπτογράφησης 3DES](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption), όπως έχει προγραμματιστεί.</span><span class="sxs-lookup"><span data-stu-id="5aa61-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="5aa61-105">Για να δείτε τις συσκευές που επηρεάζονται μεταβείτε στο θέμα [Αναφορά προγραμμάτων-πελατών με έλεγχο ταυτότητας SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="5aa61-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="5aa61-106">Τα συνήθη σφάλματα θα μπορούσαν να είναι παρόμοια με: Αποτυχία/σφάλμα ελέγχου ταυτότητας, αποτυχία/σφάλμα TLS, σφάλμα αλγορίθμου κρυπτογράφησης, ασυμφωνία αλγορίθμου ή απόρριψη σύνδεσης.</span><span class="sxs-lookup"><span data-stu-id="5aa61-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="5aa61-107">Για να επιλύσετε το ζήτημα:</span><span class="sxs-lookup"><span data-stu-id="5aa61-107">To resolve the issue:</span></span>
 - <span data-ttu-id="5aa61-108">**Ο Windows Server 2003 IIS SMTP δεν θα λειτουργεί πλέον – απαιτείται μια νεότερη έκδοση των Windows.**</span><span class="sxs-lookup"><span data-stu-id="5aa61-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="5aa61-109">Συμβουλευτείτε τον προμηθευτή της εφαρμογής ή της συσκευής σας για να δείτε εάν υποστηρίζεται κάποια σύγχρονη κρυπτογράφηση ή αν υπάρχει ενημέρωση.</span><span class="sxs-lookup"><span data-stu-id="5aa61-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
