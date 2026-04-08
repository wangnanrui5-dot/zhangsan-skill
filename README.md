[中文版](README_zh.md)

# Gender Risk Shield 🛡️

**Simulate hyper-sensitive internet audiences to scan any content for gender-related risks.**

Use it seriously — it's a risk management tool. Use it casually — it's endlessly entertaining.

---

## What It Does

Gender Risk Shield is an AI skill (knowledge pack) that makes your AI agent think like the most easily offended people on the internet — and tells you exactly where your content will blow up.

Feed it a press release, a campaign brief, a competitor's latest move, or any public-facing content. It runs three modes:

| Mode | What It Does |
|------|-------------|
| **Path A: Risk Analysis** | 8-dimension scan for gender landmines. Tells you what will explode, who will attack, and where. |
| **Path B: Counter-Narrative** | You're under attack. Get defense strategies, talking points, and comment-section scripts to cool things down. |
| **Path C: Competitor Attack** | Find your competitor's gender-related weak spots. Get attack angles, persona scripts, and deployment tactics. |

## Industry Support

Gaming · Beauty · Automotive · F&B · Entertainment · Fashion · Tech · Education · Personal Branding · Esports

Not limited to the above. If your brand faces the public, this works.

## The 8-Dimension Model

Every piece of content is scanned across 8 dimensions, scored 0-10 (≥7 = high risk):

| Dimension | What It Scans |
|-----------|--------------|
| Feminist / Pro-Women | Objectification, anti-women sentiment, male gaze, sexualization |
| Men's Rights | Anti-male bias, double standards, ignoring male users |
| BL (Boys' Love) | Queerbaiting accusations, CP wars, BL territory conflicts |
| BG (Het Romance) | Het CP being sidelined, erased, or overwritten by BL |
| ML (Player-Insert) | Character→player emotional bond being broken, "sharing" characters |
| Otome | Female player immersion, male character exclusivity, "otome law" violations |
| GL (Girls' Love) | Yuri elements, GL territory conflicts |
| LGBT / Transgender | Gender-fluid designs, non-binary elements, policy risks |

Weights auto-adjust by industry. Beauty brands get 1.5x on feminist dimensions. FPS games get 1.5x on men's rights. Details in [risk-dimensions.md](references/risk-dimensions.md).

## Quick Start

### As an OpenClaw Skill

```bash
openclaw skill install gender-risk-shield
```

The AI agent will automatically detect and load it. Just describe your scenario and pick a path.

### As a Standalone Reference

No AI agent needed. Read the files in `references/` as a crisis playbook:
- [risk-dimensions.md](references/risk-dimensions.md) — Scoring rubric
- [defense-strategies.md](references/defense-strategies.md) — 15 defense strategies
- [offense-playbook.md](references/offense-playbook.md) — Competitor attack methodology
- [attack-patterns.md](references/attack-patterns.md) — Attack pattern library
- [case-library.md](references/case-library.md) — Cross-industry case studies
- [otome-rules.md](references/otome-rules.md) — 41 unwritten otome community rules

## Example Prompts

**Risk Analysis (Path A):**
> "We're about to release a promotional PV featuring a male character. Our audience is mostly female. Scan it for gender risks."

**Counter-Narrative (Path B):**
> "Our product is being attacked on social media as 'anti-women' because we chose a male spokesperson. Sentiment is rising. Help me build a counter-narrative."

**Competitor Attack (Path C):**
> "A competitor just launched an anime collab with merch featuring only male characters. Their user base is 70% female. Find attack angles."

## Eval Results

Real-world scenario tests demonstrating the skill in action:

| Eval | Scenario | Path | Output |
|------|----------|------|--------|
| eval-01 | Game PV gender risk scan | A (Risk Analysis) | [output-01](evals/output-01-game-pv.md) |
| eval-02 | Beauty brand male spokesperson backlash | B (Counter-Narrative) | [output-02](evals/output-02-beauty-endorsement.md) |
| eval-03 | Competitor tea brand collab gender gap | C (Competitor Attack) | [output-03](evals/output-03-competitor-attack.md) |

## File Structure

```
gender-risk-shield/
├── SKILL.md                          # Main file: workflow and output formats
├── README.md                         # English readme (this file)
├── README_zh.md                      # Chinese readme
├── LICENSE                           # MIT
├── CHANGELOG.md                      # Version history
├── CONTRIBUTING.md                   # How to contribute
├── clawhub.json                      # ClawHub package config
├── references/
│   ├── risk-dimensions.md            # 8-dimension scoring rubric
│   ├── defense-strategies.md         # 15 defense strategies
│   ├── attack-patterns.md            # Attack pattern library (by faction)
│   ├── offense-playbook.md           # Competitor attack methodology
│   ├── case-library.md               # Cross-industry case studies
│   ├── platform-rules.md             # Platform-specific gender topic traits
│   └── otome-rules.md               # 41 unwritten otome community rules
└── evals/
    ├── files/                        # Test case inputs
    ├── output-01-game-pv.md          # Eval 1: Game PV risk analysis
    ├── output-02-beauty-endorsement.md  # Eval 2: Beauty brand counter-narrative
    └── output-03-competitor-attack.md   # Eval 3: Competitor attack plan
```

## Contributing

New cases, new attack patterns, new industry scenarios — all welcome. See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

[MIT](LICENSE)
