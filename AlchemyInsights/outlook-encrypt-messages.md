---
title: S/MIME στο Outlook στο web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511508"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="7f217-102">Κρυπτογράφηση μηνυμάτων ηλεκτρονικού ταχυδρομείου στο Outlook</span><span class="sxs-lookup"><span data-stu-id="7f217-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="7f217-103">Η κρυπτογράφηση μηνυμάτων Microsoft 365 είναι ενσωματωμένη στη Διαχείριση δικαιωμάτων Microsoft Azure (Azure RMS), η οποία αποτελεί μέρος της Προστασίας Πληροφοριών Azure.</span><span class="sxs-lookup"><span data-stu-id="7f217-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="7f217-104">Εάν η συνδρομή σας περιλαμβάνει τη Διαχείριση δικαιωμάτων Azure ή την Προστασία πληροφοριών Azure, **δεν χρειάζεται να προβείτε σε ενέργειες για να ενεργοποιήσετε ή να ενεργοποιήσετε με μη αυτόματο τρόπο** την Υπηρεσία διαχείρισης δικαιωμάτων.</span><span class="sxs-lookup"><span data-stu-id="7f217-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="7f217-105">Με βάση τα σχόλια των πελατών, δεν θα επιτρέπουμε πλέον στους κανόνες ροής αλληλογραφίας του Exchange να κρυπτογραφούν αυτόματα εξερχόμενα μηνύματα ηλεκτρονικού ταχυδρομείου που περιέχουν συγκεκριμένο τύπο ευαίσθητων πληροφοριών στον μισθωτή σας από προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="7f217-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="7f217-106">Αντ 'αυτού, παρέχουμε λεπτομερείς οδηγίες για το πώς μπορείτε να το κάνετε μόνοι σας.</span><span class="sxs-lookup"><span data-stu-id="7f217-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="7f217-107">Για πρόσθετες λεπτομέρειες σχετικά με τον τρόπο δημιουργίας ενός κανόνα μεταφοράς για την κρυπτογράφηση ευαίσθητων πληροφοριών, ανατρέξτε [σε αυτό το άρθρο](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="7f217-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="7f217-108">Εάν χρησιμοποιείτε το Outlook στο Web (πρώην **OWA):** Όταν συνθέτετε ένα μήνυμα ηλεκτρονικού ταχυδρομείου, απλώς κάντε κλικ στην επιλογή **Προστασία** σε OWA.</span><span class="sxs-lookup"><span data-stu-id="7f217-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="7f217-109">Αυτό θα εφαρμόσει το δικαίωμα "Χωρίς προώθηση".</span><span class="sxs-lookup"><span data-stu-id="7f217-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="7f217-110">Κάντε κλικ στην επιλογή **Αλλαγή δικαιώματος** και **επιλέξτε Κρυπτογράφηση** για να κρυπτογραφήσετε μόνο το μήνυμα.</span><span class="sxs-lookup"><span data-stu-id="7f217-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="7f217-111">Εάν χρησιμοποιείτε **το πρόγραμμα-πελάτη του Outlook**: Για να στείλετε ένα κρυπτογραφημένο μήνυμα από το Outlook 2013 ή το 2016 ή το Outlook 2016 για Mac, επιλέξτε **Δικαιώματα**  >  **επιλογών**και, στη συνέχεια, ενεργοποιήστε την επιλογή προστασίας που χρειάζεστε.</span><span class="sxs-lookup"><span data-stu-id="7f217-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="7f217-112">Για να **κρυπτογραφήσετε αυτόματα όλα τα μηνύματα ηλεκτρονικού ταχυδρομείου** που αποστέλλονται σε συγκεκριμένους παραλήπτες ή εξωτερικούς οργανισμούς συνεργατών, πρέπει να δημιουργήσετε έναν κανόνα μεταφοράς ροής αλληλογραφίας στο Κέντρο διαχείρισης του Exchange.</span><span class="sxs-lookup"><span data-stu-id="7f217-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="7f217-113">Λεπτομερείς οδηγίες παρέχονται σε [αυτό το άρθρο υποστήριξης](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="7f217-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

