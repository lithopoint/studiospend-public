# Security

## Reporting a problem

If you think you have found a security problem in StudioSpend, please tell us privately first.

- **Preferred:** [report it on GitHub](https://github.com/lithopoint/studiospend-public/security/advisories/new). Only we can see the report.
- **Email:** support@studiospend.com with "Security" in the subject.

Please include what you found, how to reproduce it, and which version (Settings, bottom of the screen). We reply within **5 business days**, keep you updated, and credit you in the release notes if you would like.

Please do not open a public issue or post details until a fix is out.

## What to know about how StudioSpend handles data

- Your plans, payments and balances are stored in a database on your Mac.
- Platform sign-ins use each platform's official sign-in page. The access granted to StudioSpend is kept in your Mac's Keychain, not in a file.
- The app sends no analytics. It contacts the platforms you connect, the license service, and the price table hosted in this repository.
- The full list is in [docs/privacy.md](docs/privacy.md).

## Supported versions

Security fixes go into the latest release. Please update before reporting.

## Verifying a download

See [docs/verify.md](docs/verify.md) for checksums and Apple's signature.
