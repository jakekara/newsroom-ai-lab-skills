# Newsroom AI Lab Toolkit Skills

Document status: Draft

Agent skills that give structured feedback and guidance on the Hacks Hackers Newsroom AI Lab Toolkit.


## Quick start 

The simplest way to use any of the skills is to open a folder and copy the SKILL.md into your LLM chat, 
such as Claude Code, Gemini, or ChatGPT.

If you already know how to install and use skills, then you probably don't need any instructions from us,
but see installation steps below for platform-specific install steps.

---

## Available Skills

### [problem-statement-coach](./problem-statement-coach/SKILL.md)

**Skill status:** Draft.

Reviews and coaches draft problem statements from design thinking workshops.

Triggers when someone shares a problem statement in the format `[User] needs [need] so that [goal]` and wants feedback, or asks for help refining a problem statement.

**What it produces:** Structured feedback covering what's working, what to sharpen, follow-up questions, and 1–3 alternative draft statements.

📥 [Download problem-statement-coach.skill](releases/download/latest/problem-statement-coach.skill)


### [problem-brief-coach](./problem-brief-coach/SKILL.md)

**Skill status:** Draft.

Use this skill to review and give feedback on draft problem briefs from a design thinking workshop.

**What it produces:** Structured feedback covering what's working, what to sharpen, section-by-section feedback, follow-up questions.

📥 [Download problem-statement-coach.skill](releases/download/latest/problem-statement-coach.skill)

## Platform-specific instll steps:

### Adding Skills to Claude

1. Download the `.skill` file from the release link above
2. Open Claude and navigate to your Project
3. Click **Add content → Upload file** and select the `.skill` file
4. Claude will use the skill automatically when the trigger conditions are met

### Local AI: Adding Skills to local LibreChat

TKTKAI

### Local AI: Adding Skills to LM Studio

TKTK

## Contributing

Each directory in this `skills/` directory is a skill and contains a SKILL.md.

To add a skill, create a new folder in the project root and open a pull request.

Packaged `.skill` files are generated and attached to releases automatically (see `.github/workflows/package-skills.yml`).

Skills should follow the [Agent Skills specification](https://agentskills.io/specification).

All skills should set a [semver compliant](https://semver.org/#semantic-versioning-specification-semver)
version number in `metadata.version`. Use `draft` as a pre-release label in place of common `alpha` and
`beta` labels. Use numeric dot suffixes for revisions of a draft, such as `1.2.1-draft.1`.