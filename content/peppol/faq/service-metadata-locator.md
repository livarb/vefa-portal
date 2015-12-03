+++

title = "FAQ: Service Metadata Locator (SML)"
linktitle = "Service Metadata Locator (SML)"
type = "faq"

+++

## What is a SML?

SML is a **central service** to locate the Service Metadata Provider (SMP) where a given participant may be found.

## How many SMLs exists?

For a given network may only **one** SML exist. PEPPOL is such a network containing only one SML.

## How many SMPs may register a participant in SML?

SML points to **one** SMP containing metadata for a given participant. Trying to register a participant registred by another SMP results in error.

## What is the address of SML?

SML doesn't provide a user interface. For location is the hostname "edelivery.tech.ec.europa.eu" used for lookup in PEPPOL.

## What is SMK?

SMK is a SML for test purposes. Hostname for SMK in PEPPOL is "acc.edelivery.tech.ec.europa.eu".

## Who administrate registration in SML?

Providers providing SMP services are the only administrators of SML.