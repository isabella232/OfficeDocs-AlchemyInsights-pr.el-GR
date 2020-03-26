---
title: Εικονίδιο ημερολογίου που δεν εμφανίζεται στο πρόγραμμα-πελάτη του Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932195"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="d6517-102">Εικονίδιο ημερολογίου που δεν εμφανίζεται στο πρόγραμμα-πελάτη του Teams</span><span class="sxs-lookup"><span data-stu-id="d6517-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="d6517-103">Η καρτέλα ημερολογίου στο Teams απαιτεί πρόσβαση σε ένα γραμματοκιβώτιο του Exchange μέσω των υπηρεσιών Web του Exchange.</span><span class="sxs-lookup"><span data-stu-id="d6517-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="d6517-104">Το γραμματοκιβώτιο του Exchange μπορεί να είναι online ή εσωτερικής εγκατάστασης.</span><span class="sxs-lookup"><span data-stu-id="d6517-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="d6517-105">Για τους online χρήστες που δεν μπορούν να δουν την καρτέλα ημερολογίου, βεβαιωθείτε ότι [έχουν άδεια χρήσης για ένα γραμματοκιβώτιο του Exchange Online και ότι το γραμματοκιβώτιο έχει ενεργοποιηθεί](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="d6517-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="d6517-106">Εάν ο χρήστης έχει ένα έγκυρο γραμματοκιβώτιο στο Exchange Online, αλλά εξακολουθεί να μην μπορεί να δει την καρτέλα ημερολογίου, ενδέχεται να αντιμετωπίζετε κάποιο πρόβλημα με το δίκτυο.</span><span class="sxs-lookup"><span data-stu-id="d6517-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="d6517-107">Χρησιμοποιήστε το [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) και εκτελέστε τους **Ελέγχους συνδεσιμότητας των Υπηρεσιών Web του Microsoft Exchange** για τον επηρεαζόμενο χρήστη.</span><span class="sxs-lookup"><span data-stu-id="d6517-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="d6517-108">Τέλος, ελέγξτε το θέμα [Εφαρμογές του Teams – Πολιτικές εγκατάστασης εφαρμογών](https://admin.teams.microsoft.com/policies/app-setup) για να εξασφαλίσετε ότι η εφαρμογή "Ημερολόγιο" δεν έχει καταργηθεί από την πολιτική που εφαρμόζεται για τον χρήστη (πιθανότατα η **Καθολική (προεπιλογή σε επίπεδο οργανισμού)**).</span><span class="sxs-lookup"><span data-stu-id="d6517-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="d6517-109">Εάν οι χρήστες σας φιλοξενούνται στην εσωτερική εγκατάσταση, πρέπει να επιβεβαιώσετε ότι η υβριδική ρύθμιση παραμέτρων λειτουργεί κανονικά.</span><span class="sxs-lookup"><span data-stu-id="d6517-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="d6517-110">Χρησιμοποιήστε τον [Οδηγό υβριδικής ρύθμισης παραμέτρων](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) για να αντιμετωπίσετε το πρόβλημα..</span><span class="sxs-lookup"><span data-stu-id="d6517-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="d6517-111">Λάβετε υπόψη ότι το [Teams απαιτεί το Exchange 2016 CU3 ή νεότερη έκδοση](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="d6517-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
