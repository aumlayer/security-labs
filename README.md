<div align="center">
  <a href="https://github.com/aumlayer">
    <img src="https://raw.githubusercontent.com/aumlayer/.github/main/assets/aumlayer-logo.jpg" width="96" alt="AUMLayer" />
  </a>
</div>

# Security Labs

Public research artifacts from [AUMLayer](https://github.com/aumlayer) for **authorized security testing and incident response**: Docker labs, log scanners, and documentation — organized by product and CVE.

> **Use only on systems you own or have explicit permission to test.** See [DISCLAIMER.md](DISCLAIMER.md).

## Catalog

| CVE | Product | Nickname | Lab | Scanner | Updated |
|-----|---------|----------|-----|---------|---------|
| [CVE-2026-109618](https://nvd.nist.gov/vuln/detail/CVE-2026-109618), [CVE-2026-109619](https://nvd.nist.gov/vuln/detail/CVE-2026-109619) | PHP | PHP2Shell | [lab](php/cve-2026-109618-php2shell/lab) | [PHP2Shell Checker](php/cve-2026-109618-php2shell/checker) | 2026-10-22 |

## Quick start (PHP2Shell)

```bash
git clone https://github.com/aumlayer/security-labs.git
cd security-labs/php/cve-2026-109618-php2shell
# Lab + verifier: see README.md in this folder
# Scanner only:  cd checker && ./run_checker.sh --help
```

## Add a new entry

[CONTRIBUTING.md](CONTRIBUTING.md) · [template](templates/CVE-ENTRY-README.template.md)

## What this repo is / is not

| In scope | Out of scope |
|----------|----------------|
| Localhost Docker labs (`127.0.0.1`) | Video production, narration, marketing assets |
| Read-only log / artifact scanners | Host-specific evidence dumps |
| Mechanism + IR documentation | Untargeted exploitation of third-party systems |

## License

MIT — [LICENSE](LICENSE). Third-party PoCs under `lab/vendor/` keep upstream licenses; see each entry’s vendor README.
