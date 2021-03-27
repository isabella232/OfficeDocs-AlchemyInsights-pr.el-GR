---
title: Αυτόματη είσοδος στον Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398729"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="26113-102">Αυτόματη είσοδος στον Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="26113-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="26113-103">Ο Microsoft Edge χρησιμοποιεί τον προεπιλεγμένο λογαριασμό λειτουργικού συστήματος για την αυτόματη είσοδο ενός χρήστη σύμφωνα με τον τρόπο ρύθμισης των παραμέτρων της συσκευής του χρήστη.</span><span class="sxs-lookup"><span data-stu-id="26113-103">Microsoft Edge uses the OS default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="26113-104">Τα σενάρια για κάθε τύπο ρύθμισης παραμέτρων συσκευής και τη διαδικασία σύνδεσης εξαρτημένου χρήστη περιγράφονται παρακάτω:</span><span class="sxs-lookup"><span data-stu-id="26113-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

- <span data-ttu-id="26113-105">**Η συσκευή είναι υβριδική/AAD-J:** Αυτή η επιλογή είναι διαθέσιμη στα Windows 10, τα Windows κάτω επιπέδου και τις αντίστοιχες εκδόσεις διακομιστή.</span><span class="sxs-lookup"><span data-stu-id="26113-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="26113-106">Οι χρήστες έχουν εισέλθει αυτόματα με τους λογαριασμούς τους Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="26113-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
- <span data-ttu-id="26113-107">**Η συσκευή είναι συνδεδεμένος με τομέα:** Αυτή η επιλογή είναι διαθέσιμη στα Windows 10, τα Windows κάτω επιπέδου και τις αντίστοιχες εκδόσεις διακομιστή.</span><span class="sxs-lookup"><span data-stu-id="26113-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="26113-108">Από προεπιλογή, οι χρήστες με λογαριασμούς τομέα δεν είναι αυτόματα συνδεδεμένοι. Για να ενεργοποιήσετε την αυτόματη είσοδο για αυτούς, χρησιμοποιήστε την πολιτική **ConfigureOnPremisesAccountAutoSignIn.**</span><span class="sxs-lookup"><span data-stu-id="26113-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="26113-109">Για να ενεργοποιήσετε την αυτόματη είσοδο για τους χρήστες με λογαριασμούς Azure AD, εξετάστε το ενδεχόμενο να ενώνετε υβριδικά τις συσκευές τους.</span><span class="sxs-lookup"><span data-stu-id="26113-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
- <span data-ttu-id="26113-110">**Ο προεπιλεγμένος** λογαριασμός του λειτουργικού συστήματος είναι ένας λογαριασμός Microsoft: Αυτή η επιλογή είναι διαθέσιμη στα Windows 10 RS3 (έκδοση 1709, έκδοση 10.0.16299) και νεότερες εκδόσεις.</span><span class="sxs-lookup"><span data-stu-id="26113-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="26113-111">Το σενάριο δεν είναι πιθανό να παρουσιαστεί σε εταιρικές συσκευές.</span><span class="sxs-lookup"><span data-stu-id="26113-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="26113-112">Ωστόσο, εάν ο προεπιλεγμένος λογαριασμός λειτουργικού συστήματος είναι λογαριασμός Microsoft, τότε ο Microsoft Edge θα κάνει αυτόματη είσοδο στο χρήστη με το λογαριασμό Microsoft.</span><span class="sxs-lookup"><span data-stu-id="26113-112">However, if the OS default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
