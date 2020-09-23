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
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219855"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="e1667-102">Αποκλεισμός ή κατάργηση αποκλεισμού προώθησης ηλεκτρονικού ταχυδρομείου</span><span class="sxs-lookup"><span data-stu-id="e1667-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="e1667-103">Για να ενεργοποιήσετε ή να απενεργοποιήσετε την προώθηση μηνυμάτων ηλεκτρονικού ταχυδρομείου για ένα συγκεκριμένο γραμματοκιβώτιο, ανατρέξτε στο θέμα [Ρύθμιση παραμέτρων προώθησης ηλεκτρονικού ταχυδρομείου](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="e1667-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="e1667-104">Στο επίπεδο μισθωτών, ο έλεγχος της εξωτερικής προώθησης γίνεται με χρήση της πολιτικής "εξερχόμενη ανεπιθύμητη αλληλογραφία".</span><span class="sxs-lookup"><span data-stu-id="e1667-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="e1667-105">Εάν έχει τεθεί σε απενεργοποιημένη ή αυτόματη, ενδέχεται να αποκλείσει την προώθηση μηνυμάτων ηλεκτρονικού ταχυδρομείου με την "550 5.7.520 δεν επιτρέπεται η πρόσβαση, η εταιρεία σας δεν επιτρέπει την εξωτερική προώθηση" σφάλμα.</span><span class="sxs-lookup"><span data-stu-id="e1667-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="e1667-106">Στη συνέχεια, εάν η προώθηση έχει καθοριστεί ώστε να είναι αποκλεισμένη, αυτό είναι το σφάλμα που θα βλέπουν οι χρήστες σας.</span><span class="sxs-lookup"><span data-stu-id="e1667-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="e1667-107">Εάν η προώθηση έχει αποκλειστεί, βεβαιωθείτε ότι η πολιτική έχει ρυθμιστεί για να ενεργοποιήσετε την εξωτερική προώθηση.</span><span class="sxs-lookup"><span data-stu-id="e1667-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="e1667-108">Μπορείτε να επιλέξετε την πολιτική φιλτραρίσματος ανεπιθύμητης αλληλογραφίας από το κέντρο ασφάλειας και συμμόρφωσης ή εκτελώντας την εντολή Get-HostedOutboundSpamFilterPolicy | όνομα FL, AutoForwardingMode.</span><span class="sxs-lookup"><span data-stu-id="e1667-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="e1667-109">Εάν θέλετε να ρυθμίσετε τον αποκλεισμό της "αυτοπροώθησης", η ίδια εντολή θα σας ενημερώσει για την κατάσταση της πολιτικής τώρα.</span><span class="sxs-lookup"><span data-stu-id="e1667-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="e1667-110">Σημείωση: συνιστάται να διατηρήσετε την εξωτερική προώθηση απενεργοποιημένη στην προεπιλεγμένη πολιτική φίλτρου εξερχομένων ανεπιθύμητης αλληλογραφίας και να την ενεργοποιήσετε μόνο για τους χρήστες που χρειάζονται εξωτερική προώθηση, δημιουργώντας μια προσαρμοσμένη πολιτική για αυτούς τους χρήστες.</span><span class="sxs-lookup"><span data-stu-id="e1667-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="e1667-111">Μπορείτε να διαβάσετε περισσότερα στη [Ρύθμιση παραμέτρων εξωτερικής προώθησης ηλεκτρονικού ταχυδρομείου στο Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="e1667-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>