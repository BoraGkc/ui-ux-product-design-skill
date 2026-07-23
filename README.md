# UI/UX Product Design Skill

A Codex skill for product UI/UX reasoning, redesign, implementation, and validation. It helps turn vague requests such as “make it nicer” into clearer product jobs, usable workflows, explicit states, accessible interactions, and verified product changes.

The skill covers dashboards, expert tools, AI-assisted products, design systems, ecommerce and UGC, onboarding, healthcare and finance workflows, search and marketplaces, editorial products, sensitive mobile experiences, booking flows, security and IoT products, and data visualization.

## How it works

The skill selects one internal mode from the request:

- **Review** diagnoses and prioritizes issues without editing.
- **Redesign** produces an implementation-ready product proposal without writing code unless asked.
- **Implement** reuses the existing system, makes the smallest complete change, and verifies the runnable interface.
- **Validate** preserves the current design and reports pass, fail, and blocked checks.

New or visually open UI also loads a compact, system-first visual-craft guide. It does not install a preset database or force a house style.

## Install

Ask Codex:

```text
Install this skill:
https://github.com/BoraGkc/ui-ux-product-design-skill/tree/main/ui-ux-product-design
```

Or install it manually:

```bash
git clone https://github.com/BoraGkc/ui-ux-product-design-skill.git
mkdir -p ~/.codex/skills
cp -R ui-ux-product-design-skill/ui-ux-product-design ~/.codex/skills/
```

The skill will be available as `$ui-ux-product-design` on the next Codex turn.

### Installation and updates

Installation copies only the `ui-ux-product-design/` folder into your local Codex skills directory. It does not run from GitHub, connect your account to the repository, or update automatically.

To update, ask Codex:

```text
Update my installed skill from:
https://github.com/BoraGkc/ui-ux-product-design-skill/tree/main/ui-ux-product-design
```

Back up intentional local edits first because an update may replace installed skill files.

## Example prompts

```text
Use $ui-ux-product-design to review this dashboard and prioritize the UX issues.
```

```text
Use $ui-ux-product-design to redesign this expert workspace without hiding the primary canvas.
```

```text
Use $ui-ux-product-design to design an AI recommendation flow with clear consent and recovery states.
```

```text
Use $ui-ux-product-design to implement this settings screen using the existing design system, then verify it at desktop and mobile sizes.
```

```text
Use $ui-ux-product-design to validate this checkout without changing it.
```

## Repository structure

```text
.
├── EVALS.md
├── README.md
├── LICENSE
├── SOURCES.md
└── ui-ux-product-design/
    ├── SKILL.md
    ├── agents/openai.yaml
    └── references/
        └── visual-craft.md
```

Repository documentation stays outside the installable skill folder.

## Source designers and creators

The reference library synthesizes product-design lessons from public case studies by:

| Creator | Portfolio |
| --- | --- |
| Michele Du | [micheledu.com](https://micheledu.com/) |
| Sanvithi Saya | [sanvithi.com](https://sanvithi.com/) |
| Amy La | [amylalai.com](https://amylalai.com/) |
| Alex Chiu | [mchiu.co.uk](https://mchiu.co.uk/) |
| Jackson Ringger | [Chaachie Designs](https://chaachiedesigns.framer.website/) |
| Joe Pendlebury | [joependlebury.com](https://www.joependlebury.com/) |
| Nicole Roberts | [nicolearoberts.com](https://www.nicolearoberts.com/) |
| Nate Bauer | [nabauer.com](https://nabauer.com/) |
| Jacob Dilley | [jacobdilley.com](https://jacobdilley.com/) |
| Ramachandran Swamy | [whyramachandran.design](https://whyramachandran.design/) |
| Lawrence Zheng | [lawrencezheng.com](https://www.lawrencezheng.com/) |
| Bethany Heck | [heckhouse.com](https://heckhouse.com/) |
| Karolis Kosas | [karoliskosas.com](https://karoliskosas.com/) |
| Jonathan Patterson | [jonathanpatterson.com](https://www.jonathanpatterson.com/) |

See [SOURCES.md](SOURCES.md) for the complete case-study index.

The creators above are credited as the authors or portfolio owners of the reviewed sources, not necessarily as the sole contributors to every project. Original pages remain authoritative for project roles and collaborator credits. This repository is independent and does not imply endorsement or affiliation.

## License

Original repository content by [Bora Gökçe](https://github.com/BoraGkc) is licensed under [CC BY 4.0](LICENSE).

The license does not cover third-party websites, case studies, images, trademarks, or other referenced works. Those remain the property of their respective owners.
