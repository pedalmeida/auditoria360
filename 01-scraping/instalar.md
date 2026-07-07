# Instalar o Claude Code + a skill cz-scraping (5 min)

> Nunca usaste um terminal? Não faz mal. Isto está escrito para quem nunca instalou nada fora da App Store. E se não quiseres instalar nada, usa o **Caminho A** do [README](./README.md): colar o `00-wizard.md` num chat do Claude.ai. Funciona igual, só não grava os ficheiros por ti.

---

## O que é o Claude Code?

É o Claude a correr no teu computador em vez do browser. A diferença que interessa aqui: consegue **criar e gravar ficheiros** (o `leads.csv`, o tracker) e aceitar **skills**, que são instruções permanentes que ele carrega sozinho. Instalas a skill uma vez, e depois basta dizer "quero encontrar clientes" em qualquer conversa.

Precisas de uma conta Claude (o plano Pro chega perfeitamente).

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

## Passo 2 - Instalar a skill cz-scraping

A skill é só uma pasta com um ficheiro dentro. Cola isto no terminal (Mac) ou no PowerShell (Windows, funciona igual):

**Mac:**
```bash
mkdir -p ~/.claude/skills/cz-scraping
```

**Windows:**
```powershell
mkdir -Force "$HOME\.claude\skills\cz-scraping"
```

Agora guarda o ficheiro [`SKILL.md`](./skill/SKILL.md) dentro dessa pasta. Duas formas:

- **Simples:** abre o `SKILL.md` daqui, copia o conteúdo todo, cria um ficheiro chamado `SKILL.md` dentro da pasta `cz-scraping` que acabaste de criar, e cola lá o conteúdo.
- **Ainda mais simples:** abre o Claude Code (`claude` no terminal) e diz-lhe: *"cria o ficheiro ~/.claude/skills/cz-scraping/SKILL.md com o conteúdo que te vou colar"* e cola o SKILL.md. Ele faz o resto.

> Esta é a série **Cliente Zero**. Este é o módulo 1 (scraping). Os módulos 2 (auditoria com entregável branded) e 3 (outreach + draft no Gmail) instalam-se da mesma forma, cada um na sua pasta. Podes usar só este, ou instalar os três e encadeá-los.

---

## Passo 3 - Usar

Abre uma pasta de trabalho qualquer (ex: `Documentos/clientes`), corre `claude` lá dentro, e escreve:

> quero encontrar clientes

A skill assume o comando: faz-te as perguntas, define contigo os critérios, encontra e pontua os negócios, e grava o `leads.csv` + o tracker nessa pasta.

---

## Problemas comuns

| Sintoma | Solução |
|---|---|
| `claude: command not found` | Fecha e reabre o terminal. Se persistir, repete o Passo 1. |
| A skill não dispara | Confirma que o ficheiro está exatamente em `~/.claude/skills/cz-scraping/SKILL.md` e reinicia o Claude Code. |
| "não tenho acesso à web" | Diz-lhe para usar o caminho manual: pesquisas tu no Google Maps e colas a lista. A skill sabe continuar a partir daí. |
