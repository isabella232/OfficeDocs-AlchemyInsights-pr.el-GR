---
title: Χώρος συγκέντρωσης εξερχομένων αναμετάδοσης
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381714"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="070d1-102">Χώρος συγκέντρωσης εξερχομένων αναμετάδοσης</span><span class="sxs-lookup"><span data-stu-id="070d1-102">Outbound relay pool</span></span>

<span data-ttu-id="070d1-103">Η Microsoft κάνει ορισμένες αλλαγές στη ρύθμιση παραμέτρων για την αναμετάδοση ή την προώθηση μηνυμάτων ηλεκτρονικού ταχυδρομείου μέσω Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="070d1-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="070d1-104">Τα μηνύματα σε ορισμένα σενάρια προωθώνται ή μεταδίδονται μέσω Microsoft 365 χρήση ενός ειδικού χώρου συγκέντρωσης αναμετάδοσης.</span><span class="sxs-lookup"><span data-stu-id="070d1-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="070d1-105">Τα μηνύματα που αποστέλλονται χρησιμοποιώντας το χώρο συγκέντρωσης αναμετάδοσης μπορεί να καταλήγουν στο φάκελο ανεπιθύμητης αλληλογραφίας του παραλήπτη.</span><span class="sxs-lookup"><span data-stu-id="070d1-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="070d1-106">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Χώρους συγκέντρωσης παράδοσης εξερχομένων](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="070d1-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="070d1-107">Για να αποφύγετε ένα σενάριο που χρησιμοποιεί το χώρο συγκέντρωσης αναμετάδοσης, βεβαιωθείτε ότι τα μηνύματα προώθησης/αναμετάδοσης πληρούν ένα από τα ακόλουθα κριτήρια:</span><span class="sxs-lookup"><span data-stu-id="070d1-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="070d1-108">Ο εξερχόμενος αποστολέας είναι ένας αποδεκτός τομέας του μισθωτή.</span><span class="sxs-lookup"><span data-stu-id="070d1-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="070d1-109">Το Πλαίσιο πολιτικής αποστολέα (SPF) περνά όταν το μήνυμα έρχεται Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="070d1-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="070d1-110">Το DomainKeys Identified Mail (DKIM) στον τομέα αποστολέα P2 περνά όταν το μήνυμα έρχεται Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="070d1-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="070d1-111">Τα μηνύματα που πληρούν τα παραπάνω κριτήρια δεν μεταδίδονται μέσω του χώρου συγκέντρωσης αναμετάδοσης.</span><span class="sxs-lookup"><span data-stu-id="070d1-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="070d1-112">Εάν η εγγραφή MX για τον τομέα σας επισημαίνεται σε διακομιστή άλλου κατασκευαστή ή εσωτερικής εγκατάστασης, χρησιμοποιήστε βελτιωμένο φιλτράρισμα για να βεβαιωθείτε ότι η επικύρωση SPF είναι σωστή για το εισερχόμενο ηλεκτρονικό ταχυδρομείο και για να αποφύγετε την αποστολή μηνυμάτων ηλεκτρονικού ταχυδρομείου μέσω του χώρου συγκέντρωσης αναμετάδοσης.</span><span class="sxs-lookup"><span data-stu-id="070d1-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="070d1-113">**Πώς μπορούμε να δούμε εάν μας επηρεάζει το χώρο συγκέντρωσης αναμετάδοσης;**</span><span class="sxs-lookup"><span data-stu-id="070d1-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="070d1-114">Εάν τα μηνύματα ηλεκτρονικού ταχυδρομείου που προωθήθηκε ή μεταβιβάσατε χρησιμοποιούν ένα από τα παραπάνω κριτήρια, τα μηνύματα δεν θα μεταδίδονται μέσω του χώρου συγκέντρωσης αναμετάδοσης.</span><span class="sxs-lookup"><span data-stu-id="070d1-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="070d1-115">Ωστόσο, εάν ένα μήνυμα σταλεί μέσω ενός χώρου συγκέντρωσης αναμετάδοσης, η διεύθυνση IP του διακομιστή εξερχομένων βρίσκεται στην περιοχή 40.95.0.0/16 και το όνομα του διακομιστή εξερχομένων **περιλαμβάνει το όνομα** του διακομιστή εξερχομένων.</span><span class="sxs-lookup"><span data-stu-id="070d1-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

