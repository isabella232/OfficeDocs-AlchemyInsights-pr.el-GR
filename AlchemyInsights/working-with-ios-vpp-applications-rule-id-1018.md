---
title: Εργασία με το αναγνωριστικό 1018 του κανόνα εφαρμογών του iOS VPP
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688946"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="97ee9-102">Εργασία με εφαρμογές του iOS VPP</span><span class="sxs-lookup"><span data-stu-id="97ee9-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="97ee9-103">Διαβάστε [Πώς μπορείτε να διαχειριστείτε τις εφαρμογές iOS που αγοράζονται μέσω ενός προγράμματος αγοράς τόμου με το Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) για να μάθετε σχετικά με τις δυνατότητες, τους περιορισμούς και τα βήματα για να κάνετε χρήση του προγράμματος αγοράς τόμου Apple και της υποστήριξης για αυτό στο Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="97ee9-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="97ee9-104">**Συνηθισμένα προβλήματα:** "Ανέθεσα μια εφαρμογή iOS VPP στους χρήστες μου, αλλά η εγκατάσταση απέτυχε."</span><span class="sxs-lookup"><span data-stu-id="97ee9-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="97ee9-105">Αυτό μπορεί να συμβεί εάν χρησιμοποιείται ένα μόνο διακριτικό VPP σε πολλές υπηρεσίες παροχής διαχείρισης κινητών συσκευών.</span><span class="sxs-lookup"><span data-stu-id="97ee9-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="97ee9-106">Τα κουπόνια VPP από την Apple μπορούν να χρησιμοποιηθούν μόνο με μία υπηρεσία παροχής.</span><span class="sxs-lookup"><span data-stu-id="97ee9-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="97ee9-107">Εάν χρησιμοποιήσατε ένα διακριτικό VPP με πολλές υπηρεσίες παροχής, πρέπει να επαναλάβετε την αποστολή του διακριτικού σε Intune.</span><span class="sxs-lookup"><span data-stu-id="97ee9-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="97ee9-108">Η εγκατάσταση μπορεί επίσης να αποτύχει εάν ο συνολικός αριθμός των εγκαταστάσεων υπερβεί τον αριθμό των αδειών χρήσης.</span><span class="sxs-lookup"><span data-stu-id="97ee9-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="97ee9-109">Για να προβάλετε μια αναφορά χρήσης για τις άδειες χρήσης σας, μεταβείτε στη σελίδα "άδειες χρήσης εφαρμογών για **κινητές συσκευές του Intune** " \> **App licenses** .</span><span class="sxs-lookup"><span data-stu-id="97ee9-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="97ee9-110">Για να μάθετε πώς μπορείτε να ανακτήσετε τις άδειες χρήσης που χρησιμοποιούνται, ανατρέξτε σε [αυτό το άρθρο.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="97ee9-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
