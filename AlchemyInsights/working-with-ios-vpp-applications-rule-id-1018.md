---
title: Εργασία με iOS 1018 αναγνωριστικό κανόνα εφαρμογές VPP
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 5bcfb6dd7222bd102ff2620c19bfb943e7bd9591
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29471323"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="eeb14-102">Εργασία με iOS εφαρμογές VPP</span><span class="sxs-lookup"><span data-stu-id="eeb14-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="eeb14-103">Διαβάστε [Πώς να διαχειρίζεστε εφαρμογές iOS που αγοράζονται μέσω ενός προγράμματος όγκου αγοράς με Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) για να μάθετε σχετικά με τις δυνατότητες, οι περιορισμοί και τα βήματα για να χρησιμοποιήσετε το πρόγραμμα αγοράς Apple τόμου και η υποστήριξη για το σκοπό αυτό στο Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="eeb14-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="eeb14-104">**Κοινά θέματα:** "Θα αντιστοιχιστεί μια εφαρμογή VPP iOS των χρηστών, αλλά η εγκατάσταση απέτυχε."</span><span class="sxs-lookup"><span data-stu-id="eeb14-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="eeb14-p101">Αυτό μπορεί να συμβεί εάν ένα μοναδικό διακριτικό VPP χρησιμοποιείται διαμέσου πολλών υπηρεσιών παροχής διαχείρισης κινητή συσκευή. Διακριτικά VPP από Apple μπορεί να χρησιμοποιηθεί μόνο με μία υπηρεσία παροχής. Εάν χρησιμοποιήσατε ένα διακριτικό VPP με πολλές υπηρεσίες παροχής, πρέπει να αποστείλετε ξανά το διακριτικό για Intune.</span><span class="sxs-lookup"><span data-stu-id="eeb14-p101">This can happen if a single VPP token is used across multiple mobile device management providers. VPP tokens from Apple may only be used with one provider. If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="eeb14-p102">Η εγκατάσταση μπορεί να αποτύχει επίσης εάν ο συνολικός αριθμός εγκαταστάσεων υπερβαίνει τον αριθμό των αδειών χρήσης. Για να προβάλετε μια αναφορά χρήσης για τις άδειες χρήσης σας, μεταβείτε το **κινητό Intune apps** \> σελίδα **άδειες App** . Για να μάθετε τον τρόπο για να ανακτήσετε τις άδειες χρήσης που χρησιμοποιείται, ανατρέξτε στην ενότητα [αυτό το άρθρο.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="eeb14-p102">The installation can also fail if the total number of installations exceed the number of licenses. To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page. To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

