---
title: Λήψη λίστας εταιρικών εφαρμογών
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
- "9004342"
- "9837"
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404932"
---
# <a name="get-a-list-of-enterprise-applications"></a>Λήψη λίστας εταιρικών εφαρμογών

1. Για να λάβετε **μια** λίστα των εταιρικών εφαρμογών (όλες οι εφαρμογές ή φιλτραρισμένο κατά εμφανιζόμενο όνομα, αναγνωριστικό, διευθύνσεις URL αναγνωριστικού κ.λπ.) μέσω της εντολής Powershell, ανατρέξτε στο θέμα [Get-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)
2. Για να λάβετε μια λίστα με τα κύρια αντικείμενα υπηρεσίας (όλα τα αντικείμενα ή φιλτραρισμένο κατά αναγνωριστικό) μέσω της εντολής Powershell, ανατρέξτε στο θέμα [Get-AzureADServicePrincipal (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)
3. Εάν θέλετε να λάβετε μια **λίστα με τις ρυθμισμένες εφαρμογές SAML, οι ακόλουθες δέσμες ενεργειών του PowerShell μπορεί** να σας βοηθήσουν:

    Κάθε εφαρμογή είτε είναι μια εφαρμογή OAuth είτε μια εφαρμογή SAML (εφαρμογές συλλογής και εφαρμογές που δεν είναι συλλογή) θα έχουν δύο αντικείμενα που δημιουργούνται στο AAD όταν συμβεί η εγγραφή τους. Το ένα ονομάζεται αντικείμενο εφαρμογής και το άλλο είναι το αντικείμενο Service Principal. Όταν τοποθετείτε σε απόρριψη τις ιδιότητες ενός κύριου αντικειμένου υπηρεσίας χρησιμοποιώντας το PowerShell, θα βρείτε ότι κάθε εφαρμογή έχει έναν συγκεκριμένο αριθμό ετικετών που σχετίζονται με αυτό, όπως:

    - Οι εφαρμογές OAuth θα έχουν μια ετικέτα που ονομάζεται "**WindowsAzureActiveDirectoryIntegratedApp**"
    - Οι εφαρμογές SAML συλλογής θα έχουν μια ετικέτα που ονομάζεται "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"
    - Οι εφαρμογές SAML που δεν είναι συλλογής θα έχουν μια ετικέτα που ονομάζεται "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"

    Ως εκ τούτου, μπορείτε να χρησιμοποιήσετε αυτές τις ετικέτες και να μάθετε τι είδους εφαρμογή είναι. Η ετικέτα **"WindowsAzureActiveDirectoryIntegratedApp"** είναι συνηθισμένη σε όλους τους τύπους εφαρμογών. Μπορείτε να χρησιμοποιήσετε το ακόλουθο τμήμα για να παρατίθενται όλες οι εφαρμογές SAML (συλλογή και μη συλλογή):

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Αναγνώριση εφαρμογών με δυνατότητα SAML στο Azure AD.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)

4. **Εύρεση και λίστα μόνο εφαρμογών Web:** Χρησιμοποιήστε την παρακάτω εντολή για να λάβετε όλες τις εφαρμογές Azure AD με τον τύπο εφαρμογής "Εφαρμογή Web/API"

    Get-AzureADApplication -Όλα:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Εύρεση και λίστα εγγενών εφαρμογών** μόνο: Εκτελέστε την ακόλουθη εντολή για να λάβετε όλες τις εγγενείς εφαρμογές προγράμματος-πελάτη (υπολογιστή/κινητής συσκευής).

    Get-AzureADApplication -Όλα:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. **Εξαγωγή όλων των καταχωρημένων λεπτομερειών εφαρμογής Azure AD στο CSV:** Η παρακάτω εντολή εξάγει όλες τις εφαρμογές Azure AD με απαιτούμενες λεπτομέρειες στο αρχείο csv:

    - Get-AzureADApplication -Όλα:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Κωδικοποίηση UTF8

7. **Πρέπει να εξαγάγετε μια λίστα των εφαρμογών Azure που δεν τίθενται σε χρήση** – Αναφορά ελέγχου

    Το Azure AD μπορεί να εμφανίζει αρχεία καταγραφής εφαρμογών μόνο για έως και 30 ημέρες, με την προϋπόθεση ότι έχετε άδεια χρήσης Azure AD Premium.
    Έχετε δύο επιλογές για να διατηρήσετε τα δεδομένα για περισσότερο από 30 ημέρες. Μπορείτε να χρησιμοποιήσετε τα [API αναφοράς AZURE AD για](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) να ανακτήσετε τα δεδομένα μέσω προγραμματισμού και να τα αποθηκεύσετε σε μια βάση δεδομένων. Εναλλακτικά, μπορείτε να ενσωματώσετε αρχεία καταγραφής ελέγχου σε ένα σύστημα SIEM άλλου κατασκευαστή.

    Μπορείτε επίσης να κάνετε λήψη της λίστας εφαρμογών για όλες τις εφαρμογές και τις εφαρμογές που ανήκουν στο Azure Active Directory>Καταχωρήσεις εφαρμογών>Λήψη>Όλες οι εφαρμογές/οι εφαρμογές που ανήκουν.

    Για να λάβετε μια λίστα εφαρμογών μέσω του MS Graph, ανατρέξτε στο θέμα Εφαρμογές λίστας [- Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) και τύπος πόρου [εφαρμογής - Microsoft Graph v1.0.](https://docs.microsoft.com/graph/api/resources/application)
