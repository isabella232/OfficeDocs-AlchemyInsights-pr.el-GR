---
title: Υπηρεσία σύνδεσης Exchange εσωτερικής εγκατάστασης του Intune
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807649"
---
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="07aed-102">Υπηρεσία σύνδεσης Exchange εσωτερικής εγκατάστασης του Intune</span><span class="sxs-lookup"><span data-stu-id="07aed-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="07aed-103">Για λεπτομέρειες σχετικά με τη ρύθμιση της σύνδεσης μεταξύ του Intune και του Exchange που φιλοξενείται εσωτερικής εγκατάστασης, ανατρέξτε στην παρακάτω τεκμηρίωση:</span><span class="sxs-lookup"><span data-stu-id="07aed-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="07aed-104">Ρύθμιση της σύνδεσης του Exchange εσωτερικής εγκατάστασης του Intune στο Microsoft Intune Azure</span><span class="sxs-lookup"><span data-stu-id="07aed-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="07aed-105">**ΣΥΝΉΘΕΙς ΕΡΩΤΉΣΕΙς**</span><span class="sxs-lookup"><span data-stu-id="07aed-105">**FAQ:**</span></span>

<span data-ttu-id="07aed-106">Ε: εμφανίζεται ένα σφάλμα, όπως "η έκδοση σύνδεσης του Exchange δεν υποστηρίζεται" κατά την προσπάθεια ρύθμισης της σύνδεσης του Exchange.</span><span class="sxs-lookup"><span data-stu-id="07aed-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="07aed-107">Ποια θα μπορούσε να είναι η αιτία;</span><span class="sxs-lookup"><span data-stu-id="07aed-107">What could be the cause?</span></span>

<span data-ttu-id="07aed-108">Α: ο λογαριασμός που χρησιμοποιείτε έχει άδεια χρήσης κατάλληλα-πρέπει να έχει ενεργή άδεια χρήσης Intune</span><span class="sxs-lookup"><span data-stu-id="07aed-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="07aed-109">Ε: είναι δυνατόν να υπάρχουν πολλές γραμμές σύνδεσης του Exchange;</span><span class="sxs-lookup"><span data-stu-id="07aed-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="07aed-110">Α: μπορείτε να ρυθμίσετε μόνο μία σύνδεση Exchange ανά μισθωτή του Intune ανά οργανισμό του Exchange.</span><span class="sxs-lookup"><span data-stu-id="07aed-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="07aed-111">Η γραμμή σύνδεσης μπορεί να εγκατασταθεί μόνο σε ένα διακομιστή σε έναν οργανισμό πολλαπλών διακομιστών Exchange.</span><span class="sxs-lookup"><span data-stu-id="07aed-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="07aed-112">Επίσης, δεν μπορείτε να έχετε ρυθμισμένες γραμμές σύνδεσης τόσο για το Exchange εσωτερικής εγκατάστασης όσο και για το Exchange Online που έχει ρυθμιστεί στον ίδιο μισθωτή.</span><span class="sxs-lookup"><span data-stu-id="07aed-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="07aed-113">Ε: μπορεί η γραμμή σύνδεσης να χρησιμοποιήσει έναν πίνακα CAS ως σύνδεσή του με το Exchange;</span><span class="sxs-lookup"><span data-stu-id="07aed-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="07aed-114">Α: ο καθορισμός ενός πίνακα CAS δεν είναι υποστηριζόμενη ρύθμιση παραμέτρων στη ρύθμιση σύνδεσης.</span><span class="sxs-lookup"><span data-stu-id="07aed-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="07aed-115">Μόνο ένας διακομιστής πρέπει να καθοριστεί και θα πρέπει να καθορίζεται στο αρχείο ρύθμισης παραμέτρων σύνδεσης που μπορεί να βρεθεί στο</span><span class="sxs-lookup"><span data-stu-id="07aed-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="07aed-116">πρόγραμμα data\microsoft\microsoft Intune στη σύνδεση του Exchange εσωτερικής εγκατάστασης \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="07aed-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="07aed-117">Εντοπίστε την ακόλουθη καταχώρηση ```<ExchangeWebServiceURL />``` και αντικαταστήστε τη διεύθυνση URL με το διακομιστή Exchange.</span><span class="sxs-lookup"><span data-stu-id="07aed-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="07aed-118">**Παράδειγμα**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="07aed-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="07aed-119">Ανατρέξτε στην παρακάτω τεκμηρίωση για πρόσθετες αντιμετώπιση προβλημάτων: [Αντιμετώπιση προβλημάτων της σύνδεσης του Exchange εσωτερικής εγκατάστασης του Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="07aed-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="07aed-120">**Ενεργοποίηση της λεπτομερούς καταγραφής για τη σύνδεση του Exchange**</span><span class="sxs-lookup"><span data-stu-id="07aed-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="07aed-121">Ανοίξτε το αρχείο ρύθμισης παραμέτρων ανίχνευσης σύνδεσης του Exchange για επεξεργασία.</span><span class="sxs-lookup"><span data-stu-id="07aed-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="07aed-122">Το αρχείο βρίσκεται στη διεύθυνση:%ProgramData%\Microsoft\Windows του Exchange Intune Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="07aed-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="07aed-123">**Παράδειγμα**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="07aed-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="07aed-124">Εντοπίστε το TraceSourceLine με το ακόλουθο κλειδί: OnPremisesExchangeConnectorService</span><span class="sxs-lookup"><span data-stu-id="07aed-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="07aed-125">Αλλαγή της τιμής κόμβου SourceLevel από τις πληροφορίες ActivityTracing (προεπιλογή) σε λεπτομερή ActivityTracing</span><span class="sxs-lookup"><span data-stu-id="07aed-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="07aed-126">**Παράδειγμα**</span><span class="sxs-lookup"><span data-stu-id="07aed-126">**Example:**</span></span>
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. <span data-ttu-id="07aed-127">Επανεκκινήστε την υπηρεσία Microsoft Intune Exchange</span><span class="sxs-lookup"><span data-stu-id="07aed-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="07aed-128">Πλήρης συγχρονισμός στην πύλη του Intune μέχρι να ολοκληρωθεί και, στη συνέχεια, αλλάξτε ξανά την XML σε "πληροφορίες ActivityTracing" και επανεκκινήστε την υπηρεσία Microsoft Intune Exchange.</span><span class="sxs-lookup"><span data-stu-id="07aed-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="07aed-129">Η θέση των αρχείων καταγραφής είναι: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="07aed-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>