---
title: Δεν βρέθηκαν συνδρομές στο Κέντρο ασφαλείας
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
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544108"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="bbf31-102">Δεν βρέθηκαν συνδρομές στο Κέντρο ασφαλείας</span><span class="sxs-lookup"><span data-stu-id="bbf31-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="bbf31-103">Εάν κατά την πρόσβαση σε Κέντρο προστασίας του Microsoft Defender λάβετε ένα μήνυμα "Δεν βρέθηκαν συνδρομές", αυτό σημαίνει ότι το Azure Active Directory (AAD) που χρησιμοποιείται για τη σύνδεση του χρήστη στην πύλη δεν διαθέτει Microsoft Defender ATP άδεια χρήσης.</span><span class="sxs-lookup"><span data-stu-id="bbf31-103">If while accessing Microsoft Defender Security Center you get a "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="bbf31-104">Οι Windows E5 και Office E5 είναι ξεχωριστές άδειες χρήσης.</span><span class="sxs-lookup"><span data-stu-id="bbf31-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="bbf31-105">Ανοίξτε μια υπόθεση υποστήριξης εάν η άδεια χρήσης αγοράστηκε, αλλά δεν έχει γίνει προμήθεια σε αυτήν την παρουσία AAD.</span><span class="sxs-lookup"><span data-stu-id="bbf31-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="bbf31-106">Είτε έχετε:</span><span class="sxs-lookup"><span data-stu-id="bbf31-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="bbf31-107">Ένα πιθανό πρόβλημα παροχής αδειών χρήσης.</span><span class="sxs-lookup"><span data-stu-id="bbf31-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="bbf31-108">Κατά λάθος, εκνεύσατε την άδεια χρήσης σε διαφορετικό Microsoft AAD από αυτό που χρησιμοποιήθηκε για τον έλεγχο ταυτότητας στην υπηρεσία.</span><span class="sxs-lookup"><span data-stu-id="bbf31-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>