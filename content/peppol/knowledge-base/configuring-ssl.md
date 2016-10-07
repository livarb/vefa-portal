+++

title = "Configuring SSL"
group = "Security"
type = "article"

+++

Providers may choose any suitable application to terminate SSL, so Difi can't provide guides on how to configure the various applications.

To validate SSL configuration, we suggest using this tool:

* [SSL Server Test (Powered by Qualys SSL Labs)](https://www.ssllabs.com/ssltest/analyze.html)

This is the minimal required values to verify in the validation tool:

* Trusted: **Yes**
* Chain issues: **None**

We urge all providers to qualify for grade "A" or better.

For testing of access points running a different port than 443, may use [DigiCert SSL Installation Diagnostics Tool](https://www.digicert.com/help/) to get a hint of status.
