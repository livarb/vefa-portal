+++

title = "EHF Invoice and Creditnote 2.0.5"
type = "standard"
status = "upcoming"

aliases = [ "/ehf/standard/ehf-invoice-and-creditnote-next/", "/ehf/standard/ehf-invoice-and-creditnote-2.0.next/" ]
current = "/ehf/standard/ehf-invoice-and-creditnote-current/"

[[resources]]
title = "Implementation guide (Norwegian)"
url = "https://github.com/difi/vefa-validator-conf/raw/updates-2015-10-01/STANDARD/EHFInvoice/2.0/guide/Implementeringsveileder%20EHF%20Fakturaprosess%20v2.0.pdf"

[[resources]]
title = "Implementation attachments (Norwegian)"
url = "https://github.com/difi/vefa-validator-conf/tree/updates-2015-10-01/STANDARD/EHFInvoice/2.0/guide/attachments-norwegian"

[[resources]]
title = "Implementation guide (English)"
url = "https://github.com/difi/vefa-validator-conf/raw/updates-2015-10-01/STANDARD/EHFInvoice/2.0/guide/Implementation%20Guide%20EHF%20Invoicing%20Process%20v2.0.pdf"

[[resources]]
title = "Implementation attachments (English)"
url = "https://github.com/difi/vefa-validator-conf/tree/updates-2015-10-01/STANDARD/EHFInvoice/2.0/guide/attachments-english"

[[resources]]
title = "Validator"
url = "https://test-vefa.difi.no/validator/"

[[resources]]
title = "Validation artifacts"
url = "https://github.com/difi/vefa-validator-conf/tree/updates-2015-10-01"

[[resources]]
title = "GEFEG for creditnote"
url = "https://test-vefa.difi.no/ehf/gefeg/creditnote/2.0/"

[[resources]]
title = "GEFEG for invoice"
url = "https://test-vefa.difi.no/ehf/gefeg/invoice/2.0/"

[[resources]]
title = "Github milestone"
url = "https://github.com/difi/vefa-validator-conf/issues?q=milestone%3A%22EHF+Invoice+and+Creditnote+2.0.5%22+is%3Aclosed%7Copen"

+++

## Changes since 2.0.4

Please monitor the Github milestone for more detailed information regarding changes.

### Missing example files (Files)

Examplefiles where removed in the latest hotfix, these will be added to the attachments again. 

### Payee Party (Guideline)

On page 18 in the guide the payee is referenced as "AccountingPayeeParty", this should be "PayeeParty". This reference will be corrected.

### Warning if elements are outside EHF specification, but exists in UBL (Validator)

Add vaildation that will generate warning if instance document is containing elements outside EHF specifications, but exist in UBL 2.1 schema (xsd).

### Empty elements generate error (Validator)

Empty elements will generate error, not warning as earlier revisions. This is according to chapter 3.3 in the guide.

### Attachments to the guide in Github will be un-zipped (Guideline)

Remove zip-files containing attachement to implementation guide on github, replaced by folder for easier access.

### Updated validation artefacts from OpenPEPPOL. (Validator)

OpenPEPPOL has done some changes/corrections to their validation artefacts, upgrade to use of xslt/xPath 2.0 and handling of numeric values as an example. These artefacts are used when validating both EHF files and PEPPOL BIS files. 
Detailed list of changes can be found on pages 10 and 11 in [overview document](/docs/ehf/20150820_updates_2015-10-01.pdf).

### Your ref. (Guideline)

Your reference is a mandatory element in EHF (cac:AccountingCustomerParty/cac:Party/cac:Contact/cbc:ID). If this information is not applicable for the invoice, the recommendation is to fill this element with the value "NA" (Not Applicable). This will be clarified in the guideline. 