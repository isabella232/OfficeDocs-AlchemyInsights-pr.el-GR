---
title: S/MIME στο Outlook στο Web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772262"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="330a4-102">Κρυπτογράφηση μηνυμάτων ηλεκτρονικού ταχυδρομείου στο Outlook</span><span class="sxs-lookup"><span data-stu-id="330a4-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="330a4-103">Η κρυπτογράφηση μηνυμάτων του Microsoft 365 είναι ενσωματωμένη στη διαχείριση δικαιωμάτων Microsoft Azure (Azure RMS), η οποία αποτελεί μέρος της προστασίας πληροφοριών του Azure.</span><span class="sxs-lookup"><span data-stu-id="330a4-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="330a4-104">Εάν η συνδρομή σας περιλαμβάνει τη διαχείριση δικαιωμάτων Azure ή την προστασία πληροφοριών Azure, **δεν χρειάζεται να κάνετε ενέργειες για να ενεργοποιήσετε ή να ενεργοποιήσετε με μη αυτόματο τρόπο** την υπηρεσία διαχείρισης δικαιωμάτων.</span><span class="sxs-lookup"><span data-stu-id="330a4-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="330a4-105">Με βάση τα σχόλια των πελατών, δεν θα είναι πλέον δυνατή η ενεργοποίηση των κανόνων ροής αλληλογραφίας του Exchange για την αυτόματη κρυπτογράφηση εξερχόμενου ηλεκτρονικού ταχυδρομείου που περιέχει συγκεκριμένο τύπο ευαίσθητων πληροφοριών στον μισθωτή σας από προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="330a4-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="330a4-106">Αντ ' αυτού, παρέχουμε αναλυτικές οδηγίες σχετικά με το πώς μπορείτε να το κάνετε μόνοι σας.</span><span class="sxs-lookup"><span data-stu-id="330a4-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="330a4-107">Για περισσότερες λεπτομέρειες σχετικά με τον τρόπο δημιουργίας ενός κανόνα μεταφοράς για την κρυπτογράφηση ευαίσθητων πληροφοριών, ανατρέξτε σε [αυτό το άρθρο](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="330a4-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="330a4-108">Εάν χρησιμοποιείτε το Outlook στο Web (πρώην **OWA**): κατά τη σύνταξη ενός μηνύματος ηλεκτρονικού ταχυδρομείου, απλώς κάντε κλικ στην επιλογή **προστασία** στο OWA.</span><span class="sxs-lookup"><span data-stu-id="330a4-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="330a4-109">Αυτό θα εφαρμόσει το δικαίωμα "χωρίς προώθηση".</span><span class="sxs-lookup"><span data-stu-id="330a4-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="330a4-110">Κάντε κλικ στην επιλογή **Αλλαγή δικαιώματος** και επιλέξτε **κρυπτογράφηση** για να κρυπτογραφήσετε μόνο το μήνυμα.</span><span class="sxs-lookup"><span data-stu-id="330a4-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="330a4-111">Εάν χρησιμοποιείτε το **πρόγραμμα-πελάτη του Outlook**: για να στείλετε ένα κρυπτογραφημένο μήνυμα από το Outlook 2013 ή το 2016 ή το Outlook 2016 για Mac, επιλέξτε **Options**  >  **δικαιώματα**επιλογών και, στη συνέχεια, επιλέξτε την επιλογή προστασίας που χρειάζεστε.</span><span class="sxs-lookup"><span data-stu-id="330a4-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="330a4-112">Για να **κρυπτογραφήσετε αυτόματα όλα τα μηνύματα ηλεκτρονικού ταχυδρομείου** που αποστέλλονται σε συγκεκριμένους παραλήπτες ή εξωτερικούς οργανισμούς συνεργατών, πρέπει να δημιουργήσετε έναν κανόνα μεταφοράς ροής αλληλογραφίας στο κέντρο διαχείρισης του Exchange.</span><span class="sxs-lookup"><span data-stu-id="330a4-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="330a4-113">Αναλυτικές οδηγίες παρέχονται σε [αυτό το άρθρο υποστήριξης](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="330a4-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

