# 🎯 Cliente Zero · Módulo 2 - Auditoria & Entregável Branded

**Dá-lhe um negócio local (nome + site ou Instagram). Ele faz um check-up honesto à presença digital, encontra os problemas que custam dinheiro, e devolve-te um entregável HTML profissional com o logótipo e as cores do próprio negócio, pronto para ofereceres. Sem instalar nada, sem gastar um cêntimo, sem nenhuma API.**

Encontrar o lead é metade do caminho (isso é o módulo 1). A outra metade é chegar com algo na mão em vez de um "olá, presto serviços de marketing". Este módulo faz-te esse presente: analisa o site, a ficha do Google e o Instagram do negócio, aponta 3 problemas que lhe estão a custar clientes e 3 quick wins, e embrulha tudo num `checkup.html` com a marca deles, para parecer feito à medida. É o entregável que transforma um cold contact numa conversa: dás valor antes de pedir seja o que for.

É o módulo 2 de uma série modular. Sozinho, pega em qualquer negócio e dá-te o entregável. Encadeado com o módulo 1, audita automaticamente o melhor lead da tua lista.

---

## A série Cliente Zero

| Módulo | O que faz | Entrega |
|---|---|---|
| **1. Scraping + Cold Call** | Encontra e qualifica negócios locais reais, gera o script de cold call do melhor lead | `leads.csv` + tracker + script de cold call |
| **2. Auditoria** (este) | Check-up à presença digital do alvo, com o logótipo e as cores dele | `checkup.html` branded + `audit.md` |
| **3. Outreach** (a seguir) | A mensagem que abre a porta, pronta a enviar | draft no Gmail + follow-ups |

Cada um funciona **sozinho**. Ou instalas os três e **encadeias**: a lista alimenta a auditoria, a auditoria alimenta a mensagem. Tu escolhes.

---

## Como usar (2 caminhos)

**Caminho A, sem instalar nada (2 min):**
1. Abre um chat novo no **Claude.ai** (grátis), **Claude Code** ou **ChatGPT**, com a pesquisa web ativada.
2. Cola o conteúdo de [`00-wizard.md`](./00-wizard.md).
3. Dá-lhe o nome + site do negócio. Ele devolve-te a auditoria e o `checkup.html` para gravares.

**Caminho B, como skill do Claude Code (5 min, a experiência completa):**
1. Instala o Claude Code e a skill: vê [`instalar.md`](./instalar.md).
2. Num chat do Claude Code, escreve: *"audita este negócio"* (e cola o site), ou *"faz-me o check-up do &lt;nome&gt;"*.
3. A skill grava o `audit.md` e o `checkup.html` direto no teu computador, na pasta do lead.

Não precisas de nenhuma API. A auditoria vive de pesquisa web e páginas públicas, que qualquer chat com navegação já tem.

---

## O que está aqui

| Ficheiro | O que é |
|---|---|
| [`00-wizard.md`](./00-wizard.md) | **O prompt principal.** Cola-o em qualquer chat de IA. Começa aqui. |
| [`skill/SKILL.md`](./skill/SKILL.md) | A mesma lógica como skill instalável do Claude Code. |
| [`instalar.md`](./instalar.md) | Instalar o Claude Code + a skill, passo a passo (5 min). |
| [`apis-opcionais.md`](./apis-opcionais.md) | Google Places para dados de ficha do Google mais afiados. 100% opcional. |
| [`exemplo/`](./exemplo/) | Um check-up real (negócio anonimizado) para veres o output antes de correres. |

---

## O output (o que sais com)

Dois ficheiros, na pasta `clientes/<slug>/`:

- **`checkup.html`** - o entregável. Página única, autossuficiente (abre com duplo-clique, offline), com o logótipo e as cores do negócio. Estrutura: resumo → 3 problemas que custam dinheiro → 3 quick wins → "por onde eu começaria" (uma recomendação). É o que ofereces ao dono.
- **`audit.md`** - a auditoria em texto (factos + evidência), a matéria-prima. É o que o módulo 3 lê para escrever a mensagem.

Vê a pasta [`exemplo/`](./exemplo/) para o formato exato.

## Precisa de pagar alguma coisa?

**Não.** A auditoria usa só pesquisa web e páginas públicas (site, ficha do Google, Instagram). O plano grátis do Claude.ai chega. Se um dia quiseres dados de ficha do Google mais estruturados em volume, vê [`apis-opcionais.md`](./apis-opcionais.md), mas nunca precisas disso para começar.

## Regras (levadas a sério)

- **Só factos com evidência.** Cada problema liga a um URL, um número ou uma data. O que não se consegue verificar fica "não consegui confirmar", nunca inventado.
- **O gap tem de doer no bolso.** Só entram problemas que custam clientes, não detalhes de gosto.
- **É um presente, não um ataque.** O dono vai ler. Respeitoso, começa pelo que está bem.
- **Nunca inventa um logótipo nem uma marca.** Se não conseguir extrair o branding, usa um cabeçalho neutro e honesto.

---

## Quem fez isto

Pedro Almeida. Construo sistemas de IA para negócios reais e mostro o processo no Instagram.
