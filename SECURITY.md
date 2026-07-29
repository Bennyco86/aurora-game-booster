# Aurora Game Booster Security

## Report a security issue

Email `nzbennycohen@gmail.com` with `Aurora security report` in the subject.

Include:

- Aurora version and installer filename.
- Download source.
- SHA-256 checksum.
- Windows version and security product.
- Exact warning or detection name.
- Screenshot with personal information removed.

Do not email passwords, license keys, registry backups, browser data, or unrelated
system logs. Do not publicly post a suspected vulnerability before there has been a
reasonable opportunity to investigate it.

## Installation blocks

Do not disable Smart App Control, Microsoft Defender, antivirus software, or Windows
security features to install Aurora. A blocked installer should be treated as a
security report and investigated before use.

## Release verification

Every public release must publish a SHA-256 checksum. Paid public releases must also
be Authenticode-signed using a certificate that chains to a trusted root authority.
A checksum verifies file identity; a digital signature also verifies the publisher
and detects modification after signing.
