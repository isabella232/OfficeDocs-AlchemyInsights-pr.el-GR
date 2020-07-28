---
title: Απογραφή συσκευής Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439652"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="d3d9d-102">Απογραφή συσκευής Intune</span><span class="sxs-lookup"><span data-stu-id="d3d9d-102">Intune Device Inventory</span></span>

<span data-ttu-id="d3d9d-103">Η λεπίδα Συσκευών παρέχει στο διαχειριστή πληροφορίες για τις συσκευές που βρίσκονται υπό διαχείριση στο Intune ανά συσκευή.</span><span class="sxs-lookup"><span data-stu-id="d3d9d-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="d3d9d-104">Οι πληροφορίες που εμφανίζονται περιλαμβάνουν: Υλικό, Εφαρμογές που ανακαλύφθηκαν, Κατάσταση συμμόρφωσης συσκευής και κατάσταση ρύθμισης παραμέτρων συσκευής.</span><span class="sxs-lookup"><span data-stu-id="d3d9d-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="d3d9d-105">Τα δεδομένα απογραφής για το υλικό και τις εφαρμογές που έχουν ανακαλυφθεί συλλέγονται σε έναν κύκλο επτά ημερών.</span><span class="sxs-lookup"><span data-stu-id="d3d9d-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="d3d9d-106">Οι εφαρμογές και τα συγκεκριμένα στοιχεία του υλικού που αναφέρθηκαν διαφέρουν ανάλογα με το λειτουργικό σύστημα της συσκευής και αν η συσκευή ανήκει προσωπικά ή στην εταιρεία.</span><span class="sxs-lookup"><span data-stu-id="d3d9d-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="d3d9d-107">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Δείτε λεπτομέρειες συσκευής στο Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="d3d9d-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="d3d9d-108">**ΣΥΝΗΘΕΙΣ ΕΡΩΤΉΣΕΙΣ**</span><span class="sxs-lookup"><span data-stu-id="d3d9d-108">**FAQ**</span></span>

<span data-ttu-id="d3d9d-109">Ε: Δεν λαμβάνω πλήρη λίστα απογραφής των εφαρμογών που υπάρχουν σε συσκευές Windows που έχουν εγγραφεί στο Intune.</span><span class="sxs-lookup"><span data-stu-id="d3d9d-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="d3d9d-110">Γιατί όχι?</span><span class="sxs-lookup"><span data-stu-id="d3d9d-110">Why not?</span></span>

<span data-ttu-id="d3d9d-111">Α: Αυτήν τη στιγμή, μόνο οι σύγχρονες εφαρμογές παρατίθενται για υπολογιστές με Windows 10 που αναγνωρίζονται ως εταιρικές συσκευές.</span><span class="sxs-lookup"><span data-stu-id="d3d9d-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="d3d9d-112">Το Intune δεν συλλέγει πληροφορίες σχετικά με τις εφαρμογές Win32 που είναι εγκατεστημένες σε αυτές τις συσκευές.</span><span class="sxs-lookup"><span data-stu-id="d3d9d-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="d3d9d-113">Ε: Γιατί οι αριθμοί τηλεφώνου δεν συλλέγονται από όλες τις συσκευές;</span><span class="sxs-lookup"><span data-stu-id="d3d9d-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="d3d9d-114">Α: Τα τηλέφωνα που κατηγοριοποιούνται ως εταιρικές συσκευές στο Intune δεν αναγνωρίζονται με τον πλήρη αριθμό τηλεφώνου τους όταν, για παράδειγμα, εκτελείτε μια αναφορά απογραφής κινητής συσκευής.</span><span class="sxs-lookup"><span data-stu-id="d3d9d-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="d3d9d-115">Οι αριθμοί τηλεφώνου της συσκευής Bring-you-own είναι πάντα μερικώς καλυμμένοι με αστερίσκους (\*\*\*\*) και εμφανίζουν μόνο τα τελευταία τέσσερα ψηφία.</span><span class="sxs-lookup"><span data-stu-id="d3d9d-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>