---
title: Πρόβλημα με τις ομάδες ασφαλείας
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
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177494"
---
# <a name="issue-with-security-groups"></a><span data-ttu-id="72bc5-102">Πρόβλημα με τις ομάδες ασφαλείας</span><span class="sxs-lookup"><span data-stu-id="72bc5-102">Issue with security groups</span></span>

<span data-ttu-id="72bc5-103">**Εάν εμφανίζεται το σφάλμα δικτύου AADDS104**</span><span class="sxs-lookup"><span data-stu-id="72bc5-103">**If you are getting Network Error AADDS104**</span></span>

<span data-ttu-id="72bc5-104">Οι μη έγκυροι κανόνες ομάδας ασφαλείας δικτύου είναι η πιο συνηθισμένη αιτία σφαλμάτων δικτύου για τις υπηρεσίες τομέα Azure Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="72bc5-104">Invalid network security group rules are the most common cause of network errors for Azure Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="72bc5-105">Η ομάδα ασφαλείας δικτύου για το εικονικό δίκτυο πρέπει να επιτρέπει την πρόσβαση σε συγκεκριμένες θύρες και πρωτόκολλα.</span><span class="sxs-lookup"><span data-stu-id="72bc5-105">The network security group for the virtual network must allow access to specific ports and protocols.</span></span> <span data-ttu-id="72bc5-106">Εάν αυτές οι θύρες έχουν αποκλειστεί, η πλατφόρμα Azure δεν μπορεί να παρακολουθεί ή να ενημερώνει τον διαχειριζόμενο τομέα.</span><span class="sxs-lookup"><span data-stu-id="72bc5-106">If these ports are blocked, the Azure platform can't monitor or update the managed domain.</span></span> <span data-ttu-id="72bc5-107">Ο συγχρονισμός μεταξύ του Azure AD και του Azure AD DS επίσης επηρεάζει.</span><span class="sxs-lookup"><span data-stu-id="72bc5-107">The synchronization between the Azure AD and Azure AD DS is also impacted.</span></span> <span data-ttu-id="72bc5-108">Βεβαιωθείτε ότι έχετε ανοιχτές τις προεπιλεγμένες θύρες για να αποφύγετε τη διακοπή της υπηρεσίας.</span><span class="sxs-lookup"><span data-stu-id="72bc5-108">Ensure you keep the default ports open to avoid interruption in service.</span></span>

<span data-ttu-id="72bc5-109">Για να κατανοήσετε και να επιλύσετε συνήθεις ειδοποιήσεις για ζητήματα ρύθμισης παραμέτρων ομάδας ασφαλείας δικτύου, ανατρέξτε στο θέμα ["Προσθήκη και επαλήθευση ομάδων ασφαλείας".](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules)</span><span class="sxs-lookup"><span data-stu-id="72bc5-109">To understand and to resolve common alerts for network security group configuration issues, see [Add and Verify Security Groups](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span></span>
