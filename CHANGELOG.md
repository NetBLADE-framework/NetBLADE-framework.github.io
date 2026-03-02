# v2025

## Phases

### New
- None

### Updated
- `Actions on the Objective`: Minor wording changes.

### Retired
- None

## Tactics

### New
- `TAC-25 Accessibility Options Abuse`
- `TAC-26 Impersonation`
- `TAC-27 Session Manipulation`
- `TAC-28 Queue Bypass`
- `TAC-29 Session Transfer`
- `TAC-30 Bonus Farming`
- `TAC-31 AI Model Training`
- `TAC-32 Geo-Location Spoofing`
- `TAC-33 Device Emulation`
- `TAC-34 Attack Surface Identification`
- `TAC-35 Fake Credibility Generation`
- `TAC-36 Specific Target Scraping`
- `TAC-37 Loose Target Scraping`
- `TAC-38 Identity Acquisition`
- `TAC-39 Inventory Manipulation`
- `TAC-40 Add to Cart`
- `TAC-41 Account Enumeration`
- `TAC-42 Payment Card Enumeration`
- `TAC-43 Information Release`


### Updated
- `TAC-02 Credential Acquisition`: Minor wording changes.
- `TAC-03 Infrastructure Acquisition`: Minor wording changes.
- `TAC-04 Payment Detail Acquisition`: Minor wording changes.
- `TAC-08 Mitigation Bypass` -> `TAC-08 CAPTCHA Bypass`: Renamed.
- `TAC-10 Proxying`: Major wording changes.
- `TAC-12 Account Creation`: Minor wording changes.
- `TAC-15 Stock Purchase` -> `TAC-15 Purchase`: Major wording changes. Renamed.
- `TAC-20 Transaction Redirect` -> `TAC-20 Cashout`: Major wording changes. Renamed.
- `TAC-21 Exfiltration` -> `TAC-21 Data Extraction`: Renamed.


### Retired
- `TAC-06 Specific Target`: Replaced by `TAC-36 Specific Target Scraping`
- `TAC-07 Loose Target`: Replaced by `TAC-37 Loose Target Scraping`
- `TAC-16 Spinning`
- `TAC-17 Sniping`

## Techniques

### New
- `TEQ-081 Accessibility Downgrade`
- `TEQ-082 Session Persistence`
- `TEQ-083 Session Reassumption`
- `TEQ-084 Queue Flooding`
- `TEQ-085 Queue Position Tracking`
- `TEQ-086 Queue Jumping`
- `TEQ-087 Queue Evasion`
- `TEQ-088 Session Spoofing`
- `TEQ-089 Queue Position Transfer`
- `TEQ-090 Referral Program Exploitation`
- `TEQ-091 Clickjacking`
- `TEQ-092 Bonus Clipping`
- `TEQ-093 LLM Training Data`
- `TEQ-094 LAM Training Data`
- `TEQ-095 GPS Spoofing`
- `TEQ-096 Mobile Network Spoofing`
- `TEQ-097 Accept-Language Manipulation`
- `TEQ-098 TLS Spoofing`
- `TEQ-099 Header Spoofing`
- `TEQ-100 Path Enumeration`
- `TEQ-101 Endpoint Enumeration`
- `TEQ-102 Fake Account Creation`
- `TEQ-103 Queue Exhaustion`
- `TEQ-104 Queue Entry`
- `TEQ-105 Account Ageing`
- `TEQ-106 Fuzzing`
- `TEQ-107 Synthetic Account Creation`
- `TEQ-108 Impersonated Account Creation`
- `TEQ-109 Inventory Exhaustion`
- `TEQ-110 Mass Add to Cart`
- `TEQ-111 Loyalty Points Redemption`
- `TEQ-112 Deepfakes`
- `TEQ-113 Credit/Debit Card Cracking`
- `TEQ-114 Gift Card Cracking`
- `TEQ-115 Intellectual Property Leak`
- `TEQ-116 Inventory Information Extraction`
- `TEQ-117 Credential Extraction`
- `TEQ-118 Payment Detail Extraction`
- `TEQ-119 PII Extraction`
- `TEQ-120 Intellectual Property Extraction`

