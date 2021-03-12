---
title: Δεν είναι δυνατή η αποστολή/λήψη ηλεκτρονικού ταχυδρομείου από/προς το Office 365 λόγω της απενεργοποίησης TLS 1.0 και TLS 1.1
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745018"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="f64c1-102">Δεν είναι δυνατή η αποστολή/λήψη ηλεκτρονικού ταχυδρομείου από/προς το Office 365 λόγω της απενεργοποίησης TLS 1.0 και TLS 1.1</span><span class="sxs-lookup"><span data-stu-id="f64c1-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="f64c1-103">Όπως επιβεβαιώθηκε από τη δημοσίευση mc229914 του κέντρου μηνυμάτων, η απόσβεση TLS 1.0 και TLS 1.1 ξεκίνησε την επιβολή για τελικά σημεία ροής αλληλογραφίας του Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="f64c1-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="f64c1-104">Σύντομα το Office 365 δεν θα δέχεται πλέον συνδέσεις ηλεκτρονικού ταχυδρομείου TLS 1.0 και TLS 1.1 από εξωτερικές προελεύσεις.</span><span class="sxs-lookup"><span data-stu-id="f64c1-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="f64c1-105">Επίσης, το Exchange Online δεν θα χρησιμοποιεί ποτέ TLS 1.0 ή 1.1 για την αποστολή εξερχόμενων μηνυμάτων ηλεκτρονικού ταχυδρομείου.</span><span class="sxs-lookup"><span data-stu-id="f64c1-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="f64c1-106">Εάν αντιμετωπίζετε προβλήματα λόγω απενεργοποίησης TLS 1.0 ή 1.1, ενδέχεται να αντιμετωπίσετε ένα από τα ακόλουθα σφάλματα.</span><span class="sxs-lookup"><span data-stu-id="f64c1-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="f64c1-107">Ο αποστολέας επιστρέφει την επιστροφή NDR - "421 4.4.2 Η σύνδεση απορρίφθηκε λόγω SocketError"</span><span class="sxs-lookup"><span data-stu-id="f64c1-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="f64c1-108">Σφάλμα στο πρόγραμμα προβολής ουράς του διακομιστή εσωτερικής εγκατάστασης που στέλνει μηνύματα ηλεκτρονικού ταχυδρομείου στον Υπεύθυνο 365- '421 4.4.2 Η σύνδεση απορρίφθηκε λόγω SocketError'</span><span class="sxs-lookup"><span data-stu-id="f64c1-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="f64c1-109">Σφάλμα στο αρχείο καταγραφής "Αποστολή πρωτοκόλλου [σύνδεσης"](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) στο διακομιστή που στέλνει μηνύματα ηλεκτρονικού ταχυδρομείου στο Office 365- Η διαπραγμάτευση TLS απέτυχε με σφάλμα SocketError</span><span class="sxs-lookup"><span data-stu-id="f64c1-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="f64c1-110">Σφάλμα στο αρχείο καταγραφής πρωτοκόλλου αποστολής ή λήψης σύνδεσης - "451 5.7.3 Πρέπει πρώτα να εκδώσει μια εντολή STARTTLS"</span><span class="sxs-lookup"><span data-stu-id="f64c1-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="f64c1-111">Εάν αντιμετωπίσετε οποιοδήποτε από τα παραπάνω σφάλματα, βεβαιωθείτε ότι ο διακομιστής που στέλνει ή λαμβάνει μηνύματα ηλεκτρονικού ταχυδρομείου έχει ενεργοποιημένο το TLS 1.2, ελέγχοντας τα ακόλουθα κλειδιά μητρώου.</span><span class="sxs-lookup"><span data-stu-id="f64c1-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="f64c1-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2\Πρόγραμμα-πελάτης] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span><span class="sxs-lookup"><span data-stu-id="f64c1-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="f64c1-113">Εάν κάνετε οποιαδήποτε αλλαγή στα παραπάνω κλειδιά μητρώου για να ενεργοποιήσετε το TLS 1.2, επανεκκινήστε το διακομιστή για να εφαρμοστούν οι αλλαγές.</span><span class="sxs-lookup"><span data-stu-id="f64c1-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="f64c1-114">Επίσης, βεβαιωθείτε ότι έχετε εγκαταστήσει τις πιο πρόσφατες ενημερώσεις των Windows και του Exchange.</span><span class="sxs-lookup"><span data-stu-id="f64c1-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="f64c1-115">Για περισσότερες πληροφορίες, ανατρέξτε στα θέματα:</span><span class="sxs-lookup"><span data-stu-id="f64c1-115">For more information, see:</span></span>

- [<span data-ttu-id="f64c1-116">Οδηγίες TLS του Exchange Server, μέρος 1: Ετοιμάζομαι για το TLS 1.2 - Κοινότητα τεχνικής υποστήριξης της Microsoft</span><span class="sxs-lookup"><span data-stu-id="f64c1-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="f64c1-117">Τμήμα καθοδήγησης TLS του Exchange Server 2: Ενεργοποίηση του TLS 1.2 και προσδιορισμός των πελατών που δεν το χρησιμοποιούν - Κοινότητα τεχνικής υποστήριξης της Microsoft</span><span class="sxs-lookup"><span data-stu-id="f64c1-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="f64c1-118">Κατανόηση των σεναρίων ηλεκτρονικού ταχυδρομείου εάν δεν είναι δυνατή η συμφωνία εκδόσεων TLS με το Exchange Online - Κοινότητα τεχνικής υποστήριξης της Microsoft</span><span class="sxs-lookup"><span data-stu-id="f64c1-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
