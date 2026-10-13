# Reconnaisance 

### 1. External Reconnaissance and Enumeration Principles

#### Why do it?
Before kicking off any pentest, it can be beneficial to perform external reconnaissance of your target. This can serve many different functions, such as:
- Validating information provided to you in the scoping document from the client
- Ensuring you are taking actions against the appropriate scope when working remotely
- Looking for any information that is publicly accessible that can affect the outcome of your test, such as leaked credentials

#### What to look for?
This can look several different ways
- As simple as gleaning a username format from a company/social media site
- Scanning GitHub repositories for credentials left in code pushes
- Hunting in public documents for credentials or links to an intranet or remote sites
- Any configuration information

Things we should look for:
1. IP Space -- Valid ASN for our target, netblocks in use for the organization's public-facing infrastructure, cloud presence and the hosting providers, DNS record entries, etc.
2. Domain Information -- Who administers the domain? Are there any subdomains tied to our target? Are there any publicly accessible domain services present? (Mailservers, DNS, Websites, VPN portals, etc.) Can we determine what kind of defenses are in place? (SIEM, AV, IPS/IDS in use, etc.)
3. Schema Format -- Can we discover the organization's email accounts, AD usernames, and even password policies? Anything that will give us information we can use to build a valid username list to test external-facing services for password spraying, credential stuffing, brute forcing, etc.
4. Data Disclosures -- For data disclosures we will be looking for publicly accessible files ( .pdf, .ppt, .docx, .xlsx, etc. ) for any information that helps shed light on the target. For example, any published files that contain intranet site listings, user metadata, shares, or other critical software or hardware in the environment (credentials pushed to a public GitHub repo, the internal AD username format in the metadata of a PDF, for example.)
5. Breach Data -- Any publicly released usernames, passwords, or other critical information that can help an attacker gain a foothold.

#### Where to look, and how?
1. 
