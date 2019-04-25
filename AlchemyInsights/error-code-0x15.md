---
title: Κωδικός σφάλματος 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Αν λαμβάνετε ένα σφάλμα κατά την ενεργοποίηση του Office 2013 σε υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS) αναπτύξεις, εξετάστε το ενδεχόμενο να Ενεργοποίηση ADAL με επεξεργασία του μητρώου.
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402739"
---
<span data-ttu-id="fcf05-103">Αν λαμβάνετε ένα σφάλμα κατά την ενεργοποίηση του Office 2013 σε υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS) αναπτύξεις, εξετάστε το ενδεχόμενο να Ενεργοποίηση ADAL με επεξεργασία του μητρώου.</span><span class="sxs-lookup"><span data-stu-id="fcf05-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="fcf05-104">**Κλειδί μητρώου**</span><span class="sxs-lookup"><span data-stu-id="fcf05-104">**Registry key**</span></span>|<span data-ttu-id="fcf05-105">**Τύπος**</span><span class="sxs-lookup"><span data-stu-id="fcf05-105">**Type**</span></span>|<span data-ttu-id="fcf05-106">**Τιμή**</span><span class="sxs-lookup"><span data-stu-id="fcf05-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="fcf05-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="fcf05-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="fcf05-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="fcf05-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="fcf05-109">1</span><span class="sxs-lookup"><span data-stu-id="fcf05-109">1</span></span>  <br/> |
   
<span data-ttu-id="fcf05-110">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Ενεργοποίηση σύγχρονη ελέγχου ταυτότητας για το Office 2013 σε συσκευές των Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="fcf05-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="fcf05-111">ADAL είναι ενεργοποιημένη από προεπιλογή στο Office 365 ProPlus και Office 2016.</span><span class="sxs-lookup"><span data-stu-id="fcf05-111">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="fcf05-112">> Υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS) ήταν προηγουμένως με το όνομα των υπηρεσιών Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="fcf05-112">>  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

