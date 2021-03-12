---
title: Μήνυμα "Δεν βρέθηκαν συνδρομές" στο Κέντρο ασφαλείας
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "50713603"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="e677b-102">Μήνυμα "Δεν βρέθηκαν συνδρομές" στο Κέντρο ασφαλείας</span><span class="sxs-lookup"><span data-stu-id="e677b-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="e677b-103">Αν κατά την πρόσβαση στο Κέντρο προστασίας του Microsoft Defender εμφανιστεί το μήνυμα "Δεν βρέθηκαν συνδρομές", αυτό σημαίνει ότι το Azure Active Directory (AAD) που χρησιμοποιήθηκε για τη σύνδεση του χρήστη στην πύλη δεν διαθέτει άδεια χρήσης atP του Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="e677b-103">If while accessing Microsoft Defender Security Center you get a  "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="e677b-104">Οι άδειες χρήσης των Windows E5 και Office E5 είναι ξεχωριστές άδειες χρήσης.</span><span class="sxs-lookup"><span data-stu-id="e677b-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="e677b-105">Ανοίξτε μια υπόθεση υποστήριξης εάν η άδεια χρήσης αγοράστηκε, αλλά δεν έχει γίνει προμήθεια σε αυτήν την παρουσία AAD.</span><span class="sxs-lookup"><span data-stu-id="e677b-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="e677b-106">Είτε έχετε:</span><span class="sxs-lookup"><span data-stu-id="e677b-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="e677b-107">Ένα πιθανό πρόβλημα παροχής άδειας χρήσης.</span><span class="sxs-lookup"><span data-stu-id="e677b-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="e677b-108">Εκδόσατε κατά λάθος την άδεια χρήσης σε ένα διαφορετικό Microsoft AAD από αυτό που χρησιμοποιήθηκε για τον έλεγχο ταυτότητας στην υπηρεσία.</span><span class="sxs-lookup"><span data-stu-id="e677b-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>