+++

title = "Validation"
group = "Quality"
type = "article"

+++

Difi provides [two validation services](/ehf/tools/validation-service/) for validation of EHF documents. One services provides validation using the current set of rules and one provides validation using the upcoming set of rules.

The validation services as provided by Difi allows for upload of file for validation, and may be used for manual test and verification. Files uploaded are stored for a limited time, and every validation receives a unique URI. Please share related URI with Difi when contacting [support](/support/) regarding errors in validator.

Specially during review of [new releases](/ehf/knowledge-base/release-management/) may validation using the upcoming set of rules be important to discover problems caused by the rules or by your own implementation.

Difi provides an [open source library for validation](https://vefa.difi.no/ehf/tools/validation-library/) with functionality to download updated rules directly from Difi servers. Difi encourage vendors to use the library as part of their own toolchain. Vendors may expect uptime of Difi servers to be ~99%, so storing rules locally is recommended for production environments.

Any errors detected in the library may be reported as issues using [Github Issues](https://github.com/difi/vefa-validator/issues).