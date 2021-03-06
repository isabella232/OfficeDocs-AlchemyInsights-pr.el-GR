---
title: 'Σφάλμα εγγραφής στο Android Enterprise: Εντοπισμός της ρύθμιση MGP'
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000652"
- "8340"
ms.openlocfilehash: 6ac90611bbe626e7f11b817965fd2d3c7fbf98c1
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50508553"
---
# <a name="android-enterprise-enrollment-error-mgp-set-up-detection"></a><span data-ttu-id="64dcf-102">Σφάλμα εγγραφής στο Android Enterprise: Εντοπισμός της ρύθμιση MGP</span><span class="sxs-lookup"><span data-stu-id="64dcf-102">Android Enterprise enrollment error: MGP set-up detection</span></span>

<span data-ttu-id="64dcf-103">Εντοπίσαμε ότι το Διαχειριζόμενο Google Play δεν έχει ρυθμιστεί ή δεν έχει αποσυνδεθεί για τον λογαριασμό σας.</span><span class="sxs-lookup"><span data-stu-id="64dcf-103">We have detected that Managed Google Play is not set up or disconnected for your account.</span></span> <span data-ttu-id="64dcf-104">Αυτό μπορεί να προκαλέσει αποτυχία εγγραφής συσκευών σε σενάρια Android Enterprise όπου απαιτείται διαχειριζόμενη σύνδεση του Google Play.</span><span class="sxs-lookup"><span data-stu-id="64dcf-104">This can cause failure to enroll devices in Android Enterprise scenarios where a Managed Google Play connection is required.</span></span>

<span data-ttu-id="64dcf-105">Μπορείτε να ελέγξετε την κατάσταση της Διαχειριζόμενης σύνδεσης Του Google Play στην κονσόλα MEM στην περιοχή Διαχείριση μισθωτή > Κατάσταση μισθωτή **> Connector** και να εξετάσετε την ακόλουθη τεκμηρίωση για να μάθετε πώς μπορείτε να συνδέσετε τον λογαριασμό σας Intune στο διαχειριζόμενο λογαριασμό σας Google: Συνδέστε το λογαριασμό **[σας Intune](https://docs.microsoft.com/mem/intune/enrollment/connect-intune-android-enterprise)** στο διαχειριζόμενο λογαριασμό σας στο Google Play.</span><span class="sxs-lookup"><span data-stu-id="64dcf-105">You can check Managed Google Play Connection status in the MEM console under **Tenant Administration > Tenant status > Connector status** and review the following documentation to learn about how to connect your Intune account to your Managed Google account: **[Connect your Intune account to your Managed Google Play account](https://docs.microsoft.com/mem/intune/enrollment/connect-intune-android-enterprise)**.</span></span>
