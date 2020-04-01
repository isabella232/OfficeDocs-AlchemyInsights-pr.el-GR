---
title: Αποκλεισμός παλαιού τύπουAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: e7bff5f9fcf6f2f2c77e93c2f27f585f2cc18bea
ms.sourcegitcommit: 98231a228ecb2bf14ec3b96d4dd4ccf2507617a3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/01/2020
ms.locfileid: "43079260"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="1b971-102">Αποκλεισμός ελέγχου ταυτότητας παλαιού τύπου</span><span class="sxs-lookup"><span data-stu-id="1b971-102">Blocking legacy authentication</span></span>

<span data-ttu-id="1b971-103">Ο έλεγχος ταυτότητας παλαιού τύπου είναι ένας όρος που αναφέρεται σε μια αίτηση ελέγχου ταυτότητας που υποβλήθηκε από:</span><span class="sxs-lookup"><span data-stu-id="1b971-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="1b971-104">Παλαιότερα προγράμματα-πελάτες του Office που δεν χρησιμοποιούν σύγχρονο έλεγχο ταυτότητας (για παράδειγμα, υπολογιστή-πελάτη ς του Office 2010).</span><span class="sxs-lookup"><span data-stu-id="1b971-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="1b971-105">Οποιοσδήποτε υπολογιστής-πελάτης χρησιμοποιεί πρωτόκολλα αλληλογραφίας παλαιού τύπου, όπως IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="1b971-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="1b971-106">Για περισσότερες πληροφορίες σχετικά με τον αποκλεισμό του ελέγχου ταυτότητας παλαιού τύπου και την ενεργοποίηση του σύγχρονου ελέγχου ταυτότητας, ανατρέξτε στην ενότητα [Αποκλεισμός ελέγχου ταυτότητας παλαιού τύπου](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="1b971-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="1b971-107">Οι προεπιλογές ασφαλείας στην υπηρεσία καταλόγου Azure Active Directory (Azure AD) διευκολύνουν την ασφάλεια και την προστασία του οργανισμού σας.</span><span class="sxs-lookup"><span data-stu-id="1b971-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="1b971-108">Οι προεπιλογές ασφαλείας περιέχουν προκαθορισμένες ρυθμίσεις ασφαλείας για κοινές επιθέσεις.</span><span class="sxs-lookup"><span data-stu-id="1b971-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="1b971-109">Για περισσότερες πληροφορίες σχετικά με τις προεπιλογές ασφαλείας, ανατρέξτε στην ενότητα [Ποιες είναι οι προεπιλογές ασφαλείας;](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="1b971-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="1b971-110">**Σημείωση:** Εάν ο μισθωτής σας δημιουργήθηκε στις ή μετά τις 22 Οκτωβρίου 2019, είναι πιθανό να αντιμετωπίζετε τη νέα συμπεριφορά ασφαλούς ασφαλείας από προεπιλογή και να έχετε ήδη ενεργοποιήσει τις προεπιλογές ασφαλείας στο μισθωτή σας.</span><span class="sxs-lookup"><span data-stu-id="1b971-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="1b971-111">Σε μια προσπάθεια προστασίας όλων των χρηστών μας, οι προεπιλογές ασφαλείας ξεδιπλώνονται σε όλους τους νέους μισθωτές που δημιουργούνται.</span><span class="sxs-lookup"><span data-stu-id="1b971-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
