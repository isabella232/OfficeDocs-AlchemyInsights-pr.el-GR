---
title: Αλλαγή διακομιστών ονομάτων
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 51532f42e7cbd39ebad3f0160465218c6e1454a2
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736649"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="e3e35-102">Ενημέρωση των διακομιστών ονομάτων του τομέα σας στο Office 365</span><span class="sxs-lookup"><span data-stu-id="e3e35-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="e3e35-103">Σημείωση: Η μετάδοση των αλλαγών στον διακομιστή ονομάτων ενδέχεται να διαρκέσει έως 48 ώρες.</span><span class="sxs-lookup"><span data-stu-id="e3e35-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="e3e35-104">Για να ρυθμίσετε τον τομέα σας στο Office 365, πρέπει να ενημερωθούν οι διακομιστές ονομάτων στο μητρώο καταχώρησής σας.</span><span class="sxs-lookup"><span data-stu-id="e3e35-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="e3e35-105">Δημιουργήστε ή επεξεργαστείτε τις εγγραφές των διακομιστών ονομάτων στο μητρώο καταχώρησης ονομάτων τομέα σας.</span><span class="sxs-lookup"><span data-stu-id="e3e35-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="e3e35-106">Μεταβείτε στην τοποθεσία Web του μητρώου καταχώρησης ονομάτων τομέων σας και βρείτε την περιοχή όπου μπορείτε να επεξεργαστείτε τους διακομιστές ονομάτων.</span><span class="sxs-lookup"><span data-stu-id="e3e35-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="e3e35-107">Δημιουργήστε ή επεξεργαστείτε δύο εγγραφές διακομιστών ονομάτων σύμφωνα με αυτές τις τιμές:</span><span class="sxs-lookup"><span data-stu-id="e3e35-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="e3e35-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="e3e35-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="e3e35-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="e3e35-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="e3e35-110">Αποθηκεύστε τις αλλαγές.</span><span class="sxs-lookup"><span data-stu-id="e3e35-110">Save changes.</span></span>

<span data-ttu-id="e3e35-111">Μπορείτε επίσης να βρείτε αναλυτικές οδηγίες σε αυτό το άρθρο: [Αλλαγή των διακομιστών ονομάτων για ρύθμιση του Office 365 με οποιοδήποτε μητρώο καταχώρησης ονομάτων τομέων](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="e3e35-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  