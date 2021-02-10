---
title: Διαχείριση διαχειριζόμενης ταυτότητας που έχει εκχωρηθεί σε χρήστη
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8211"
- "9003230"
ms.openlocfilehash: a44cb484b6d89e6d5f67b2900c38dde3610b0e23
ms.sourcegitcommit: 23e778f7414e5f1a98cc786146fe76d622b458bc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177578"
---
# <a name="manage-a-user-assigned-managed-identity"></a><span data-ttu-id="2e427-102">Διαχείριση διαχειριζόμενης ταυτότητας που έχει εκχωρηθεί σε χρήστη</span><span class="sxs-lookup"><span data-stu-id="2e427-102">Manage a user-assigned managed identity</span></span>

<span data-ttu-id="2e427-103">Η διαχείριση μιας διαχειριζόμενης ταυτότητας στην οποία έχει εκχωρηθεί από το χρήστη περιλαμβάνει τα εξής:</span><span class="sxs-lookup"><span data-stu-id="2e427-103">The management of a user-assigned managed identity involves:</span></span>

- <span data-ttu-id="2e427-104">Ανάθεση ρόλων σε διαχειριζόμενη ταυτότητα που έχει εκχωρηθεί σε χρήστη</span><span class="sxs-lookup"><span data-stu-id="2e427-104">Assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="2e427-105">Διαγραφή διαχειριζόμενης ταυτότητας που έχει εκχωρηθεί σε χρήστη</span><span class="sxs-lookup"><span data-stu-id="2e427-105">Deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="2e427-106">Καταχώρηση διαχειριζόμενης ταυτότητας που έχει εκχωρηθεί σε χρήστη</span><span class="sxs-lookup"><span data-stu-id="2e427-106">Listing a user-assigned managed identity</span></span>

<span data-ttu-id="2e427-107">Για περισσότερες πληροφορίες σχετικά με τις εργασίες που αναφέρονται παραπάνω, ανατρέξτε στα ακόλουθα άρθρα:</span><span class="sxs-lookup"><span data-stu-id="2e427-107">For more information on the tasks mentioned above, see the following articles:</span></span>

- <span data-ttu-id="2e427-108">[Πώς μπορείτε να δημιουργήσετε μια διαχειριζόμενη ταυτότητα που έχει](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) εκχωρηθεί σε χρήστη, για την ανάθεση ρόλων σε διαχειριζόμενη ταυτότητα που έχει εκχωρηθεί σε χρήστη</span><span class="sxs-lookup"><span data-stu-id="2e427-108">[How to create a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="2e427-109">[Πώς μπορείτε να διαγράψετε μια διαχειριζόμενη ταυτότητα που έχει εκχωρηθεί σε χρήστη,](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) για τη διαγραφή μιας διαχειριζόμενης ταυτότητας που έχει εκχωρηθεί σε χρήστη</span><span class="sxs-lookup"><span data-stu-id="2e427-109">[How to delete a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="2e427-110">[Πώς μπορείτε να παραθέσετε μια διαχειριζόμενη ταυτότητα](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) που έχει εκχωρηθεί σε χρήστη, για καταχώρηση μιας διαχειριζόμενης ταυτότητας που έχει εκχωρηθεί σε χρήστη</span><span class="sxs-lookup"><span data-stu-id="2e427-110">[How to list a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for listing a user-assigned managed identity</span></span>

> [!NOTE]
> <span data-ttu-id="2e427-111">Επαληθεύστε εάν έχετε την ανάθεση **ρόλου "Διαχειριζόμενος συνεργάτης** ταυτότητας".</span><span class="sxs-lookup"><span data-stu-id="2e427-111">Verify whether you have the **Managed Identity Contributor** role assignment.</span></span> <span data-ttu-id="2e427-112">Η ανάθεση ρόλου απαιτείται για τη δημιουργία/διαγραφή διαχειριζόμενων ταυτοτήτων που έχουν εκχωρηθεί σε χρήστη.</span><span class="sxs-lookup"><span data-stu-id="2e427-112">That role assignment is required for creating/deleting user-assigned managed identities.</span></span>
