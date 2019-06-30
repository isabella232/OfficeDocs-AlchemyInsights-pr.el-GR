---
title: Εργασία με iOS 1018 αναγνωριστικό κανόνα εφαρμογές VPP
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 58471f22ce78be1b40d3330a76a92d811819849d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35364851"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="3473d-102">Εργασία με iOS εφαρμογές VPP</span><span class="sxs-lookup"><span data-stu-id="3473d-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="3473d-103">Διαβάστε [Πώς να διαχειρίζεστε εφαρμογές iOS που αγοράζονται μέσω ενός προγράμματος όγκου αγοράς με Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) για να μάθετε σχετικά με τις δυνατότητες, οι περιορισμοί και τα βήματα για να χρησιμοποιήσετε το πρόγραμμα αγοράς Apple τόμου και η υποστήριξη για το σκοπό αυτό στο Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="3473d-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="3473d-104">**Κοινά θέματα:** "Θα αντιστοιχιστεί μια εφαρμογή VPP iOS των χρηστών, αλλά η εγκατάσταση απέτυχε."</span><span class="sxs-lookup"><span data-stu-id="3473d-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="3473d-105">Αυτό μπορεί να συμβεί εάν ένα μοναδικό διακριτικό VPP χρησιμοποιείται διαμέσου πολλών υπηρεσιών παροχής διαχείρισης κινητή συσκευή.</span><span class="sxs-lookup"><span data-stu-id="3473d-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="3473d-106">Διακριτικά VPP από Apple μπορεί να χρησιμοποιηθεί μόνο με μία υπηρεσία παροχής.</span><span class="sxs-lookup"><span data-stu-id="3473d-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="3473d-107">Εάν χρησιμοποιήσατε ένα διακριτικό VPP με πολλές υπηρεσίες παροχής, πρέπει να αποστείλετε ξανά το διακριτικό για Intune.</span><span class="sxs-lookup"><span data-stu-id="3473d-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="3473d-108">Η εγκατάσταση μπορεί να αποτύχει επίσης εάν ο συνολικός αριθμός εγκαταστάσεων υπερβαίνει τον αριθμό των αδειών χρήσης.</span><span class="sxs-lookup"><span data-stu-id="3473d-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="3473d-109">Για να προβάλετε μια αναφορά χρήσης για τις άδειες χρήσης σας, μεταβείτε το **κινητό Intune apps** \> σελίδα **άδειες App** .</span><span class="sxs-lookup"><span data-stu-id="3473d-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="3473d-110">Για να μάθετε τον τρόπο για να ανακτήσετε τις άδειες χρήσης που χρησιμοποιείται, ανατρέξτε στην ενότητα [αυτό το άρθρο.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="3473d-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
