---
title: Εικονική ρύθμιση παραμέτρων με τις υπηρεσίες τομέα AAD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885202"
---
# <a name="virtual-configuration-with-aad-domain-services"></a><span data-ttu-id="dca05-102">Εικονική ρύθμιση παραμέτρων με τις υπηρεσίες τομέα AAD</span><span class="sxs-lookup"><span data-stu-id="dca05-102">Virtual configuration with AAD domain services</span></span>

<span data-ttu-id="dca05-103">Η εικονική ρύθμιση παραμέτρων με τις υπηρεσίες τομέα του AAD περιλαμβάνει τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="dca05-103">Virtual configuration with AAD domain services involves the following steps:</span></span> 

1. <span data-ttu-id="dca05-104">Έλεγχος της εύρυθμης λειτουργίας του τομέα σας στην πύλη Azure https://aka.ms/aadds-health</span><span class="sxs-lookup"><span data-stu-id="dca05-104">Checking your domain’s health on the Azure portal https://aka.ms/aadds-health</span></span>
2. <span data-ttu-id="dca05-105">Έλεγχος του NSG για κανόνες που εμποδίζουν τις θύρες που απαιτούνται για το συγχρονισμό στις υπηρεσίες τομέα AD Azure στην πύλη https://aka.ms/aadds-networking</span><span class="sxs-lookup"><span data-stu-id="dca05-105">Checking your NSG for rules that block ports needed to synchronize in Azure AD Domain Services on the portal https://aka.ms/aadds-networking</span></span>
3. <span data-ttu-id="dca05-106">Διασφάλιση ότι το εικονικό σας δίκτυο αναπτύσσεται στην ίδια περιοχή Azure με τις υπηρεσίες τομέα AD Azure-διαχειριζόμενο τομέα.</span><span class="sxs-lookup"><span data-stu-id="dca05-106">Ensuring that your virtual network is deployed in the same Azure Region as your Azure AD Domain Services-managed domain.</span></span>
4. <span data-ttu-id="dca05-107">Βεβαιωθείτε ότι δεν διαθέτετε τομέα με το ίδιο όνομα τομέα που είναι διαθέσιμο στο εικονικό δίκτυο.</span><span class="sxs-lookup"><span data-stu-id="dca05-107">Ensuring you don’t have an existent domain with the same domain name available on the virtual network.</span></span>

<span data-ttu-id="dca05-108">Για περισσότερες λεπτομέρειες σχετικά με την εξέταση του σχεδιασμού στο εικονικό δίκτυο Azure για την υποστήριξη των υπηρεσιών τομέα AAD, ανατρέξτε στο θέμα [εικονικό δίκτυο εξέτασης](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span><span class="sxs-lookup"><span data-stu-id="dca05-108">For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span></span>

