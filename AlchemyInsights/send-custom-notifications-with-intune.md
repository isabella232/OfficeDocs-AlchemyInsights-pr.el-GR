---
title: Αποστολή προσαρμοσμένων ειδοποιήσεων με το Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992313"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="a2cc5-102">Πώς να στείλετε προσαρμοσμένες ειδοποιήσεις στους χρήστες των διαχειριζόμενων συσκευών iOS και Android</span><span class="sxs-lookup"><span data-stu-id="a2cc5-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="a2cc5-103">Οι προσαρμοσμένες ειδοποιήσεις για το Intune υποβάλλονται σε επεξεργασία από την εφαρμογή πύλης εταιρείας στη συσκευή ενός χρήστη.</span><span class="sxs-lookup"><span data-stu-id="a2cc5-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="a2cc5-104">Στη συνέχεια, η εφαρμογή δημιουργεί την ειδοποίηση push σε αυτήν τη συσκευή.</span><span class="sxs-lookup"><span data-stu-id="a2cc5-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="a2cc5-105">Τα παρακάτω είναι προαπαιτούμενα συσκευών για την υποστήριξη παραλαβής προσαρμοσμένων ειδοποιήσεων και για την εφαρμογή στη συνέχεια να δημιουργήσετε την ειδοποίηση push:</span><span class="sxs-lookup"><span data-stu-id="a2cc5-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="a2cc5-106">Η συσκευή πρέπει να έχει εγκατεστημένη την εφαρμογή πύλης εταιρείας.</span><span class="sxs-lookup"><span data-stu-id="a2cc5-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="a2cc5-107">Η συσκευή πρέπει να επιτρέπει στην εφαρμογή πύλης εταιρείας να αποστέλλει ειδοποιήσεις push.</span><span class="sxs-lookup"><span data-stu-id="a2cc5-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="a2cc5-108">Όταν η εφαρμογή έχει εγκατασταθεί ή ενημερωθεί, θα ζητήσει από το χρήστη να επιτρέψει τις ειδοποιήσεις.</span><span class="sxs-lookup"><span data-stu-id="a2cc5-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="a2cc5-109">Οι συσκευές Android πρέπει να έχουν εγκατεστημένες τις υπηρεσίες Google Play.</span><span class="sxs-lookup"><span data-stu-id="a2cc5-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="a2cc5-110">Η συσκευή πρέπει να εγγραφεί στο Intune.</span><span class="sxs-lookup"><span data-stu-id="a2cc5-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="a2cc5-111">Για περισσότερες πληροφορίες, όπως πώς να στείλετε ένα μήνυμα, ανατρέξτε στην [τεκμηρίωση της δυνατότητας](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="a2cc5-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
