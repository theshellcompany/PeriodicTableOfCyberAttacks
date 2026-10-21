<p align="center">
  <img src="assets/logo.svg" width="200" alt="Periodic Table of Cyber Attacks logo">
</p>

# Periodic Table of Cyber Attacks

An interactive "periodic table" of cyber attack techniques, each with a sourced European case and defences, plus a framework for running tabletop exercises with it.

**Live site: https://theshellcompany.github.io/periodictableofcyberattacks/**

Everything is plain HTML, CSS and JavaScript. There is no build step and nothing to install.

## Contents

| File | What it is |
|------|------------|
| `index.html` | The Periodic Table of Cyber Attacks: attack techniques grouped by family and sophistication, each with a sourced European case and defences |
| `periodic-table-cyber-attacks-tabletop.md` | Tabletop exercise framework that uses the attack table as its scenario source |
| `assets/logo.svg` | Project logo |
| `periodic-table-cyber-attacks.html` | Redirect to `index.html`, so old links keep working |
| `_config.yml` | GitHub Pages settings (renders the tabletop guide as a web page) |

## Quick start

1. Clone or download the repository.
2. Open `index.html` in a modern browser, or use the live site above.
3. Select any tile to see its details.

The page loads fonts from Google Fonts. Offline, it falls back to system fonts and works the same way.

## The Periodic Table of Cyber Attacks

### Layout

- **Columns** are attack families: social engineering, credentials and identity, malware, web applications, network, supply chain and cloud, impact, lateral movement and persistence, and advanced and state-level.
- **Two detached rows** at the bottom, like the lanthanides and actinides, hold AI and machine learning attacks and physical and proximity attacks.
- **Within each column**, techniques get more sophisticated from top to bottom.
- **Dots on each tile** show sophistication from 1 (automated, cheap, widely available) to 5 (custom capability, usually well-resourced criminal groups or state actors). This is an editorial scale, not a formal standard.

### Each element shows

- What the attack is
- A real case with a **Source** link to the page it was taken from
- The main defences
- A reference ID: MITRE ATT&CK (`T…`), MITRE ATLAS for AI attacks (`AML.T…`), or CWE for web weaknesses

### Case labels

Every case is labelled as one of:

- **European incident**: an attack that happened in Europe (48 elements)
- **European research or disclosure**: European research, testing or disclosure, used where no real European incident is documented (11 elements)
- **Global case**: used where no well-documented European incident could be found (6 elements: MFA fatigue, typosquatting, dependency confusion, Kerberoasting, AI agent hijacking, malicious model files)

### Interaction

- **Colour by family / By sophistication** toggles the colour scheme.
- **Search** dims everything that doesn't match.
- **Legend chips** filter to one family.
- On narrow screens the detail panel moves below the table.

## Tabletop exercise framework

`periodic-table-cyber-attacks-tabletop.md` ([read it on the site](https://theshellcompany.github.io/periodictableofcyberattacks/periodic-table-cyber-attacks-tabletop.html)) turns the attack table into a ready-to-run exercise kit:

- **Four ways to pick scenarios**: random attack draw, family deep dive, defence gap analysis, sophistication escalation.
- **Three templates**: attack chain simulation (60–90 min), sophistication escalation (45 min), defence validation (30 min).
- **Role-based assignments** for technical roles, executives (CISO, CIO/CTO, CFO, CEO, COO), business functions (communications, legal, HR, finance, customer success) and the board.
- **A worked example**: a cross-functional ransomware exercise built from FluBot, Great Western Railway and Picanol.
- **A tracking sheet template** for gaps, owners and due dates.

## Editing the data

All content lives in plain JavaScript arrays inside `index.html`. Main columns are in `const D = { … }` and detached rows in `const ROWS = [ … ]`. Each element is:

```js
["Sym", "Name", level, "What it is", "Case", "Defences", "Reference ID", "Source URL", "scope"]
```

- `level` is 1–5. Keep each column sorted from lowest to highest.
- `scope` is `"eu"`, `"eu-res"` or `"global"`.
- Symbols must be unique across the whole table.
- Inner columns (positions 3–7) can hold at most 5 elements, because the detail panel sits above them. Outer columns can hold 6 or 7.


## References

- [MITRE ATT&CK](https://attack.mitre.org)
- [MITRE ATLAS](https://atlas.mitre.org)
- [CWE](https://cwe.mitre.org)
- [ENISA](https://www.enisa.europa.eu)
- [CERT-EU](https://cert.europa.eu)

## Disclaimer and usage

Cases come from public reporting, including trade press, and are summarised in our own words with a link to the source. Attribution and impact figures reflect what those sources reported at the time.

This material is provided as-is for cybersecurity education and preparedness. You may use it for internal exercises, adapt it, and share it with attribution. Please keep the European focus and source links when sharing.
