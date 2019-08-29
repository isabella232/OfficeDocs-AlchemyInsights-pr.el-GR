---
title: S/MIME στο Outlook στο web
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: f2c047ca31c586c0aa36701e6e7ca9976cfd1734
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666840"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="fa622-102">Κρυπτογράφηση μηνυμάτων ηλεκτρονικού ταχυδρομείου στο Outlook</span><span class="sxs-lookup"><span data-stu-id="fa622-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="fa622-103">Κρυπτογράφηση μηνυμάτων του Office 365 είναι ενσωματωμένη στο Microsoft Azure διαχείρισης δικαιωμάτων (Azure RMS), που αποτελεί μέρος της προστασίας πληροφορίες Azure.</span><span class="sxs-lookup"><span data-stu-id="fa622-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="fa622-104">Εάν η συνδρομή σας περιλαμβάνει Διαχείριση δικαιωμάτων Azure ή Azure πληροφορίες προστασίας, **δεν χρειάζεται να προβεί σε τυχόν ενέργειες για να ενεργοποιήσετε ή να ενεργοποιήσετε με μη αυτόματο τρόπο** την υπηρεσία διαχείρισης δικαιωμάτων.</span><span class="sxs-lookup"><span data-stu-id="fa622-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="fa622-105">Με βάση τα σχόλια των πελατών, εμείς θα πλέον έχουν ενεργοποιημένες κανόνων ροής αλληλογραφίας Exchange για την αυτόματη κρυπτογράφηση εξερχόμενου ηλεκτρονικού ταχυδρομείου που περιέχει συγκεκριμένο τύπο ευαίσθητων πληροφοριών σας μισθωτών από προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="fa622-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="fa622-106">Αντί για αυτό, παρέχουμε λεπτομερείς οδηγίες για το πώς μπορείτε να το κάνετε μόνοι σας.</span><span class="sxs-lookup"><span data-stu-id="fa622-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="fa622-107">Για πρόσθετες πληροφορίες σχετικά με τον τρόπο για να δημιουργήσετε έναν κανόνα μεταφοράς για να κρυπτογραφήσετε ευαίσθητες πληροφορίες, ανατρέξτε στην ενότητα [αυτού του άρθρου](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="fa622-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="fa622-108">Εάν χρησιμοποιείτε το Outlook στο Web (παλαιότερα **OWA**): κατά τη σύνθεση ενός μηνύματος ηλεκτρονικού ταχυδρομείου, κάντε απλώς κλικ **προστασία** στο OWA.</span><span class="sxs-lookup"><span data-stu-id="fa622-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="fa622-109">Αυτό θα ισχύει το δικαίωμα "Να μη γίνει προώθηση".</span><span class="sxs-lookup"><span data-stu-id="fa622-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="fa622-110">Κάντε κλικ στην επιλογή **Αλλαγή δικαιωμάτων** και επιλέξτε **κρυπτογράφηση** για να κρυπτογραφήσετε μόνο το μήνυμα.</span><span class="sxs-lookup"><span data-stu-id="fa622-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="fa622-111">Εάν χρησιμοποιείτε το **πρόγραμμα-πελάτης Outlook**: για να στείλετε ένα κρυπτογραφημένο μήνυμα από το Outlook 2013 ή 2016 ή Outlook 2016 για Mac, επιλέξτε **Επιλογές** > **δικαιώματα**και στη συνέχεια επιλέξτε την επιλογή προστασίας που χρειάζεστε.</span><span class="sxs-lookup"><span data-stu-id="fa622-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="fa622-112">Για την **αυτόματη κρυπτογράφηση όλων ηλεκτρονικού ταχυδρομείου** αποστέλλονται σε ορισμένους παραλήπτες ή εξωτερικών συνεργατών οργανισμών, πρέπει να δημιουργήσετε έναν κανόνα μεταφοράς ροή αλληλογραφίας στο στο Κέντρο διαχείρισης του Exchange.</span><span class="sxs-lookup"><span data-stu-id="fa622-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="fa622-113">Λεπτομερείς οδηγίες που παρέχονται σε [αυτό το άρθρο υποστήριξης](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="fa622-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

