<div align="center">

# Samarpan Aree

**IT & software engineering — security tooling, backend APIs, developer utilities.**

[![GitHub](https://img.shields.io/badge/GitHub-samarpan--aree-181717?style=flat-square&logo=github)](https://github.com/samarpan-aree)
[![Location](https://img.shields.io/badge/Kathmandu-Nepal-0f766e?style=flat-square)](https://github.com/samarpan-aree)
[![Open to work](https://img.shields.io/badge/status-open_to_work-16a34a?style=flat-square)](https://github.com/samarpan-aree)
[![Repos](https://img.shields.io/badge/public_repos-5-blue?style=flat-square)](https://github.com/samarpan-aree?tab=repositories)

</div>

---

I build software that holds up under review: tested, documented, and shipped with
CI. My work sits in two places — **security tooling** that turns noisy signal into
something a human can act on, and the **backend and DX layer** around it, because
that is what decides whether a codebase is still maintainable after month one.

Every repository below runs. Every one ships with a test suite you can execute in
under a second, and no runtime dependencies unless the problem genuinely requires them.

## Tech stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

## Featured work

| Repository | What it does |
| --- | --- |
| **[sshwatch](https://github.com/samarpan-aree/sshwatch)** | Reads SSH auth logs and reports the three findings that matter: brute force, credential spraying, and accounts that were actually compromised. Persistence-gated so scanner noise stays out. Offline, zero dependencies, 99 tests, SARIF output. |
| **[leakscan](https://github.com/samarpan-aree/leakscan)** | Secret and credential scanner with 24 vendor patterns and Shannon-entropy gating, so `your_api_key_here` does not appear in the report. Redaction happens at finding-creation time — there is no code path that emits a full secret. |
| **[posturekit](https://github.com/samarpan-aree/posturekit)** | External security posture in one pass: HTTP security headers, cookie flags, TLS configuration and DNS email authentication (SPF/DKIM/DMARC). Weighted 0–100 grade, SARIF for code scanning. |
| **[uptimekit](https://github.com/samarpan-aree/uptimekit)** | Self-hosted API uptime and latency monitoring. FastAPI + React + SQLite, with a shields.io badge endpoint. No external services, no third-party data retention. 65 tests. |
| **[repolint](https://github.com/samarpan-aree/repolint)** | Zero-dependency CLI that scores any repository against a seven-point professional checklist. Weighted 0–100 with a letter grade and `--min-score` gating for CI. |

Four of the five are security tools, and that is deliberate: it is the domain
where precision matters most. A scanner that reports everything gets switched
off, and a scanner that is off catches nothing — so each of these is built around
what it must *not* report, and the test suites assert the silence cases as
carefully as the detections.

## What I care about

- **Tests that assert behaviour at the boundary.** The off-by-one at a threshold
  is the bug that ships; a test against a big fixture log hides it.
- **Zero dependencies where possible.** A tool you drop onto a locked-down host
  should not add an audit surface.
- **Honest limitations.** Every README here has a "limits worth knowing" section.
  A tool that hides its failure modes cannot be trusted with its successes.
- **CI that gates on something real.** Not a green checkmark — an actual exit code
  that fails the build.

---

<div align="center">
<sub>Open to backend, platform and full-stack roles. Reach out through GitHub.</sub>
</div>
