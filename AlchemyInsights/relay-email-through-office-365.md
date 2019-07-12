---
title: Μεταγωγή ηλεκτρονικού ταχυδρομείου μέσω του Office 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 9/21/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 3c056f5c78935adcf0b64779f9632f9336080a40
ms.sourcegitcommit: dce9cf9bb05d29f0f9bab61fe3fc25e99f0cebf1
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 07/11/2019
ms.locfileid: "35630741"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email-using-office-365"></a><span data-ttu-id="3ccd5-102">Ρύθμιση μιας συσκευής ή μιας εφαρμογής πολλαπλών λειτουργιών για την αποστολή μηνύματος ηλεκτρονικού ταχυδρομείου με χρήση του Office 365</span><span class="sxs-lookup"><span data-stu-id="3ccd5-102">Set up a multifunction device or application to send email using Office 365</span></span>

<span data-ttu-id="3ccd5-103">Για να μάθετε σχετικά με τις επιλογές και τα βήματα, ανατρέξτε στο θέμα [Πώς μπορείτε να ρυθμίσετε μια συσκευή ή μια εφαρμογή πολλαπλών λειτουργιών για αποστολή ηλεκτρονικού ταχυδρομείου με χρήση του Office 365](https://support.office.com/article/69f58e99-c550-4274-ad18-c805d654b4c4).</span><span class="sxs-lookup"><span data-stu-id="3ccd5-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Office 365](https://support.office.com/article/69f58e99-c550-4274-ad18-c805d654b4c4).</span></span>
  
<span data-ttu-id="3ccd5-104">**Σημείωση:** Εάν έχετε μια συσκευή ή μια εφαρμογή που σταμάτησε πρόσφατα να λειτουργεί, λάβετε υπόψη ότι έχουμε ξεκινήσει πρόσφατα την [απενεργοποίηση της κρυπτογράφησης 3DES](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption), όπως έχει προγραμματιστεί.</span><span class="sxs-lookup"><span data-stu-id="3ccd5-104">**Note:** If you have a device or application which recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="3ccd5-105">Για να δείτε τις συσκευές που επηρεάζονται μεταβείτε στο θέμα [Αναφορά προγραμμάτων-πελατών με έλεγχο ταυτότητας SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="3ccd5-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="3ccd5-106">Τα συνήθη σφάλματα θα μπορούσαν να είναι παρόμοια με: Αποτυχία/σφάλμα ελέγχου ταυτότητας, αποτυχία/σφάλμα TLS, σφάλμα αλγορίθμου κρυπτογράφησης, ασυμφωνία αλγορίθμου ή απόρριψη σύνδεσης.</span><span class="sxs-lookup"><span data-stu-id="3ccd5-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="3ccd5-107">Για να επιλύσετε το ζήτημα:</span><span class="sxs-lookup"><span data-stu-id="3ccd5-107">To resolve the issue:</span></span>
 - <span data-ttu-id="3ccd5-108">**Ο Windows Server 2003 IIS SMTP δεν θα λειτουργεί πλέον – απαιτείται μια νεότερη έκδοση των Windows.**</span><span class="sxs-lookup"><span data-stu-id="3ccd5-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="3ccd5-109">Συμβουλευτείτε τον προμηθευτή της εφαρμογής ή της συσκευής σας για να δείτε εάν υποστηρίζεται κάποια σύγχρονη κρυπτογράφηση ή αν υπάρχει ενημέρωση.</span><span class="sxs-lookup"><span data-stu-id="3ccd5-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
