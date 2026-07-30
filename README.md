# Kobalt

Kobalt Music Group is an independent music rights management and administrative publishing company founded in 2000 by Willard Ahdritz, operating from New York and London. Unlike traditional publishers it administers copyrights rather than owning them, running Kobalt Music Publishing, a neighbouring rights division, and AMRA, the digital-first collection society it acquired in 2014. Royalty and rights processing runs on KTech, the rights and content management platform built to independently serve both Kobalt Music Publishing and AMRA, with songwriters and rightsholders viewing statements and analytics through the authenticated Kobalt Portal.

## API surface

Kobalt publishes **no public developer program**. A 2026-07-19 probe found no developer portal, no API documentation, no OpenAPI or AsyncAPI description, and no API discovery documents under `/.well-known/`. The Kobalt Portal (`portal.kobaltmusic.com`) is an authenticated client application for signed songwriters and rightsholders, not an open API. Integration is arranged commercially through Kobalt or KTech.

The corporate site sits behind Cloudflare bot protection — HTML paths return `403` to non-browser clients, while static `/.well-known/` and `/robots.txt` paths serve normally.

## Artifacts

| Artifact | File |
|---|---|
| Well-Known index | `well-known/kobalt-well-known.yml` |
| security.txt (RFC 9116) | `well-known/kobalt-security.txt` |
| Vulnerability disclosure | `security/kobalt-vulnerability-disclosure.yml` |
| Domain security | `security/kobalt-domain-security.yml` |
| llms.txt | `llms/kobalt-llms.txt` |

Backed by: gv, version-one-ventures — https://www.kobaltmusic.com
