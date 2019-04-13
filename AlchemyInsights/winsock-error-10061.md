---
title: Σφάλμα Winsock 1554 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7651effc43cb0c4bc2fbbe5349bb72303943f493
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/13/2019
ms.locfileid: "31859140"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="c5049-102">Σφάλμα Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="c5049-102">Winsock error 10061</span></span>

<span data-ttu-id="c5049-103">Αυτός ο κωδικός σφάλματος σημαίνει ότι το Office 365 δεν ήταν δυνατό να δημιουργήσει μια υποδοχή TCP (σύνδεση) με τον κεντρικό υπολογιστή προορισμού.</span><span class="sxs-lookup"><span data-stu-id="c5049-103">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="c5049-104">Η πιο πιθανή αιτία αυτού του σφάλματος είναι κάποιο πρόβλημα με τις ρυθμίσεις παραμέτρων του τείχους προστασίας.</span><span class="sxs-lookup"><span data-stu-id="c5049-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="c5049-105">Για να διορθώσετε το πρόβλημα, ελέγξτε αυτές τις ρυθμίσεις:</span><span class="sxs-lookup"><span data-stu-id="c5049-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="c5049-106">Επαληθεύστε τις ρυθμίσεις του τείχους προστασίας σας με τις πληροφορίες [διευθύνσεων URL του Office 365 και περιοχές διευθύνσεων IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="c5049-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="c5049-107">Εάν το σφάλμα αφορά σε Exchange Online προστασίας (EOP), πρέπει να έχετε προηγουμένως ειδοποιηθεί για μια αλλαγή στις [διευθύνσεις Exchange Online προστασίας IP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="c5049-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="c5049-108">Βεβαιωθείτε ότι η υπηρεσία παροχής Internet (ISP) δεν εμποδίζει τη θύρα.</span><span class="sxs-lookup"><span data-stu-id="c5049-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="c5049-109">Επαληθεύστε τις Έξυπνες ρυθμίσεις διακομιστή κεντρικού υπολογιστή και του προορισμού σε σας γραμμές σύνδεσης.</span><span class="sxs-lookup"><span data-stu-id="c5049-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="c5049-110">Σημειώστε ότι Office 365 δεν αποκλειστούν οι *εισερχόμενες* συνδέσεις με αυτόν τον τρόπο.</span><span class="sxs-lookup"><span data-stu-id="c5049-110">Note that Office 365 doesn't block *incoming* connections in this manner.</span></span>
