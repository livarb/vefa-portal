+++

title = "Implementing invoice"
type = "starter"

+++

**Correct implementation of EHF gives the best result, and the most satisfied customers. This is the recipe.**

The implementation guide may be seen as the bible when implementing EHF. Implementation guides defines the standard, and implementations implementing the implementation guide will be backward compatible when validation artefacts are updated.

For invoice, the make sure to use the latest version of [EHF Invoice and Creditnote 2.0.x](/ehf/standard/ehf-invoice-and-creditnote-2.0.current/). The guide include attachments containing example file, structure tables and message table.

EHF uses [Universal Business Language (UBL)](/ehf/standard/ubl/) for syntax, and EHF Invoice and Creditnote 2.0.x uses UBL version 2.1. Those implemeting invoice using Java may note the availability of Java bindings on Maven Central, others may find XSD files on the UBL homepage (click "Version 2.1").

Receivers may support different CEN/BII Profiles. In [VEFA PEPPOL](/peppol/tools/vefa-peppol/) may the (Java) lookup client be used to determine supported document identifiers by the receiver.

Difi provides [validation services](/ehf/tools/validation-service/) intended to support development of EHF. Validation services will never be able to validate all aspects of documents, so make sure to implement according to implementation guides even when errors and warnings are not triggered in the validator as this may change later.

Implementers of EHF Invoice and Creditnote should expect new versions to be made available. EHF has it's own [release management](/ehf/knowledge-base/release-management/), and new versions are announced as soon as possible. Full changelog for new versions is found in the implementation guide.
