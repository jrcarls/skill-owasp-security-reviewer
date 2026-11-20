# OWASP Security Reviewer

**English** | [Português (Brasil)](README.pt-BR.md)

An agent skill that audits web applications against the **OWASP Top 10 (2021)**: access control, cryptography, injection, insecure design, misconfiguration, vulnerable components, authentication, integrity (webhooks/HMAC), logging and SSRF.

It reviews auth, API routes, database queries, CSRF/JWT, webhooks and secrets, and delivers a report with findings ranked by severity.

The skill is **read-only**: it analyzes and reports without editing files.

It follows the open [Agent Skills](https://agentskills.io) format (`SKILL.md` with `name` and `description` frontmatter) and works with Claude Code, Cursor and other compatible agents. The skill instructions are written in Brazilian Portuguese.

## Installation

The target folder must be named `owasp-security-reviewer` (the skill name), not the repository name.

### Claude Code

```bash
# All projects
git clone https://github.com/jrcarls/skill-owasp-security-reviewer.git ~/.claude/skills/owasp-security-reviewer

# A single project
git clone https://github.com/jrcarls/skill-owasp-security-reviewer.git .claude/skills/owasp-security-reviewer
```

### Cursor

```bash
git clone https://github.com/jrcarls/skill-owasp-security-reviewer.git .cursor/skills/owasp-security-reviewer
```

## Usage

The agent loads the skill automatically when the task matches its description. To invoke it explicitly in Claude Code:

```text
/owasp-security-reviewer
```

## Related skills

This skill is part of a complementary set:

- `skill-owasp-security-reviewer` — OWASP Top 10
- `skill-llm-security-reviewer` — OWASP LLM Top 10
- `skill-tenant-isolation-reviewer` — IDOR / ownership
- `skill-lgpd-compliance-advisor` — LGPD compliance
- `skill-qa-verifier` — functional verification
- `skill-vue-reviewer` — Vue frontend review

## License

[MIT](LICENSE)
