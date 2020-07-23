---
title: Αντιμετώπιση προβλημάτων συγχρονισμού κωδικού πρόσβασης
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387877"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="4bd27-102">Αντιμετώπιση προβλημάτων συγχρονισμού κωδικού πρόσβασης</span><span class="sxs-lookup"><span data-stu-id="4bd27-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="4bd27-103">Για να αντιμετωπίσετε προβλήματα συγχρονισμού κωδικού πρόσβασης, ξεκινήστε χρησιμοποιώντας αυτήν την εργασία αντιμετώπισης προβλημάτων AAD Connect για να προσδιορίσετε γιατί οι κωδικοί πρόσβασης δεν συγχρονίζονται.</span><span class="sxs-lookup"><span data-stu-id="4bd27-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="4bd27-104">Για να ξεκινήσετε, μεταβείτε στην ενότητα [Διαχείριση άμεσου συγχρονισμού](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="4bd27-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="4bd27-105">Ανοίξτε μια νέα περίοδο λειτουργίας του Windows PowerShell στο διακομιστή Azure AD Connect και ενεργοποιήστε την επιλογή **Εκτέλεση ως διαχειριστής.**</span><span class="sxs-lookup"><span data-stu-id="4bd27-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="4bd27-106">Εκτελέστε το Set-ExecutionPolicy RemoteSigned ή Set-ExecutionPolicy Χωρίς περιορισμούς.</span><span class="sxs-lookup"><span data-stu-id="4bd27-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="4bd27-107">Ξεκινήστε τον "Οδηγό σύνδεσης Azure AD".</span><span class="sxs-lookup"><span data-stu-id="4bd27-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="4bd27-108">Μεταβείτε στη σελίδα "Πρόσθετες εργασίες" > **Αντιμετώπιση προβλημάτων**  >  **στο επόμενο**.</span><span class="sxs-lookup"><span data-stu-id="4bd27-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="4bd27-109">Επιλέξτε **Εκκίνηση** για να ανοίξετε το μενού αντιμετώπισης προβλημάτων του PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4bd27-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="4bd27-110">Επιλέξτε **Αντιμετώπιση προβλημάτων συγχρονισμού κωδικού πρόσβασης**.</span><span class="sxs-lookup"><span data-stu-id="4bd27-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="4bd27-111">Το ζήτημα είναι συνήθως ότι ένας κωδικός πρόσβασης δεν συγχρονίζεται για ένα συγκεκριμένο λογαριασμό χρήστη.</span><span class="sxs-lookup"><span data-stu-id="4bd27-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="4bd27-112">**Σημειώσεις** Ο συγχρονισμός κωδικού πρόσβασης αποτυγχάνει εάν ο τελευταίος επιτυχής συγχρονισμός κωδικού πρόσβασης ήταν πριν από λίγο καιρό.</span><span class="sxs-lookup"><span data-stu-id="4bd27-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="4bd27-113">Για περισσότερη βοήθεια σχετικά με την αντιμετώπιση του συγχρονισμού κωδικών πρόσβασης, ανατρέξτε στο θέμα [Αντιμετώπιση προβλημάτων συγχρονισμού κατακερματισμού κωδικού πρόσβασης με το συγχρονισμό Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="4bd27-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>