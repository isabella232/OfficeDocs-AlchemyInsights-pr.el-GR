---
title: 1554 Σφάλμα Winsock 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766169"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="8c3dd-102">Σφάλμα Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="8c3dd-102">Winsock error 10061</span></span>

<span data-ttu-id="8c3dd-103">Αυτός ο κωδικός σφάλματος σημαίνει ότι η Microsoft δεν ήταν δυνατή η δημιουργία μιας υποδοχής TCP (σύνδεση) με τον κεντρικό υπολογιστή προορισμού.</span><span class="sxs-lookup"><span data-stu-id="8c3dd-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="8c3dd-104">Η πιο πιθανή αιτία αυτού του σφάλματος είναι ένα πρόβλημα με τις παραμέτρους του τείχους προστασίας.</span><span class="sxs-lookup"><span data-stu-id="8c3dd-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="8c3dd-105">Για να διορθώσετε το πρόβλημα, ελέγξτε αυτές τις ρυθμίσεις:</span><span class="sxs-lookup"><span data-stu-id="8c3dd-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="8c3dd-106">Επαληθεύστε τις παραμέτρους του τείχους προστασίας σας με τις πληροφορίες στις [διευθύνσεις URL και τις περιοχές διευθύνσεων IP της Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="8c3dd-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="8c3dd-107">Εάν το σφάλμα αφορά συγκεκριμένα την Ηλεκτρονική προστασία του Exchange (EOP), θα πρέπει να έχετε ειδοποιηθεί προηγουμένως για αλλαγή στις [διευθύνσεις IP ηλεκτρονικής προστασίας του Exchange](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="8c3dd-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="8c3dd-108">Βεβαιωθείτε ότι η υπηρεσία παροχής Internet (ISP) δεν αποκλείει τη θύρα.</span><span class="sxs-lookup"><span data-stu-id="8c3dd-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="8c3dd-109">Επαληθεύστε τις ρυθμίσεις του έξυπνου κεντρικού υπολογιστή και του διακομιστή προορισμού στις συνδέσεις σας.</span><span class="sxs-lookup"><span data-stu-id="8c3dd-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="8c3dd-110">Σημειώστε ότι το Microsoft 365 δεν αποκλείει *τις εισερχόμενες* συνδέσεις με αυτόν τον τρόπο.</span><span class="sxs-lookup"><span data-stu-id="8c3dd-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
