# APIs opcionais - só para quem quer afiar os dados

> **Não precisas de nada disto para a auditoria.** O caminho base (pesquisa web + páginas públicas) chega perfeitamente para auditar 1 a 2 negócios por dia, que é o ritmo certo quando estás a trabalhar leads a fundo. Vem cá só se quiseres dados da ficha do Google mais estruturados, ou se estiveres a auditar em volume.

---

## Quando faz sentido

| Situação | Precisa de API? |
|---|---|
| Auditar 1-2 negócios por dia, a fundo | ❌ Não. Pesquisa web e páginas públicas chegam. |
| Dados exatos da ficha do Google (rating, nº avaliações, horários) em vários negócios | ✅ Google Places (afia; não é obrigatório) |
| Insights que só o dono vê (alcance do Instagram, cliques na ficha, histórico completo de avaliações) | ⚠️ Nenhuma API pública dá isto. Só com acesso do dono. Fica honestamente "precisa de acesso do dono" na auditoria. |

A auditoria funciona 100% sem isto. A API só torna o Passo 1 (ficha do Google) mais rápido e mais exato quando o volume aperta.

---

## Google Places API (dados da ficha do Google, limpos)

O que dá: rating, nº de avaliações, telefone, site, horários e categoria de um negócio, direto da fonte, sem depender do que aparece na pesquisa.

Custo real: a Google dá **crédito mensal grátis** que cobre milhares de pesquisas por mês. Para auditar leads um a um, na prática pagas zero.

Setup (10 min, uma vez):
1. Vai a [console.cloud.google.com](https://console.cloud.google.com) e cria um projeto (conta Google normal serve).
2. Ativa a **Places API** (menu "APIs & Services" → "Enable APIs").
3. Cria uma chave em "Credentials" → "Create credentials" → "API key".
4. Guarda a chave num ficheiro no teu computador (ex: `~/.config/google-places-api-key`), **nunca a coles em chats públicos nem a ponhas em código partilhado**.
5. Diz ao Claude Code: *"tenho uma chave da Places API em ~/.config/google-places-api-key, usa-a para os dados da ficha do Google deste negócio"*. Ele sabe o que fazer.

---

## O que NENHUMA API te dá (e porquê a honestidade importa)

Alcance do Instagram, impressões, quantas pessoas clicaram no "como chegar" da ficha, o histórico completo das avaliações: isto vive atrás do login do dono. Nenhuma API pública to entrega. A auditoria trata isto como deve: marca "precisa de acesso do dono" em vez de inventar um número. Um check-up que inventa dados perde a credibilidade toda no momento em que o dono percebe. Vale mais dizer "não consegui ver isto" do que arriscar um número errado.

---

## Regra de segurança (leva a sério)

Uma chave de API é uma senha. **Nunca** a coles numa conversa que possas vir a partilhar, num print, num repositório público. Ficheiro local + referência ao caminho, sempre. Se uma chave escapar, revoga-a e cria outra (a consola deixa fazer isso num clique).
