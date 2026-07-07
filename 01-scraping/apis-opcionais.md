# APIs opcionais - só para quem quer escalar

> **Não precisas de nada disto para começar.** O caminho base (pesquisa web + Google Maps) é grátis e chega para trabalhar 1 a 2 leads por dia, que é exatamente o ritmo certo no início. Vem cá quando estiveres a fazer 20+ leads por semana e a pesquisa manual começar a ser o gargalo.

---

## Quando faz sentido

| Situação | Precisa de API? |
|---|---|
| Primeiros 10-20 leads, 1 nicho, 1 cidade | ❌ Não. Pesquisa web chega. |
| Listas grandes (50+ leads), vários nichos ou cidades | ✅ Google Places |
| Dados de Instagram em volume (seguidores, posts, engagement) | ✅ Apify |

---

## Opção 1 - Google Places API (listas de negócios com dados limpos)

O que dá: listas completas de negócios por categoria e zona, com rating, nº de avaliações, telefone, site e horários, direto da fonte.

Custo real: a Google dá **crédito mensal grátis** que cobre milhares de pesquisas por mês. Para este uso, na prática pagas zero.

Setup (10 min, uma vez):
1. Vai a [console.cloud.google.com](https://console.cloud.google.com) e cria um projeto (conta Google normal serve).
2. Ativa a **Places API** (menu "APIs & Services" → "Enable APIs").
3. Cria uma chave em "Credentials" → "Create credentials" → "API key".
4. Guarda a chave num ficheiro no teu computador (ex: `~/.config/google-places-api-key`), **nunca a coles em chats públicos nem a ponhas em código partilhado**.
5. Diz ao Claude Code: *"tenho uma chave da Places API em ~/.config/google-places-api-key, usa-a para procurar os leads"*. Ele sabe o que fazer.

## Opção 2 - Apify (scraping de Instagram e Maps em volume)

O que dá: "actors" prontos (Google Maps Scraper, Instagram Profile Scraper) que devolvem centenas de resultados estruturados de uma vez.

Custo real: tem plano grátis com crédito mensal para experimentar; depois disso, uma pesquisa típica de Maps custa cêntimos. Define um limite de gastos na conta no primeiro dia.

Setup (5 min):
1. Cria conta em [apify.com](https://apify.com) (grátis).
2. Vai a Settings → Integrations e copia o teu **API token**.
3. Guarda-o como acima (ficheiro local, nunca em chats públicos).
4. Diz ao Claude Code: *"tenho um token do Apify em <caminho>, usa o Google Maps Scraper para puxar <nicho> em <cidade>"*.

---

## Regra de segurança (leva a sério)

Uma chave de API é uma senha. **Nunca** a coles numa conversa que possas vir a partilhar, num print, num repositório público. Ficheiro local + referência ao caminho, sempre. Se uma chave escapar, revoga-a e cria outra (ambas as consolas deixam fazer isso num clique).
