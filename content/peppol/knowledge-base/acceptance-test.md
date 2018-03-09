+++

title = "Acceptance test"
group = "Governance"
type = "article"

+++

Testing is performed to ensure the introduction of a new provider in the network will not cause instability and problems.


## Prerequisites

The following steps must be done according to the [Governance model](/peppol/knowledge-base/governance-model/):

1. Apply for OpenPEPPOL Membership.
1. Sign and send the Transport Infrastructure Agreement (TIA) to your PEPPOL Authority.

The provider subject to testing will receive enrolment information from their PEPPOL Authority to generate the certificate in the OpenPEPPOL TEST PKI chain.

The generated certificate must be installed in the Access Point of choice.

**Tips** Make sure to do self-testing before initiating the acceptance test.  The provider is free to use the [Access point (test)](/peppol/tools/ap-test/) provided by Difi to perform self-testing.

Providers deemed not ready for acceptance testing will be asked to restart when ready.


## Configuration

Providers using [Oxalis 3.x](/peppol/tools/oxalis/) must update oxalis-global.properties to contain these values:

```
oxalis.pki.version=V2
oxalis.operation.mode=TEST
oxalis.sml.hostname=acc.edelivery.tech.ec.europa.eu
```

Other products must be configured accordingly.


## Performing acceptance test

Acceptance testing is performed using an Access Point configured for production with a test certificate (only after successful testing, switching the certificate from test certificate to production certificate should be required to go into production).

Please notice:

* A Difi notification that the test has ended due to lack of activity means you need to start at Step 1 again - by sending the test initiation memo. Such a notification is normally sent after one week of inactivity.

* Acceptance testing is performed step by step. Any action performed for upcoming steps before receiving notification from Difi to continue are seen as self-testing and is not accepted as part of acceptance testing.


### Step 0: Checklist

Make sure to be ready to perform testing when contacting Difi. Please use this checklist:

* The AP MUST [implement HTTPS](/peppol/knowledge-base/configuring-ssl/) with certificate chains to certificate authorities which would be considered to be trusted by the PEPPOL community.

* The AP URL MUST only refer to HTTPS.

* The AP URL SHOULD use the default port 443. This assures firewall rules are often setup in advance.

* The AP MUST be accessible over the Internet.

Due to occasionally heavy demand on performing acceptance testing, Difi cannot promise completed testing unless the Access Point is deemed ready for testing minimum two weeks before deadline. During Norwegian holiday seasons, testing may take more than 2 weeks.


### Step 1: Inform Difi

Before testing starts, make sure to inform Difi by sending mail to [ap@difi.no](mailto:ap@difi.no) containing this information:

* Who performs the test?
* Contact information
* URL to AS2 endpoint of access point
* File containing OpenPEPPOL AP certificate **(Do not send private key!)**
* Specify the PEPPOL Authority (PA) chosen

Please use this subject: *"AP Acceptance testing: [Your company name]"*

To be checked by Difi before next step:

* Information sent as specified above.
* AP is online and responding when connecting using HTTPS on port 443.
* HTTPS is configured to provide an **A** score using [SSL Server Test](https://www.ssllabs.com/ssltest/). Any remarks must be clarified by the AP provider.


### Step 2: Send document to Difi

Send a document of your choice to [9908:810418052](https://test-vefa.difi.no/smp/9908/810418052). Find your transmission in [the list of transmissions](/peppol/tools/ap-test/) and send the URL pointing to the transmission to be used for verification to [ap@difi.no](mailto:ap@difi.no).

To be checked by Difi before next step:

* Verify receipt of document.
* Checking the received document in general.
* Verifying correct use of SBDH based on document sent.


### Step 3: Receive document from Difi

Difi will send a document of choice to the Access Point.  The provider will receive a mail with a question regarding the content - to confirm successful sending.

Providers do not need to register any recipients in the SMP/SMK to be ready for this step.

To be checked by Difi before next step:

* Checking MDN received from AP provider.
* Verifying AP provider is able to reproduce information to uniquely verify receipt of document.


## Step 4: Send test report

Provider subject to testing must use results from testing to complete a [test report](/docs/peppol/aptest.xlsx) and send it to [ap@difi.no](mailto:ap@difi.no) within one week from completing testing.

To be checked by Difi before sending recommendation to the PA:

* Report is according to actual acceptance test.
* All responses to be acceptable for AP providers to be part of the OpenPEPPOL network.

Upon receiving the accepted report from Difi, the PA will trigger enrolment to generate the certificate in the OpenPEPPOL PRODUCTION PKI chain to become available to the provider.
