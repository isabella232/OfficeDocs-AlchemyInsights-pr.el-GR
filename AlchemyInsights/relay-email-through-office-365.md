---
title: Μεταγωγή ηλεκτρονικού ταχυδρομείου μέσω του Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117983"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="b150c-102">Ρύθμιση μιας συσκευής ή μιας εφαρμογής πολλαπλών λειτουργιών για την αποστολή μηνύματος ηλεκτρονικού ταχυδρομείου</span><span class="sxs-lookup"><span data-stu-id="b150c-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="b150c-103">Για να μάθετε σχετικά με τις επιλογές και τα βήματα, ανατρέξτε στο θέμα [Πώς μπορείτε να ρυθμίσετε μια συσκευή ή μια εφαρμογή πολλαπλών λειτουργιών για αποστολή ηλεκτρονικού ταχυδρομείου με χρήση του Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="b150c-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="b150c-104">Εάν έχετε μια συσκευή ή εφαρμογή που σταμάτησε να λειτουργεί πρόσφατα, τα πιο συνηθισμένα προβλήματα είναι τα εξής:</span><span class="sxs-lookup"><span data-stu-id="b150c-104">If you have a device or application that recently stopped working, the most common issues are:</span></span>

- <span data-ttu-id="b150c-105">**Σφάλματα που σχετίζονται με τον έλεγχο ταυτότητας κατά τη χρήση της υποβολής προγράμματος-πελάτη SMTP Auth** Πρόσφατα κάναμε ορισμένες αλλαγές που σχετίζονται με τον τρόπο με τον οποίο λειτουργεί ο έλεγχος ταυτότητας SMTP.</span><span class="sxs-lookup"><span data-stu-id="b150c-105">**Authentication related errors while using SMTP Auth client submission** We recently made some changes related to how SMTP Authentication works.</span></span> <span data-ttu-id="b150c-106">Για περισσότερες πληροφορίες σχετικά με τον τρόπο επίλυσης προβλημάτων, ανατρέξτε στην ενότητα ανεπιτυχούς ελέγχου ταυτότητας της ενότητας "Επιδιόρθωση προβλημάτων με εκτυπωτές, σαρωτές και [εφαρμογές LOB"](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)που στέλνουν μηνύματα ηλεκτρονικού ταχυδρομείου χρησιμοποιώντας Microsoft 365 ή Office 365.</span><span class="sxs-lookup"><span data-stu-id="b150c-106">For more information about how to resolve issues, see the authentication unsuccessful section of [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span></span>
- <span data-ttu-id="b150c-107">**Δεχόμαστε μόνο την έκδοση TLS 1.2 κατά τη δημιουργία ασφαλούς σύνδεσης με Office 365** Εάν χρησιμοποιείτε ασφαλή σύνδεση (TLS), βεβαιωθείτε ότι η συσκευή εφαρμογής σας υποστηρίζει TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="b150c-107">**We accept only the TLS 1.2 version while making a secure connection to Office 365** If you're using Secure connection (TLS), make sure your application device supports TLS 1.2.</span></span> <span data-ttu-id="b150c-108">Για περισσότερες πληροφορίες, [ανατρέξτε στο θέμα Προετοιμασία για TLS 1.2 σε Office 365 και Office 365 GCC.](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="b150c-108">For more information, see [Preparing for TLS 1.2 in Office 365 and Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span></span>
 
<span data-ttu-id="b150c-109">Για άλλα προβλήματα και λύσεις, ανατρέξτε στο θέμα Επιδιόρθωση προβλημάτων με εκτυπωτές, σαρωτές και εφαρμογές LOB που στέλνουν [μηνύματα ηλεκτρονικού ταχυδρομείου χρησιμοποιώντας Microsoft 365 ή Office 365.](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)</span><span class="sxs-lookup"><span data-stu-id="b150c-109">For other issues and solutions, see [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span></span>

<span data-ttu-id="b150c-110">Για να δείτε τις συσκευές που επηρεάζονται μεταβείτε στο θέμα [Αναφορά προγραμμάτων-πελατών με έλεγχο ταυτότητας SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="b150c-110">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span>

<span data-ttu-id="b150c-111">**Σημείωση:** Exchange Online δεν χωρούν σενάρια μαζικής αλληλογραφίας.</span><span class="sxs-lookup"><span data-stu-id="b150c-111">**Note**: Exchange Online doesn't accommodate bulk-mailing scenarios.</span></span> <span data-ttu-id="b150c-112">Για να στείλετε μαζικά εμπορικά μηνύματα ηλεκτρονικού ταχυδρομείου (για παράδειγμα, ενημερωτικά δελτία πελατών), θα πρέπει να χρησιμοποιήσετε υπηρεσίες παροχής τρίτων που ειδικεύονται σε αυτές τις υπηρεσίες.</span><span class="sxs-lookup"><span data-stu-id="b150c-112">To send bulk commercial email (for example, customer newsletters), you should use third-party providers that specialize in these services.</span></span>
