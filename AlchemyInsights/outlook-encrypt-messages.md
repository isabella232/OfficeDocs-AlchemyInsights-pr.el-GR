---
title: S/MIME στο Outlook στο Web
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6915470655b85922f6f97e8ca6fac353224b1ae0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752860"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="3da58-102">Κρυπτογράφηση μηνυμάτων ηλεκτρονικού ταχυδρομείου στο Outlook</span><span class="sxs-lookup"><span data-stu-id="3da58-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="3da58-103">Η κρυπτογράφηση μηνυμάτων Office 365 είναι ενσωματωμένη στη διαχείριση δικαιωμάτων Azure της Microsoft (Azure RMS), η οποία αποτελεί μέρος της προστασίας πληροφοριών Azure.</span><span class="sxs-lookup"><span data-stu-id="3da58-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="3da58-104">Εάν η συνδρομή σας περιλαμβάνει διαχείριση δικαιωμάτων Azure ή προστασία πληροφοριών Azure, **δεν χρειάζεται να κάνετε ενέργειες για να ενεργοποιήσετε ή να ενεργοποιήσετε με μη αυτόματο τρόπο** την υπηρεσία διαχείρισης δικαιωμάτων.</span><span class="sxs-lookup"><span data-stu-id="3da58-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="3da58-105">Βάσει των σχολίων των πελατών, δεν θα μπορούμε πλέον να ενεργοποιήσετε τους κανόνες ροής αλληλογραφίας του Exchange για την αυτόματη κρυπτογράφηση εξερχόμενων μηνυμάτων ηλεκτρονικού ταχυδρομείου που περιέχουν συγκεκριμένο τύπο ευαίσθητων πληροφοριών στον μισθωτή σας από προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="3da58-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="3da58-106">Αντ ' αυτού, παρέχουμε λεπτομερείς οδηγίες για το πώς μπορείτε να το κάνετε αυτό μόνοι σας.</span><span class="sxs-lookup"><span data-stu-id="3da58-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="3da58-107">Για πρόσθετες λεπτομέρειες σχετικά με τον τρόπο δημιουργίας ενός κανόνα μεταφοράς για την κρυπτογράφηση ευαίσθητων πληροφοριών, ανατρέξτε σε [αυτό το άρθρο](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="3da58-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="3da58-108">Εάν χρησιμοποιείτε το Outlook στο Web (πρώην **OWA**): κατά τη σύνταξη ενός μηνύματος ηλεκτρονικού ταχυδρομείου, απλά κάντε κλικ στο κουμπί **προστασία** στο OWA.</span><span class="sxs-lookup"><span data-stu-id="3da58-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="3da58-109">Αυτό θα εφαρμόσει την άδεια "χωρίς προώθηση".</span><span class="sxs-lookup"><span data-stu-id="3da58-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="3da58-110">Κάντε κλικ στην επιλογή **Αλλαγή δικαιωμάτων** και επιλέξτε **κρυπτογράφηση** για να κρυπτογραφήσετε μόνο το μήνυμα.</span><span class="sxs-lookup"><span data-stu-id="3da58-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="3da58-111">Εάν χρησιμοποιείτε το **πρόγραμμα-πελάτη του Outlook**: για να στείλετε ένα κρυπτογραφημένο μήνυμα από το Outlook 2013 ή 2016 ή το Outlook 2016 για Mac, επιλέξτε**δικαιώματα** **επιλογών** > και, στη συνέχεια, επιλέξτε την επιλογή προστασίας που χρειάζεστε.</span><span class="sxs-lookup"><span data-stu-id="3da58-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="3da58-112">Για την **αυτόματη κρυπτογράφηση όλων των μηνυμάτων ηλεκτρονικού ταχυδρομείου** που αποστέλλονται σε συγκεκριμένους παραλήπτες ή εξωτερικούς οργανισμούς συνεργατών, πρέπει να δημιουργήσετε έναν κανόνα μεταφοράς αλληλογραφίας στο κέντρο διαχείρισης Exchange.</span><span class="sxs-lookup"><span data-stu-id="3da58-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="3da58-113">Λεπτομερείς οδηγίες παρέχονται σε [αυτό το άρθρο υποστήριξης](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="3da58-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

