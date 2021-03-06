+++

title = "Implementing invoice"
type = "starter"

groups = ["shortcuts"]

+++

**Correct implementation of EHF gives the best result, and the most satisfied customers. This is the recipe.**

The implementation guide may be seen as the bible when implementing EHF. Implementation guides defines the standard, and implementations implementing the implementation guide will be backward compatible when validation artefacts are updated.

For invoice, make sure to use the latest version of [EHF Invoice and Creditnote 2.0.x](/ehf/standard/ehf-invoice-and-creditnote-2.0.current/) guide. The guide includes attachments containing example files, structure tables and message tables.

EHF uses [Universal Business Language (UBL)](/ehf/standard/ubl/) for syntax, and EHF Invoice and Creditnote 2.0.x uses UBL version 2.1. Those implemeting invoice using Java may note the availability of [Java bindings on Maven Central](http://mvnrepository.com/artifact/no.difi.commons/commons-ubl21), others may find XSD files on the UBL homepage (click "Version 2.1").

Receivers may support different CEN/BII Profiles. A [Java lookup client](/peppol/tools/vefa-peppol/) is provided to determine the receivers supported document identifiers.

Difi provides [validation services](/ehf/tools/validation-service/) intended to support development of EHF. Validation services will never be able to validate all aspects of documents, so make sure to implement according to implementation guides even when errors and warnings are not triggered in the validator as this may change later.

Implementers of EHF Invoice and Creditnote should expect new versions to be made available. EHF has it's own [release management](/ehf/knowledge-base/release-management/), and new versions are announced as soon as possible. Full changelog for new versions is found in the implementation guide.
