+++

title = "ESPD attachment"
group = "Governance"
type = "article"

+++

Implementers of transactions may attach ESPD Request or ESPD response by adding a ```DocumentReference``` element. Special values to be used in addition to normal values for attachments:

```cac:DocumentReference/cbc:DocumentTypeCode```: 916 (Related document)

```cbc:DocumentDescription```: "ESPD Request" or "ESPD Response"
