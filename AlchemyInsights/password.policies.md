---
title: Πολιτικές κωδικού πρόσβασης
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744985"
---
# <a name="password-policies"></a><span data-ttu-id="73d98-102">Πολιτικές κωδικού πρόσβασης</span><span class="sxs-lookup"><span data-stu-id="73d98-102">Password policies</span></span>

<span data-ttu-id="73d98-103">**Έχω προβλήματα με την πολιτική κωδικού πρόσβασης για ένα χρήστη**</span><span class="sxs-lookup"><span data-stu-id="73d98-103">**I'm having problems with the password policy for a user**</span></span>

- <span data-ttu-id="73d98-104">Η πολιτική κωδικού πρόσβασης για ένα χρήστη εξαρτάται από το εάν ο χρήστης είναι μόνο στο cloud ή στην εσωτερική εγκατάσταση.</span><span class="sxs-lookup"><span data-stu-id="73d98-104">The password policy for a user depends on whether the user is cloud only or on-premises.</span></span>
- <span data-ttu-id="73d98-105">Μόνο οι χρήστες στο cloud πρέπει να επιλέξουν έναν κωδικό πρόσβασης που πληροί τις απαιτήσεις αυτού του άρθρου: [Πολιτικές κωδικού πρόσβασης που ισχύουν μόνο για λογαριασμούς χρηστών cloud](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="73d98-105">Cloud only users must choose a password that meets the requirements in this article: [Password policies that only apply to cloud user accounts](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span></span>
- <span data-ttu-id="73d98-106">Οι χρήστες εσωτερικής εγκατάστασης πρέπει να επιλέξουν έναν κωδικό πρόσβασης που πληροί τις απαιτήσεις εσωτερικής εγκατάστασης.</span><span class="sxs-lookup"><span data-stu-id="73d98-106">On-premises users must choose a password that meets the on-premises requirements.</span></span> <span data-ttu-id="73d98-107">Εάν ένας χρήστης εσωτερικής εγκατάστασης δεν μπορεί να ορίσει τον κωδικό πρόσβασής του, ελέγξτε τις απαιτήσεις εσωτερικής εγκατάστασης.</span><span class="sxs-lookup"><span data-stu-id="73d98-107">If an on-premises user is unable to set their password, check your on-premises requirements.</span></span>

<span data-ttu-id="73d98-108">**Δεν ξέρω πώς μπορείτε να ορίσετε ή να ελέγξετε τις πολιτικές λήξης κωδικού πρόσβασης**</span><span class="sxs-lookup"><span data-stu-id="73d98-108">**I don't know how to set or check password expiration policies**</span></span>

- <span data-ttu-id="73d98-109">Μπορείτε να ορίσετε και να ελέγξετε την πολιτική λήξης για χρήστες cloud στο μισθωτή σας χρησιμοποιώντας το PowerShell.</span><span class="sxs-lookup"><span data-stu-id="73d98-109">You can set and check the expiration policy for cloud users in your tenant by using PowerShell.</span></span> <span data-ttu-id="73d98-110">Ακολουθήστε τις οδηγίες σε αυτό το άρθρο: [Ορίστε ή ελέγξτε τις πολιτικές κωδικού πρόσβασης χρησιμοποιώντας το PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span><span class="sxs-lookup"><span data-stu-id="73d98-110">Follow the instructions in this article: [Set or check the password policies by using PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span></span>
- <span data-ttu-id="73d98-111">Η πολιτική λήξης κωδικού πρόσβασης για τους χρήστες εσωτερικής εγκατάστασης έχει οριστεί στο AD εσωτερικής εγκατάστασης.</span><span class="sxs-lookup"><span data-stu-id="73d98-111">The password expiration policy for on-premises users is set in your on-premises AD.</span></span>

<span data-ttu-id="73d98-112">**Άλλες χρήσιμες συνδέσεις:**</span><span class="sxs-lookup"><span data-stu-id="73d98-112">**Other Helpful links:**</span></span>
- [<span data-ttu-id="73d98-113">Γρήγορα αποτελέσματα με την επαναφορά κωδικού πρόσβασης</span><span class="sxs-lookup"><span data-stu-id="73d98-113">Getting Started with Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [<span data-ttu-id="73d98-114">Αντιμετώπιση προβλημάτων επαναφοράς κωδικού πρόσβασης που ξεκίνησε από το διαχειριστή</span><span class="sxs-lookup"><span data-stu-id="73d98-114">Troubleshoot Administrator-initiated Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
