+++

title = "EHF Despatch Advice 1.0.2"
type = "standard"
status = "deprecated"

current = "/ehf/standard/ehf-despatch-advice-current/"

[[resources]]
title = "Implementation guide (Norwegian)"
url = "https://github.com/difi/vefa-validator-conf/raw/dc4c01bcf3782a3578ff8cd2ef0565919eb7e40f/STANDARD/EHFDespatchAdvice/1.0/guide/Implementeringsveileder%20EHF%20Pakkseddel%20v1.0.2.pdf"

[[resources]]
title = "Implementation attachments (Norwegian)"
url = "https://github.com/difi/vefa-validator-conf/tree/dc4c01bcf3782a3578ff8cd2ef0565919eb7e40f/STANDARD/EHFDespatchAdvice/1.0/guide/attachments-norwegian"

[[resources]]
title = "Implementation guide (English)"
url = "https://github.com/difi/vefa-validator-conf/raw/dc4c01bcf3782a3578ff8cd2ef0565919eb7e40f/STANDARD/EHFDespatchAdvice/1.0/guide/ImplementationGuide%20EHF%20DespatchAdvice%20v1.0.2.pdf"

[[resources]]
title = "Implementation attachments (English)"
url = "https://github.com/difi/vefa-validator-conf/tree/dc4c01bcf3782a3578ff8cd2ef0565919eb7e40f/STANDARD/EHFDespatchAdvice/1.0/guide/attachments-english"

[[resources]]
title = "Validation artefacts"
url = "https://github.com/difi/vefa-validator-conf/tree/dc4c01bcf3782a3578ff8cd2ef0565919eb7e40f"

[[resources]]
title = "Github milestone"
url = "https://github.com/difi/vefa-validator-conf/issues?q=milestone%3A%22EHF+Despatch+Advice+1.0.2%22+is%3Aclosed%7Copen"

+++

## Changes since 1.0.1

Please monitor the Github milestone for more detailed information regarding changes.

### Warning if elements are outside EHF specification, but exists in UBL (Validator)

Add vaildation that will generate warning if instance document is containing elements outside EHF specifications, but exist in UBL 2.1 schema (xsd).

### Warning if elements are outside PEPPOL specification, but exists in UBL (Validator)

Add vaildation that will generate warning if instance document is containing elements outside PEPPOL BIS, but exist in UBL 2.1 schema (xsd).

### Empty elements generate error (Validator)

Empty elements will generate error, not warning as earlier revisions. This is according to chapter 3.3 in the guide.

### Attachments to the guide in Github will be un-zipped (Guideline)

Remove zip-files containing attachement to implementation guide on github, replaced by folder for easier access.

### Updated validation artefacts from OpenPEPPOL (Validator)

OpenPEPPOL has done some changes/corrections to their validation artefacts, upgrade to use of xslt/xPath 2.0 and handling of numeric values as an example. These artefacts are used when validating both EHF files and PEPPOL BIS files.
Detailed list of changes can be found on pages 10 and 11 in [overview document](/docs/ehf/20150820_updates_2015-10-01.pdf).
