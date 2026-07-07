# 🎯 Cliente Zero

**Do zero (sem clientes) a uma reunião marcada, usando IA. Uma série de skills modulares para o Claude Code, cada uma corre sozinha ou encadeada com as outras. Sem instalar nada complicado, sem gastar um cêntimo, sem nenhuma API paga.**

Toda a gente que quer arrancar uma agência ou um serviço trava no mesmo sítio: "quem contacto, e o que digo?". Esta série fecha esse ciclo. Encontra negócios locais reais e qualifica-os, prepara um entregável profissional que dás antes de pedires nada, e escreve a mensagem que abre a porta. Cada peça é uma skill instalável (ou um prompt que colas num chat), pensada para quem nunca abriu um terminal na vida, mas com o teto alto para quem quer levar a IA ao limite.

Feito por [Pedro Almeida](https://instagram.com/pedroalmeida_ai). Construo sistemas de IA para negócios reais e mostro o processo no Instagram.

---

## Os módulos

| Módulo | O que faz | Entrega | Estado |
|---|---|---|---|
| [**01 · Scraping + Cold Call**](./01-scraping/) | Encontra e qualifica negócios locais reais, gera o script de cold call do melhor lead | `leads.csv` + tracker + script de cold call | ✅ Pronto |
| [**02 · Auditoria**](./02-audit/) | Check-up à presença digital do alvo, com o logótipo e as cores dele | `checkup.html` branded + `audit.md` | ✅ Pronto |
| **03 · Outreach** | A mensagem que abre a porta, pronta a enviar | draft + follow-ups | 🔜 A caminho |

Cada módulo funciona **sozinho**. Ou instalas os três e **encadeias**: a lista alimenta a auditoria, a auditoria alimenta a mensagem. Comunicam por ficheiros numa pasta previsível, nenhum depende dos outros estarem instalados.

---

## Como começar (2 caminhos)

**Sem instalar nada (o mais rápido):** abre o módulo que te interessa, copia o `00-wizard.md` de lá, e cola-o num chat do [Claude.ai](https://claude.ai) (grátis) ou do ChatGPT com pesquisa web ativada. Respondes a umas perguntas e tens o output.

**Como skill do Claude Code (a experiência completa):** cada módulo tem um `instalar.md` com o passo a passo (5 min, escrito para quem nunca usou um terminal). Instalas a skill uma vez e depois basta pedir em linguagem normal ("quero encontrar clientes", "audita este negócio").

Começa pelo módulo [01-scraping](./01-scraping/) se ainda não tens lista, ou pelo [02-audit](./02-audit/) se já tens um negócio em mente.

---

## Precisa de pagar alguma coisa?

**Não.** O caminho base usa só pesquisa web e páginas públicas, que qualquer chat de IA com navegação já tem. O plano grátis do Claude.ai chega para começar. Cada módulo tem um `apis-opcionais.md` para quem, mais tarde, quiser escalar em volume (Google Places, Apify), sempre 100% opcional e com créditos grátis generosos.

## Regras da série (levadas a sério)

- **Negócios reais apenas.** Nada é inventado. O que não se sabe fica marcado, nunca preenchido a adivinhar.
- **Factos ligam a evidência** (URL, número, data). Deduções vão marcadas como tal.
- **Dar antes de pedir.** A auditoria é um presente. Nunca se pede a venda, pede-se a conversa.
- **A skill nunca envia nada.** Prepara tudo, tu carregas no botão.

---

## Licença

MIT. Usa, adapta, aprende. Se te for útil, [segue-me no Instagram](https://instagram.com/pedroalmeida_ai) que é onde mostro como construo estas coisas.
