# Phishing Email Investigation Report

## 1. Objective
To investigate a simulated phishing email and identify suspicious indicators using email security tools.

## 2. Email Details
- **Sender:** security-alert@micros0ft-support.example
- **Subject:** Urgent! Your Microsoft account will be suspended.
- **Suspicious link:** `http://micros0ft-support.example/verify`

## 3. Findings

**Email Indicators**
- Fake Microsoft-like domain (`micros0ft`).
- Urgent language and account suspension threat.
- Suspicious verification link.

**VirusTotal**
- Tested a separate Google Safe Browsing test URL.
- 3 vendors flagged it; 52 marked it clean; 25 were unrated.
- Different vendors can produce different results.

**IP Investigation**
- IP: `172.217.214.153`
- Organization: Google LLC
- ASN: 15169

**Email Authentication**
| SPF | DKIM | DMARC |
| --- |  --- |  ---  |
| Fail| none | Fail |

**MXToolbox**
- Analyzed a simulated email header.
- Authentication checks showed failures.
- Blacklist section displayed a green tick.

## 4. Conclusion
The simulated email shows multiple phishing indicators, including domain impersonation, urgency, and failed email authentication.

**Assessment:** Suspected phishing (training scenario).

## 5. Tools Used
- VirusTotal
- MXToolbox Email Header Analyzer

## 6. Security Recommendations
- Avoid clicking suspicious links.
- Verify messages through official websites.
- Report suspicious emails.
- Use SPF, DKIM, and DMARC for email protection.

