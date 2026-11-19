# Indicators of Compromise (IOCs)

| Indicator | Observation |
|  ------   |   -------   |
| Sender Domain | `micros0ft-support.example` |
| Sender Address | `security-alert@micros0ft-support.example` |
| Suspicious URL | `http://micros0ft-support.example/verify` |
| Email Subject | Urgent! Your Microsoft account will be suspended. |
| Authentication | SPF: Fail, DKIM: None, DMARC: Fail |

## Key Observations
- Domain impersonates Microsoft using a zero instead of the letter O.
- Email uses urgency to pressure the recipient.
- Authentication results indicate potential email spoofing.