### Updated
- `TEQ-002 URL Disguise`: Minor wording changes.
- `TEQ-003 Data Dumps`: Added `TAC-38 Identity Acquisition` as parent.
- `TEQ-004 Malware` -> `TEQ-004 Infostealer`: Major wording changes. Renamed.
- `TEQ-005 Person in the Middle`: Minor wording changes.
- `TEQ-008 Botnet`: Minor wording changes. Removed `TAC-10 Proxying` as parent.
- `TEQ-011 Supply Chain Compromise` -> `TEQ-011 Trusted Infrastructure`: Major wording changes. Renamed.
- `TEQ-015 Continual Content Scraping`: Removed `TAC-06 Specific Target` and `TAC-07 Loose Target` as parents and replaced with `TAC-36 Specific Target Scraping` and `TAC-37 Loose Target Scraping`.
- `TEQ-018 CAPTCHA Farm`: Minor wording changes.
- `TEQ-020 Token Bypass`: Removed `TAC-08 Mitigation Bypass` as parent and replaced with `TAC-27 Session Manipulation`.
- `TEQ-021 Cookie Abuse`: Removed `TAC-08 Mitigation Bypass` as parent and replaced with `TAC-27 Session Manipulation`.
- `TEQ-022 Accessibility Options Abuse` -> `TEQ-022 Accessibilty Feature Abuse`: Minor wording changes. Renamed. Removed `TAC-08 Mitigation Bypass`, `TAC-09 Human Emulation` and `TAC-14 Fake Interaction` as parents and replaced with `TAC-25 Accessibility Option Abuse`.
- `TEQ-023 MFA Bypass`: Removed `TAC-08 Mitigation Bypass` as parent and replaced with `TAC-26 Impersonation`.
- `TEQ-024 Credential Pinning`: Removed `TAC-08 Mitigation Bypass` as parent and replaced with `TAC-26 Impersonation`.
- `TEQ-025 Certificate Abuse`: Removed `TAC-08 Mitigation Bypass` as parent and replaced with `TAC-27 Session Manipulation`.
- `TEQ-027 User Agent Spoofing`: Minor wording changes. Removed `TAC-09 Human Emulation` and `TAC-10 Proxying` as parents and replaced with `TAC-33 Device Emulation`.
- `TEQ-028 Device Fingerprint Emulation` -> `TEQ-028 Device Configuration Emulation`: Minor wording changes. Renamed. Removed `TAC-09 Human Emulation` as parent and replaced with `TAC-33 Device Emulation`.
- `TEQ-029 Notification Hijack`: Removed `TAC-14 Fake Interaction` as parent.
- `TEQ-030 IP Rotation`: Added `TAC-32 Geolocation Spoofing` as parent.
- `TEQ-033 Smurfing` -> `TEQ-033 Multi-Accounting`: Renamed.
- `TEQ-036 Social Media Creation`: Major wording changes. Removed `TAC-12 Account Creation` as parent and replaced with `TAC-38 Identity Acquisition`.
- `TEQ-037 Email Generator`: Removed `TAC-12 Account Creation` as parent and replaced with `TAC-38 Identity Acquisition`.
- `TEQ-038 Call/SMS Generator`: Removed `TAC-12 Account Creation` as parent and replaced with `TAC-38 Identity Acquisition`.
- `TEQ-039 Virtual Wallet Creation`: Removed `TAC-12 Account Creation` as parent and replaced with `TAC-38 Identity Acquisition`.
- `TEQ-040 Credential Cracking`: Minor wording changes.
- `TEQ-041 Credential Stuffing`: Added `TAC-41 Account Enumeration` as parent.
- `TEQ-045 Written Interaction` -> `TEQ-045 Content Posting`: Minor wording changes. Renamed.
- `TEQ-047 Form Filling` -> `TEQ-047 Form Submission`: Major wording changes. Renamed.
- `TEQ-049 Automated Add to Cart`: Removed `TAC-15 Stock Purchase`, `TAC-16 Spinning` and `TAC-10 Sniping` as parents and replaced with `TAC-40 Add to Cart`.
- `TEQ-050 Automated Purchase`: Removed `TAC-16 Spinning` and `TAC-10 Sniping` as parents.
- `TEQ-051 Stock Price Manipulation` -> `TEQ-051 Price Manipulation`: Minor wording changes. Renamed.
- `TEQ-053 Inventory Hoarding`: Major wording changes. Removed `TAC-16 Spinning` as parent and replaced with `TAC-39 Inventory Manipulation`.
- `TEQ-054 Transfer of Cart`: Removed `TAC-16 Spinning` as parent and replaced with `TAC-29 Session Transfer`.
- `TEQ-055 Automated Sale`: Major wording changes. Removed `TAC-16 Spinning` and `TAC-17 Sniping` as parents.
- `TEQ-056 Automated Bid`: Major wording changes. Removed `TAC-17 Sniping` as parent and replaced with `TAC-15 Purchase`.
- `TEQ-061 Credit/Debit Card Abuse`: Minor wording changes.
- `TEQ-062 Gift Card Abuse`: Major wording changes.
- `TEQ-063 Loyalty Points Abuse`: Minor wording changes.
- `TEQ-061 Buy Now Pay Later Abuse`: Major wording changes.
- `TEQ-065 ATS Fraud` -> `TEQ-065 Bank Transfer`: Renamed.
- `TEQ-066 Automated Advertisement of Stock` -> `TEQ-066 Inventory Information Release`: Minor wording changes. Renamed. Removed `TAC-21 Exfiltration` as parent and replaced with `TAC-43 Information Release`
- `TEQ-067 Credential Dumping`: Major wording changes. Removed `TAC-21 Exfiltration` as parent and replaced with `TAC-43 Information Release`
- `TEQ-069 Payment Detail Dumping`: Removed `TAC-21 Exfiltration` as parent and replaced with `TAC-43 Information Release`
- `TEQ-070 PII Dumping`: Removed `TAC-21 Exfiltration` as parent and replaced with `TAC-43 Information Release`
- `TEQ-072 Jigging` -> `TEQ-072 Address Manipulation`: Minor wording changes. Renamed.
- `TEQ-074 Driver Intercept` -> `TEQ-074 Driver Redirect`: Major wording changes. Renamed.
- `TEQ-076 Manual Sale`: Major wording changes.
- `TEQ-078 Valid Accounts`: Minor wording changes.
- `TEQ-079 Fund Withdrawal` -> `TEQ-079 Account Balance Withdrawal`: Renamed.



### Retired
- `TEQ-007 Fake Credibility Generation`: Replaced by `TAC-35 Fake Credibility Generation`
- `TEQ-009 Command & Control`
- `TEQ-017 Technical Reconnaissance`: Replaced by `TAC-34 Attack Surface Identification` and `TAC-44 Vulnerability Identification`
- `TEQ-043 Comment Flooding`: Merged into `TEQ-045 Content Posting`
- `TEQ-048 Overlay Attack`
- `TEQ-052 Distributed Stock Purchase`
- `TEQ-057 Pre-Release Buying`
- `TEQ-068 API Information Flow Exfiltration`

## Killchains

### New
- None

### Updated
- Updated all killchains to reflect the new and updated tactics and techniques

### Retired
- None

## Website
- Renamed framework from Business Logic *Attack* Definition Framework to Business Logic *Abuse* Definition Framework and updated terminology accordingly. The term attack could imply an immediate need for remediation and force a binary response, such as blocking or not blocking. In cases of business logic abuse, multiple levers could be pulled to assist companies facing these challenges. Customers often need to make a business decision, not just a security decision
- Tactics and techniques in Matrix and Killchain views are now displayed in alphabetical order