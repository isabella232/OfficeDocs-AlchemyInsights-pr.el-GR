---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685598"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="10e88-102">Αποκλεισμός παλαιού ελέγχου ταυτότητας</span><span class="sxs-lookup"><span data-stu-id="10e88-102">Blocking legacy authentication</span></span>

<span data-ttu-id="10e88-103">Ο έλεγχος ταυτότητας παλαιού τύπου είναι ένας όρος που αναφέρεται σε μια αίτηση ελέγχου ταυτότητας που γίνεται από:</span><span class="sxs-lookup"><span data-stu-id="10e88-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="10e88-104">Παλαιότερα προγράμματα-πελάτες του Office που δεν χρησιμοποιούν σύγχρονο έλεγχο ταυτότητας (για παράδειγμα, πρόγραμμα-πελάτης του Office 2010).</span><span class="sxs-lookup"><span data-stu-id="10e88-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="10e88-105">Οποιοσδήποτε υπολογιστής-πελάτης που χρησιμοποιεί πρωτόκολλα αλληλογραφίας παλαιού τύπου, όπως IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="10e88-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="10e88-106">Για περισσότερες πληροφορίες σχετικά με τον αποκλεισμό παλαιού ελέγχου ταυτότητας και την ενεργοποίηση του σύγχρονου ελέγχου ταυτότητας, ανατρέξτε στο θέμα [Αποκλεισμός ελέγχου ταυτότητας παλαιού τύπου](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)</span><span class="sxs-lookup"><span data-stu-id="10e88-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="10e88-107">Οι προεπιλογές ασφαλείας στο Azure Active Directory (Azure AD) διευκολύνουν την ασφάλειά σας και συμβάλλουν στην προστασία του οργανισμού σας.</span><span class="sxs-lookup"><span data-stu-id="10e88-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="10e88-108">Οι προεπιλογές ασφαλείας περιέχουν προκαθορισμένες ρυθμίσεις ασφαλείας για συνηθισμένες επιθέσεις.</span><span class="sxs-lookup"><span data-stu-id="10e88-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="10e88-109">Για περισσότερες πληροφορίες σχετικά με τις προεπιλογές ασφαλείας, ανατρέξτε στο θέμα [Τι είναι οι προεπιλογές ασφαλείας;](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="10e88-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="10e88-110">**Σημείωση**: Εάν ο ενοικιαστής σας δημιουργήθηκε στις ή μετά τις 22 Οκτωβρίου 2019, είναι πιθανό να αντιμετωπίζετε τη νέα συμπεριφορά ασφαλούς από προεπιλογή και να έχετε ήδη ενεργοποιημένες τις προεπιλογές ασφαλείας στον μισθωτή σας.</span><span class="sxs-lookup"><span data-stu-id="10e88-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="10e88-111">Σε μια προσπάθεια για την προστασία όλων των χρηστών μας, οι προεπιλογές ασφαλείας εκσύρονται σε όλους τους νέους μισθωτές που δημιουργήθηκαν.</span><span class="sxs-lookup"><span data-stu-id="10e88-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
