---
title: σφάλμα 1554 Winsock 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698862"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="db80d-102">Σφάλμα Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="db80d-102">Winsock error 10061</span></span>

<span data-ttu-id="db80d-103">Αυτός ο κωδικός σφάλματος σημαίνει ότι η Microsoft δεν μπόρεσε να δημιουργήσει μια υποδοχή TCP (σύνδεση) με τον κεντρικό υπολογιστή προορισμού.</span><span class="sxs-lookup"><span data-stu-id="db80d-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="db80d-104">Η πιο πιθανή αιτία αυτού του σφάλματος είναι ένα πρόβλημα με τη ρύθμιση παραμέτρων του τείχους προστασίας σας.</span><span class="sxs-lookup"><span data-stu-id="db80d-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="db80d-105">Για να διορθώσετε το πρόβλημα, ανατρέξτε σε αυτές τις ρυθμίσεις:</span><span class="sxs-lookup"><span data-stu-id="db80d-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="db80d-106">Επαληθεύστε τη ρύθμιση παραμέτρων του τείχους προστασίας σας με τις πληροφορίες στις [διευθύνσεις URL και τις περιοχές διευθύνσεων IP του Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="db80d-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="db80d-107">Εάν το σφάλμα αφορά συγκεκριμένα την προστασία του Exchange Online (EOP), θα έπρεπε να έχετε προηγουμένως ειδοποιηθεί για μια αλλαγή στις [ΔΙΕΥΘΎΝΣΕΙς IP του Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="db80d-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="db80d-108">Βεβαιωθείτε ότι η υπηρεσία παροχής Internet (ISP) δεν αποκλείει τη θύρα.</span><span class="sxs-lookup"><span data-stu-id="db80d-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="db80d-109">Επαληθεύστε τις ρυθμίσεις του έξυπνου κεντρικού υπολογιστή και του διακομιστή προορισμού στις γραμμές σύνδεσης.</span><span class="sxs-lookup"><span data-stu-id="db80d-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="db80d-110">Σημειώστε ότι το Microsoft 365 δεν αποκλείει τις *εισερχόμενες* συνδέσεις με αυτόν τον τρόπο.</span><span class="sxs-lookup"><span data-stu-id="db80d-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
