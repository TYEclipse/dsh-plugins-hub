# dsh-plugins-hub

> An independent, community-friendly plugin index for [DeepSeek Harness (dsh)](https://github.com/deepseek-ai/deepseek-harness).
> Curated by automation + human review. Topic: `dsh-plugin`.

## Featured Plugins

| Plugin | Description | Install | Status | Security | Trial | Checked at | Commit |
|--------|-------------|---------|--------|----------|-------|------------|--------|
| [dsh-netdoctor](https://github.com/TYEclipse/dsh-netdoctor) | Network diagnostics toolbox: DNS lookup, ICMP ping, TCP port check, TLS cert check, traceroute, public IP — six read-only probes, zero runtime dependencies | `dsh plugin --profile web add github:TYEclipse/dsh-netdoctor` | ✅ active | ✅ | ✅ e2e (dns_lookup ×2: system + 8.8.8.8) | 2026-08-16 | 43de786b |
| [dsh-webfetch](https://github.com/TYEclipse/dsh-webfetch) | Web page reader: fetch any URL and extract clean Markdown / plain text plus a link inventory — zero runtime dependencies, read-only | `dsh plugin --profile web add github:TYEclipse/dsh-webfetch` | ✅ active | ✅ | ✅ e2e (web_fetch) | 2026-08-16 | 6296371d |
| [dsh-units](https://github.com/TYEclipse/dsh-units) | Unit conversion toolbox: 14 categories (length, mass, temperature, data sizes decimal-vs-binary, speed, time, volume, pressure, energy, angle, frequency, typography px/pt/em/rem, fuel economy mpg ↔ L/100km) — zero runtime dependencies, pure math | `dsh plugin --profile web add github:TYEclipse/dsh-units` | ✅ active | ✅ | ✅ e2e (convert_unit) | 2026-08-16 | 2bdfae10 |
| [dsh-color](https://github.com/TYEclipse/dsh-color) | Color conversion toolbox: parse/convert any CSS color (hex, rgb()/hsl()/hwb(), all 148 CSS Color 4 named colors), WCAG 2.x contrast ratio with AA/AAA verdicts, named-color lookup by name or value — zero runtime dependencies, pure math | `dsh plugin --profile web add github:TYEclipse/dsh-color` | ✅ active | ✅ | ✅ e2e (contrast_ratio) | 2026-08-16 | 2783169 |
| [Code2Skill](https://github.com/leechen298/Code2Skill) | Three agent skills that generate portable Function / MCP Tool / workflow Skill packages (with offline tests) from user-authorized code, plus independent flow and source-semantics review — pure skill bundle, MIT | `dsh plugin --profile web add github:leechen298/Code2Skill#v1.1.3` | ✅ active | ✅ | ✅ e2e (code2skill-review-source skill invoked headless) | 2026-08-16 | 7815d8f1 |

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
