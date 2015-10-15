+++

title = "FAQ: Validation"
linktitle = "Validation"
type = "faq"

+++

## Where do I find the validation service?

Please see the [validation service](/ehf/tools/validation-service/) page for information regarding location of the validation service.

## My document is validated without errors, is it valid?

The validator are able to perform a technical validation so your document may be technically valid, but the document is not valid unless it's also semantically correct according to the implementation guide.

## How can I change the rules my document is validated against?

Documents are declared by using the elements CustomizationId and ProfileId. The declaration is used to determine the rules to use. Make sure to redeclare your document if you want to change the rules used for validation.

## I'm receiving fewer warnings/errors in the validation service than locally in my editor, what is wrong?

The config.xml file in the validation artifacts declare what rules are used. EHF filters some rules in the declaration of the validation artifacts. Please consult the config.xml and/or the list of rules in the implementation guide.

## What SLA is expected for the Difi validator?

The Difi validator is served at a best effort basis.

## May I use the Difi validator for production data?

Using the service for production data is not allowed, and will result in blocking of IPs.
