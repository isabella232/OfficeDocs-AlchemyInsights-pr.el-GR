---
title: 1048 5.7.750 Η υπηρεσία δεν είναι διαθέσιμη. Το πρόγραμμα-πελάτης αποκλείστηκε από την αποστολή από μη καταχωρημένους τομείς
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 48b9c2de27f8d7f52215c3a3d547bdf746a3a4cd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676713"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="b0c40-103">5.7.750 Πελάτης που έχει αποκλειστεί από την αποστολή από μη καταχωρημένο τομέα</span><span class="sxs-lookup"><span data-stu-id="b0c40-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="b0c40-104">Το σφάλμα παρουσιάζεται όταν ένας μεγάλος όγκος μηνυμάτων αποστέλλεται από τομείς που δεν έχουν προβλεφθεί στον μισθωτή σας (προστίθενται ως αποδεκτοί τομείς και επικυρώνονται).</span><span class="sxs-lookup"><span data-stu-id="b0c40-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="b0c40-105">Για να αποφύγετε αυτό το σφάλμα, μπορείτε να χρησιμοποιήσετε μια σύνδεση ροής αλληλογραφίας που βασίζεται σε πιστοποιητικό, όπου ο τομέας του πιστοποιητικού είναι τομέας που έχει προμήθεια ή μπορείτε να προβλέψετε όλους τους τομείς αποστολής.</span><span class="sxs-lookup"><span data-stu-id="b0c40-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
