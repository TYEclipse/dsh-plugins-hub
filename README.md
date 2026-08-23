# dsh-plugins-hub

> An independent, community-friendly plugin index for [DeepSeek Harness (dsh)](https://github.com/deepseek-ai/deepseek-harness).
> Curated by automation + human review. Topic: `dsh-plugin`.

## Featured Plugins

| Plugin | Description | Install | Status | Security | Trial | Checked at | Commit |
|--------|-------------|---------|--------|----------|-------|------------|--------|
| [dsh-netdoctor](https://github.com/TYEclipse/dsh-netdoctor) | Network diagnostics toolbox: DNS lookup, ICMP ping, TCP port check, TLS cert check, traceroute, public IP — six read-only probes, zero runtime dependencies | `dsh plugin --profile web add github:TYEclipse/dsh-netdoctor` | ✅ active | ✅ | ✅ e2e (dns_lookup ×2: system + 8.8.8.8) | 2026-08-16 | 43de786b |
| [dsh-webfetch](https://github.com/TYEclipse/dsh-webfetch) | Web page reader: fetch any URL as clean Markdown / plain text, inventory links, read RSS/Atom feeds, inspect HTTP status/headers/redirect chain without the body (web_headers: HEAD with automatic GET fallback), zero-dependency http proxy support — zero runtime dependencies, read-only | `dsh plugin --profile web add github:TYEclipse/dsh-webfetch#v0.3.0` | ✅ active | ✅ | ✅ e2e (web_headers headless: example.com → 200 text/html; httpbin redirect/2 → 2×302 hops → 200; status/404 → 404 reported) | 2026-08-24 | 1f57cd6 |
| [dsh-units](https://github.com/TYEclipse/dsh-units) | Unit conversion toolbox: 17 categories (length, mass, temperature, data sizes decimal-vs-binary, speed, time, volume, pressure, energy, angle, frequency, power with 3 horsepower definitions, force, torque, typography px/pt/em/rem, fuel economy mpg ↔ L/100km) — zero runtime dependencies, pure math | `dsh plugin --profile web add github:TYEclipse/dsh-units` | ✅ active | ✅ | ✅ e2e (convert_unit headless: 150 kw→hp 201.153313, 1 lbfft→n.m 1.355818, 1 kilonewton→n 1000) | 2026-08-23 | 316aca3 |
| [dsh-color](https://github.com/TYEclipse/dsh-color) | Color conversion toolbox: parse/convert any CSS color (hex, rgb()/hsl()/hwb(), all 148 CSS Color 4 named colors), WCAG 2.x contrast ratio with AA/AAA verdicts, named-color lookup by name or value — zero runtime dependencies, pure math | `dsh plugin --profile web add github:TYEclipse/dsh-color` | ✅ active | ✅ | ✅ e2e (contrast_ratio) | 2026-08-16 | 2783169 |
| [Code2Skill](https://github.com/leechen298/Code2Skill) | Three agent skills that generate portable Function / MCP Tool / workflow Skill packages (with offline tests) from user-authorized code, plus independent flow and source-semantics review — pure skill bundle, MIT | `dsh plugin --profile web add github:leechen298/Code2Skill#v1.1.3` | ✅ active | ✅ | ✅ e2e (code2skill-review-source skill invoked headless) | 2026-08-16 | 7815d8f1 |
| [dsh-semver](https://github.com/TYEclipse/dsh-semver) | Semantic versioning toolbox: parse any semver string (semver_parse), compare versions with spec-compliant prerelease ordering (semver_compare, build metadata ignored), and check npm-style ranges (semver_satisfies: ^ ~ >= <= > < =, x-ranges, hyphen, \|\|, AND, tuple-lock prerelease semantics, includePrerelease override) — zero runtime dependencies, pure logic | `dsh plugin --profile web add github:TYEclipse/dsh-semver` | ✅ active | ✅ | ✅ e2e (semver_satisfies tuple-lock + semver_compare) | 2026-08-16 | e347c15 |
| [Archify for DSH](https://github.com/tt-a1i/archify) | Opt-in skill-only bundle (@tt-a1i/archify-dsh) bringing the Archify architecture-diagram skill to dsh: typed JSON specs (architecture / workflow / sequence / dataflow / lifecycle) rendered to self-contained interactive HTML with inline SVG, showcase-quality validation (9 artifact checks) — pure skill bundle, MIT | `dsh plugin --profile web add @tt-a1i/archify-dsh@0.1.0` | ✅ active | ✅ | ✅ e2e (archify skill headless: 9/9 showcase validation) | 2026-08-16 | 0.1.0 |
| [dsh-finance](https://github.com/TYEclipse/dsh-finance) | Money math toolbox: fixed-rate loan payment with amortization schedule and extra-payment impact (loan_payment), compound growth projection with monthly contributions and any compounding frequency (compound_growth), nominal ↔ effective annual rate conversion incl. continuous (rate_convert) — zero runtime dependencies, pure arithmetic, headline values verified against published anchors | `dsh plugin --profile web add github:TYEclipse/dsh-finance` | ✅ active | ✅ | ✅ e2e (compound_growth + rate_convert headless) | 2026-08-17 | 3d1e277 |
| [dsh-ipcalc](https://github.com/TYEclipse/dsh-ipcalc) | IP & subnet math toolbox: full IPv4 subnet layouts (ipv4_subnet: network/broadcast/mask/hosts + IANA classes, RFC 3021 /31), minimal covering CIDR aggregation (ipv4_summarize), and IPv4/IPv6 parsing with RFC 5952 normalization and embedded-IPv4 recognition (ip_parse) — zero runtime dependencies, pure local math, no network I/O | `dsh plugin --profile web add github:TYEclipse/dsh-ipcalc` | ✅ active | ✅ | ✅ e2e (ipv4_summarize headless: 4×/24 → /22) | 2026-08-18 | 6a267cd |
| [dsh-geodesy](https://github.com/TYEclipse/dsh-geodesy) | Geodesic math toolbox: great-circle distance with bearings and compass direction (geo_distance), initial/final bearings plus great-circle midpoint (geo_bearing), direct-problem destination point with round-trip check (geo_destination), and decimal/DMS coordinate parsing with pair & suffix support (coord_parse) — zero runtime dependencies, pure trigonometry on the IUGG mean Earth radius, configurable radiusKm | `dsh plugin --profile web add github:TYEclipse/dsh-geodesy` | ✅ active | ✅ | ✅ e2e (geo_bearing London→NY 288.33° WNW + geo_destination 1000 km due east → 0, 8.993204) | 2026-08-19 | 034883a |
| [dsh-checkdigit](https://github.com/TYEclipse/dsh-checkdigit) | Check-digit mathematics toolbox: generate, validate and auto-detect check digits for 11 schemes — Luhn (cards/IMEI), Verhoeff, Damm, ISBN-10 (mod-11, X) / ISBN-13, EAN-8/13, UPC-A, ISIN (ISO 6166), CUSIP (ANSI X9.6) and IBAN (ISO 13616, 75+ country BBAN table) — zero runtime dependencies, pure integer arithmetic anchored to published worked examples | `dsh plugin --profile web add github:TYEclipse/dsh-checkdigit` | ✅ active | ✅ | ✅ e2e (checkdigit_validate GB82 IBAN + checkdigit_generate Luhn 7992739871→3, headless) | 2026-08-20 | 3d0f9b5 |
| [MemOS Cloud for DSH](https://github.com/MemTensor/MemOS-Cloud-OpenClaw-Plugin/tree/main/packages/dsh) | Cloud lifecycle-memory plugin: pre-step recall injection and post-turn memory sync backed by the MemOS Cloud API (memos.memtensor.cn); no tools registered — agent/pre-step + session/event hooks with graceful degradation when no API key is configured; MIT | `dsh plugin --profile web add @memtensor/memos-cloud-dsh-plugin@0.1.0` | ✅ active | ✅ | ✅ e2e (headless turn completes 17×23=391 with plugin mounted, no-credential degradation verified) | 2026-08-20 | 0.1.0 |

Columns: **Security** = passed preliminary source review (TRACE-lite: trust / reliability / auditability / confidentiality / effectiveness); **Trial** = verified in an isolated profile with a real end-to-end tool call; **Commit** = the exact revision that was verified.

## How to add your plugin

1. Add the `dsh-plugin` topic to your plugin repository
2. Open an issue in this repository using the **Plugin Submission** template (plugin name, repo link, release tag, license, install command)
3. The pipeline verifies the submission in an isolated profile — security review, install, and one real end-to-end tool call
4. Verified plugins are added to the index and the issue is closed; failed submissions stay open with a `needs-fix` label and a summary reply

## About

- Independent community index (not affiliated with DeepSeek AI)
- Updated automatically on a daily basis
- MIT License

---

*Maintained by the dsh-autopilot pipeline.*
