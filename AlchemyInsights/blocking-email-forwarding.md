---
title: 726 αποκλεισμός προώθησης ηλεκτρονικού ταχυδρομείου
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478344"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="8d5fa-102">Αποκλεισμός ή κατάργηση αποκλεισμού προώθησης ηλεκτρονικού ταχυδρομείου</span><span class="sxs-lookup"><span data-stu-id="8d5fa-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="8d5fa-103">Για να ενεργοποιήσετε ή να απενεργοποιήσετε την προώθηση μηνυμάτων ηλεκτρονικού ταχυδρομείου για ένα συγκεκριμένο γραμματοκιβώτιο, ανατρέξτε στο θέμα [Ρύθμιση παραμέτρων προώθησης ηλεκτρονικού ταχυδρομείου](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="8d5fa-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="8d5fa-104">Στο επίπεδο μισθωτών, ο έλεγχος της εξωτερικής προώθησης γίνεται με χρήση της πολιτικής ανεπιθύμητης αλληλογραφίας εξερχομένων.</span><span class="sxs-lookup"><span data-stu-id="8d5fa-104">On the tenant level, control of external forwarding is done using the outbound spam policy.</span></span> <span data-ttu-id="8d5fa-105">Μπορείτε να επιλέξετε την πολιτική φιλτραρίσματος ανεπιθύμητης αλληλογραφίας από το κέντρο ασφάλειας και συμμόρφωσης [εδώ](https://protection.office.com/antispam) ή χρησιμοποιώντας την [εντολή Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span><span class="sxs-lookup"><span data-stu-id="8d5fa-105">You can check the outbound spam filter policy from Security and Compliance Center [here](https://protection.office.com/antispam) or by using the [Get-HostedOutboundSpamFilterPolicy command](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span></span>

<span data-ttu-id="8d5fa-106">Εάν λαμβάνετε το ακόλουθο μήνυμα σφάλματος: **"δεν επιτρέπεται η πρόσβαση του 550 5.7.520, η εταιρεία σας δεν επιτρέπει την εξωτερική προώθηση"**, βεβαιωθείτε ότι η πολιτική έχει ρυθμιστεί ώστε να ενεργοποιεί την εξωτερική αυτόματη προώθηση.</span><span class="sxs-lookup"><span data-stu-id="8d5fa-106">If you are getting the following error: **“550 5.7.520 Access denied, Your organization does not allow external forwarding”**, please make sure the policy is configured to enable External Auto-forward.</span></span>

<span data-ttu-id="8d5fa-107">**Σημείωση:** Συνιστάται να διατηρήσετε την εξωτερική προώθηση απενεργοποιημένη στην προεπιλεγμένη πολιτική φίλτρου ανεπιθύμητης αλληλογραφίας και να την ενεργοποιήσετε μόνο για τους χρήστες που χρειάζονται εξωτερική προώθηση με τη δημιουργία μιας προσαρμοσμένης πολιτικής για αυτούς τους χρήστες.</span><span class="sxs-lookup"><span data-stu-id="8d5fa-107">**Note:** It is recommended to keep the External Autoforward disabled on your default outbound spam filter policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="8d5fa-108">Μπορείτε να διαβάσετε περισσότερα στη [Ρύθμιση παραμέτρων εξωτερικής προώθησης ηλεκτρονικού ταχυδρομείου στο Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="8d5fa-108">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>