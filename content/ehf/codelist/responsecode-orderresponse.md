+++

title = "Response Code (OrderResponse)"
type = "codelist"

documenttypes = ["OrderResponse"]
source = "UN/ECE 1225"
subset = "PEPPOL"
xpath = ["cbc:OrderResponseCode","cac:OrderLine/cac:LineItem/cbc:LineStatusCode"]
listid = "UNCL1225"

+++

| Code | Description                               |
| ---- | ----------------------------------------- |
| 27   | Not Accepted                              |
| 29   | Accepted                                  |
| 30   | Accepted with amendment in detail section |
