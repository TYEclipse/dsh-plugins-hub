# dsh-plugins-hub

> An independent, community-friendly plugin index for [DeepSeek Harness (dsh)](https://github.com/deepseek-ai/deepseek-harness).
> Curated by automation + human review. Topic: `dsh-plugin`.

## Featured Plugins

| Plugin | Description | Install | Status | Security | Trial | Checked at | Commit |
|--------|-------------|---------|--------|----------|-------|------------|--------|
| [dsh-netdoctor](https://github.com/TYEclipse/dsh-netdoctor) | Network diagnostics toolbox: DNS lookup, ICMP ping, TCP port check, TLS cert check, traceroute, public IP — six read-only probes, zero runtime dependencies | `dsh plugin --profile web add github:TYEclipse/dsh-netdoctor` | ✅ active | ✅ | ✅ e2e (dns_lookup ×2: system + 8.8.8.8) | 2026-08-16 | 43de786b |
| [dsh-webfetch](https://github.com/TYEclipse/dsh-webfetch) | Web page reader: fetch any URL and extract clean Markdown / plain text plus a link inventory — zero runtime dependencies, read-only | `dsh plugin --profile web add github:TYEclipse/dsh-webfetch` | ✅ active | ✅ | ✅ e2e (web_fetch) | 2026-08-16 | 6296371d |
| [dsh-units](https://github.com/TYEclipse/dsh-units) | Unit conversion toolbox: 12 categories (length, mass, temperature, data sizes decimal-vs-binary, speed, time, volume, pressure, energy, angle, frequency) — zero runtime dependencies, pure math | `dsh plugin --profile web add github:TYEclipse/dsh-units` | ✅ active | ✅ | ✅ e2e (convert_unit) | 2026-08-16 | dbfc5350 |

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
