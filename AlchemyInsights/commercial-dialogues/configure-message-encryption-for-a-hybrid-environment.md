---
title: Ρύθμιση παραμέτρων κρυπτογράφησης μηνυμάτων για υβριδικό περιβάλλον
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 22c2468b7639680b447b6464431a79b69f7198c3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745402"
---
# <a name="configure-message-encryption-for-a-hybrid-environment"></a><span data-ttu-id="c6101-102">Ρύθμιση παραμέτρων κρυπτογράφησης μηνυμάτων για υβριδικό περιβάλλον</span><span class="sxs-lookup"><span data-stu-id="c6101-102">Configure message encryption for a hybrid environment</span></span>

<span data-ttu-id="c6101-103">Για υβριδικά περιβάλλοντα Exchange, οι χρήστες εσωτερικής εγκατάστασης μπορούν να στέλνουν κρυπτογραφημένα μηνύματα ηλεκτρονικού ταχυδρομείου χρησιμοποιώντας την Κρυπτογράφηση μηνυμάτων του Office (OME) μόνο εάν το ηλεκτρονικό ταχυδρομείο δρομολογηθεί μέσω του Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="c6101-103">For hybrid Exchange environments, on-premises users can send encrypted email using Office Message Encryption (OME) only if email is routed through Exchange Online.</span></span>

<span data-ttu-id="c6101-104">Για να κρυπτογραφήσετε μηνύματα ηλεκτρονικού ταχυδρομείου χρησιμοποιώντας OME, ακολουθήστε τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="c6101-104">To encrypt emails using OME, perform the following steps:</span></span>

1. <span data-ttu-id="c6101-105">Χρησιμοποιήστε τον [Οδηγό υβριδικής ρύθμισης παραμέτρων](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) για να ρυθμίσετε το υβριδικό περιβάλλον σας.</span><span class="sxs-lookup"><span data-stu-id="c6101-105">Use the [Hybrid Configuration wizard](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) to set up your hybrid environment.</span></span> <span data-ttu-id="c6101-106">Δεν απαιτούνται ειδικά βήματα για τη ρύθμιση της κρυπτογράφησης.</span><span class="sxs-lookup"><span data-stu-id="c6101-106">No special steps are required for setting up encryption.</span></span>
2. <span data-ttu-id="c6101-107">[Ρυθμίστε τους κανόνες ροής αλληλογραφίας για κρυπτογράφηση](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) όπως θα κάνατε κανονικά.</span><span class="sxs-lookup"><span data-stu-id="c6101-107">[Set up your mail flow rules for encryption](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) like you normally would.</span></span>


