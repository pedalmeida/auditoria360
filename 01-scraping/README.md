# 🎯 Cliente Zero · Módulo 1 - Scraping, Qualificação & Cold Call

**Dá-lhe um nicho e uma cidade. Ele encontra negócios locais reais, pontua-os pelos teus critérios, devolve-te uma lista pronta a trabalhar no Excel, e já te dá o script para ligares ao melhor lead. Sem instalar nada, sem gastar um cêntimo.**

Toda a gente que quer arrancar uma agência ou um serviço trava no mesmo sítio: "quem é que eu contacto, e o que digo quando ligar?". Passas horas no Google Maps a copiar nomes para uma folha sem critério nenhum, e mesmo com a lista feita, ainda tens de inventar o que dizer na primeira chamada. Este módulo fecha o ciclo todo: encontra, **qualifica** (cada negócio leva uma pontuação, tem um problema visível? tem dinheiro? consigo falar com uma pessoa?), e entrega o **script de cold call** pronto para o lead do topo, com a estrutura que uso de verdade (abertura sem nome, uma observação específica, o convite com fecho de desqualificação, dois slots concretos). Dizes que sim, e ele avança logo para o lead seguinte.

É o módulo 1 de uma série modular. Sozinho, já te leva da lista ao telefone. Encadeado com os próximos (auditoria + mensagem escrita), leva-te até uma reunião marcada por qualquer canal.

---

## A série Cliente Zero

| Módulo | O que faz | Entrega |
|---|---|---|
| **1. Scraping + Cold Call** (este) | Encontra e qualifica negócios locais reais, gera o script de cold call do melhor lead | `leads.csv` + tracker + script de cold call |
| **2. Auditoria** (a seguir) | Check-up à presença digital do melhor alvo, com o logótipo dele | `checkup.html` branded |
| **3. Outreach** (a seguir) | A mensagem que abre a porta, pronta a enviar | draft no Gmail + follow-ups |

Cada um funciona **sozinho**. Ou instalas os três e **encadeias**: a lista alimenta a auditoria, a auditoria alimenta a mensagem. Tu escolhes.

---

## Como usar (2 caminhos)

**Caminho A, sem instalar nada (2 min):**
1. Abre um chat novo no **Claude.ai** (grátis), **Claude Code** ou **ChatGPT**.
2. Cola o conteúdo de [`00-wizard.md`](./00-wizard.md).
3. Responde às perguntas. Ele devolve-te o CSV e o tracker para gravares.

**Caminho B, como skill do Claude Code (5 min, a experiência completa):**
1. Instala o Claude Code e a skill: vê [`instalar.md`](./instalar.md).
2. Num chat do Claude Code, escreve: *"quero encontrar clientes"*.
3. A skill grava o `leads.csv` e o tracker direto no teu computador.

Não precisas de nenhuma API. Se um dia quiseres volume (50+ leads), vê [`apis-opcionais.md`](./apis-opcionais.md).

---

## O que está aqui

| Ficheiro | O que é |
|---|---|
| [`00-wizard.md`](./00-wizard.md) | **O prompt principal.** Cola-o em qualquer chat de IA. Começa aqui. |
| [`skill/SKILL.md`](./skill/SKILL.md) | A mesma lógica como skill instalável do Claude Code. |
| [`instalar.md`](./instalar.md) | Instalar o Claude Code + a skill, passo a passo (5 min). |
| [`apis-opcionais.md`](./apis-opcionais.md) | Google Places e Apify para escalar. 100% opcional. |

---

## O output (o que sais com)

Um ficheiro `leads.csv` que abre no Excel/Sheets, com uma linha por negócio verificado e estas colunas:

`slug, nome, cidade, site, instagram, google_rating, google_reviews, ultimo_post, contacto, canal_contacto, score_gap, score_dinheiro, score_contactavel, score_total, notas`

Ordenado pelo score. Mais um `tracker.md` para acompanhares o estado de cada lead, e um `scripts/<lead>-cold-call.md` com o script de cold call do melhor lead (abertura, observação específica, convite, marcação de slots, objeções mais prováveis). É o mesmo formato que os módulos 2 e 3 leem, por isso encadeia sem fricção.

## Precisa de pagar alguma coisa?

**Não.** O caminho base usa pesquisa web e Google Maps, grátis. O plano grátis do Claude.ai chega para começar. APIs pagas (Google Places, Apify) são só para volume e têm créditos grátis generosos.

## Regras (levadas a sério)

- **Negócios reais apenas.** Cada linha é verificada. Nada é inventado; o que não se sabe fica "n/d".
- **Qualificar é o valor.** Não entrega volume, entrega discernimento.

---

## Quem fez isto

Pedro Almeida. Construo sistemas de IA para negócios reais e mostro o processo no Instagram.
