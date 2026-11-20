# OWASP Security Reviewer

[English](README.md) | **Português (Brasil)**

Skill de agente para auditoria de segurança de aplicações web pelo **OWASP Top 10 (2021)**: controle de acesso, criptografia, injection, design inseguro, configuração, dependências, autenticação, integridade (webhooks/HMAC), logging e SSRF.

Revisa auth, rotas de API, consultas ao banco, CSRF/JWT, webhooks e segredos, e entrega um relatório com achados classificados por severidade.

A skill é **somente leitura**: analisa e reporta, sem editar arquivos.

Segue o formato aberto de [Agent Skills](https://agentskills.io) (`SKILL.md` com frontmatter `name` e `description`) e funciona no Claude Code, Cursor e outros agentes compatíveis.

## Instalação

A pasta de destino deve se chamar `owasp-security-reviewer` (o nome da skill), não o nome do repositório.

### Claude Code

```bash
# Para todos os projetos
git clone https://github.com/jrcarls/skill-owasp-security-reviewer.git ~/.claude/skills/owasp-security-reviewer

# Apenas para um projeto
git clone https://github.com/jrcarls/skill-owasp-security-reviewer.git .claude/skills/owasp-security-reviewer
```

### Cursor

```bash
git clone https://github.com/jrcarls/skill-owasp-security-reviewer.git .cursor/skills/owasp-security-reviewer
```

## Uso

O agente carrega a skill automaticamente quando a tarefa combina com a descrição. Para chamar explicitamente no Claude Code:

```text
/owasp-security-reviewer
```

## Skills relacionadas

Esta skill faz parte de um conjunto que se complementa:

- `skill-owasp-security-reviewer` — OWASP Top 10
- `skill-llm-security-reviewer` — OWASP LLM Top 10
- `skill-tenant-isolation-reviewer` — IDOR / ownership
- `skill-lgpd-compliance-advisor` — conformidade LGPD
- `skill-qa-verifier` — verificação funcional
- `skill-vue-reviewer` — revisão de frontend Vue

## Licença

[MIT](LICENSE)
