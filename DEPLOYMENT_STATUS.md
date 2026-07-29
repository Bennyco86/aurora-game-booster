# Aurora Deployment Status

Updated: 2026-07-29

## Current state

Aurora Game Booster is being prepared for Microsoft Store certification. No public
Store listing or approved customer package is available yet.

The Store-specific `1.0.18.0` prototype has passed Aurora's local package checks.
It still needs the production identity assigned by Partner Center, Windows App
Certification Kit retesting, clean Windows 11 testing, owner policy review, and
Microsoft Store certification.

The older direct installer `1.0.17` remains on distribution hold and is not the
Store release candidate.

The planned introductory Store price is USD 9.99 as a one-time purchase. It is not
available for sale until Microsoft completes certification and the listing is
published.

Microsoft completed false-positive submission
`ebef05f6-3719-49ee-8ecb-4639f3c42fcf`. The last verified portal result showed no
malware detected by cloud or client scanning and a favorable analyst comment. The
portal's final-determination column still showed `Pending`, so that status should
not be described as fully final without a new portal check.

## Safety

Do not disable Smart App Control, Microsoft Defender, or another security control
to install Aurora. Do not use installers or packages from mirrors.

When released, the official product page will link to the Microsoft-certified Store
listing and publish release notes, known issues, policies, and support information.
