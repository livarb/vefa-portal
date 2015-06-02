+++

date = "2015-06-09"
title = "SML migration"
type = "event"

+++

This change will impose need for changes in configuration of services and potentially updates to available versions of CIPA/Oxalis or the deployed configuration of other implementations.

The transfer of services includes changes in the domain names used for SML and impacts all PEPPOL Service Providers both Access Points Services and SMP.

New domains:

* SML: edelivery.tech.ec.europa.eu
* SMK: acc.edelivery.tech.ec.europa.eu

Timeline for Access Points June 9th 2015:

* 09:00 CEST - Blocking updates to old SML
* 14:00 CEST - All providers change to use new SML

Between 09:00 CEST and 14:00 CEST will the old SML respond as usual. While SML is blocking updates is also ELMA blocked for adding/removing participants.

If you are using **Oxalis (version 3.0 or newer)**, make sure to add this line to **oxalis-global.proerties** and restart all services using Oxalis configuration: 
oxalis.sml.hostname=edelivery.tech.ec.europa.eu

**Oxalis 2.x is not supported**, and there are no upgrade path provided for upgrading Oxalis 2.x to use the new SML/SMK.
