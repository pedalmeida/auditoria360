# Instalar o Claude Code + a skill cz-audit (5 min)

> Nunca usaste um terminal? Não faz mal. Isto está escrito para quem nunca instalou nada fora da App Store. E se não quiseres instalar nada, usa o **Caminho A** do [README](./README.md): colar o `00-wizard.md` num chat do Claude.ai. Funciona igual, só não grava os ficheiros por ti.

---

## O que é o Claude Code?

É o Claude a correr no teu computador em vez do browser. A diferença que interessa aqui: consegue **criar e gravar ficheiros** (o `checkup.html`, o `audit.md`) e aceitar **skills**, que são instruções permanentes que ele carrega sozinho. Instalas a skill uma vez, e depois basta dizer "audita este negócio" em qualquer conversa.

Precisas de uma conta Claude (o plano Pro chega perfeitamente).

*(Já instalaste o módulo 1? Então já tens o Claude Code. Salta para o Passo 2.)*

---

## Passo 1 - Instalar o Claude Code

**Mac:** abre a app **Terminal** (cmd+espaço, escreve "terminal", enter) e cola:

```bash
curl -fsSL https://claude.ai/install.sh | bash
```

**Windows:** abre o **PowerShell** (menu iniciar, escreve "powershell", enter) e cola:

```powershell
irm https://claude.ai/install.ps1 | iex
```

Quando terminar, fecha e volta a abrir o terminal, e escreve:

```bash
claude
```

Na primeira vez pede-te para fazeres login com a tua conta Claude. Segue as instruções no ecrã e está feito.

*(Se algum destes comandos der erro, vai a [docs.anthropic.com/claude-code](https://docs.anthropic.com/en/docs/claude-code) que tem os métodos alternativos de instalação sempre atualizados.)*

---

## Passo 2 - Instalar a skill cz-audit

A skill é só uma pasta com um ficheiro dentro. Cola isto no terminal (Mac) ou no PowerShell (Windows, funciona igual):

**Mac:**
```bash
mkdir -p ~/.claude/skills/cz-audit
```

**Windows:**
```powershell
mkdir -Force "$HOME\.claude\skills\cz-audit"
```

Agora guarda o ficheiro [`SKILL.md`](./skill/SKILL.md) dentro dessa pasta. Duas formas:

- **Simples:** abre o `SKILL.md` daqui, copia o conteúdo todo, cria um ficheiro chamado `SKILL.md` dentro da pasta `cz-audit` que acabaste de criar, e cola lá o conteúdo.
- **Ainda mais simples:** abre o Claude Code (`claude` no terminal) e diz-lhe: *"cria o ficheiro ~/.claude/skills/cz-audit/SKILL.md com o conteúdo que te vou colar"* e cola o SKILL.md. Ele faz o resto.

> Esta é a série **Cliente Zero**. Este é o módulo 2 (auditoria). O módulo 1 (scraping + cold call) e o módulo 3 (outreach) instalam-se da mesma forma, cada um na sua pasta. Podes usar só este, ou instalar os três e encadeá-los.

---

## Passo 3 - Usar

Abre a tua pasta de trabalho (a mesma do módulo 1, se o usaste: `Documentos/clientes` ou onde tiveres o `leads.csv`), corre `claude` lá dentro, e escreve:

> audita este negócio: &lt;cola o site aqui&gt;

Ou, se já correste o módulo 1 e tens o `leads.csv` na pasta:

> faz o check-up do melhor lead

A skill assume o comando: faz a auditoria, extrai o branding do negócio, e grava o `checkup.html` + o `audit.md` na pasta `clientes/<slug>/`.

---

## Problemas comuns

| Sintoma | Solução |
|---|---|
| `claude: command not found` | Fecha e reabre o terminal. Se persistir, repete o Passo 1. |
| A skill não dispara | Confirma que o ficheiro está exatamente em `~/.claude/skills/cz-audit/SKILL.md` e reinicia o Claude Code. |
| "não consigo abrir o site" | Confirma que o site está online e o URL correto. Se for um site pesado em JS (Wix/Squarespace) e o Claude não vir o conteúdo, cola-lhe tu o texto principal da página, ele continua a partir daí. |
| O `checkup.html` saiu sem o logo | O site não expunha o logótipo de forma extraível. É esperado, a skill usa então o cabeçalho neutro. Se tiveres o logo à mão, dá-lho e pede para o meter. |
