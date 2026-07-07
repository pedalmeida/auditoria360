# Auditoria de presença digital - Clínica Dentária X (Portimão)

> Exemplo real, anonimizado. Uma clínica dentária independente em Portimão, a operar desde 2007, auditada só com informação pública. Nome, logótipo e contactos removidos; os factos e a estrutura são o output verdadeiro da skill. Só sobre presença digital, sem qualquer juízo sobre a qualidade clínica.

**Auditado em:** exemplo. **Fontes:** site (aberto em browser), ficha do Google, Facebook.

---

## O que observei (por eixo)

**Site**
- Abre e é responsivo no telemóvel (testado a 375px). Feito em WordPress, formulário via Contact Form 7.
- Tem telefones clicáveis e WhatsApp funcional (botão flutuante, 1 clique). Boa base.
- Não há marcação online real: o botão "MARCAR CONSULTA" faz scroll para um formulário de contacto genérico, sem calendário nem escolha de horário.
- Bug verificável: um dos botões "MARCAÇÕES" aponta para uma âncora errada (leva a uma secção que não é o contacto).
- Acima da dobra no telemóvel não há telefone clicável direto, só botões de âncora.

**Ficha do Google**
- Rating 4,3 (verificado, screenshot). Sem foto de capa (convite "Adicione fotos e vídeos" ativo) e sem contador de avaliações visível junto ao rating. Nº exato de avaliações: não consegui confirmar.

**Facebook**
- Ativo, com publicação recente. "Ainda sem classificação (0 críticas)" no Facebook. Frequência de publicação não confirmável (login wall).

**Instagram + ligação site→redes**
- Gap duro e verificável: no HTML do site, os ícones de rede social apontam para um placeholder (`http://url`, 4 ocorrências) que nunca foi preenchido. Quem clica no ícone de Instagram cai numa página de erro. O perfil de Instagram associado está vazio (0 posts).

---

## 3 problemas que custam dinheiro

1. **Ficha do Google sem fotos e com poucas avaliações visíveis.**
   Facto: a ficha mostra 4,3 sem contador de reviews e sem foto de capa ("Adicione fotos e vídeos" ativo).
   O que custa (inferência): fichas sem fotos e com poucas reviews convertem pior no local pack e ganham menos cliques que concorrentes com galeria e dezenas de avaliações. Perdem-se marcações de quem pesquisa "dentista Portimão".
   Como se resolve: pedir review no Google no fim da consulta (link/QR na receção), carregar 10-15 fotos reais (instalações, equipa), responder às reviews existentes.

2. **Não há marcação online real, só formulário de contacto.**
   Facto: o CTA "MARCAR CONSULTA" leva a um formulário, sem calendário nem escolha de horário.
   O que custa (inferência): pacientes que preferem marcar fora do horário de atendimento (noite/fim de semana) desistem se só houver "deixe o contacto e ligamos". Perde-se a marcação de impulso.
   Como se resolve: adicionar um sistema de marcação com disponibilidade real, ou pelo menos destacar o WhatsApp como via de marcação rápida.

3. **Instagram do site partido e perfil vazio.**
   Facto: 4 ocorrências de um link placeholder (`http://url`) no HTML; o perfil de Instagram associado tem 0 posts.
   O que custa (inferência): a clínica tem um ícone de Instagram que só gera frustração (clique em erro) e não capta seguidores. Perde prova social junto de um público jovem/estético que valoriza o Instagram na escolha de dentista.
   Como se resolve: ligar o ícone ao perfil correto e publicar com regularidade, ou remover o ícone (melhor não ter do que ter partido).

## 3 quick wins

1. **Corrigir o botão "MARCAÇÕES" que leva à âncora errada.** Quem clica é levado para a secção errada em vez do formulário e alguns desistem. Edição de 1 minuto no WordPress.
2. **Arranjar ou remover os ícones sociais partidos (`http://url`).** Apontar o Facebook para a página real (já existe) e o Instagram para o perfil real, ou removê-los. Cliques desperdiçados em erro passam imagem de descuido.
3. **Pôr telefone/WhatsApp clicável acima da dobra no mobile.** Acima da dobra só há botões de âncora. Um botão fixo "Ligar" (`tel:`) no cabeçalho mobile, além do WhatsApp que já existe, tira fricção a quem só quer ligar já.

## Por onde eu começaria

Pela ficha do Google. É a montra que decide quem clica quando alguém pesquisa "dentista Portimão", e está a jogar em desvantagem sem fotos e com poucas avaliações. Carregar 10-15 fotos e pôr um QR de avaliação na receção é trabalho de uma tarde, e é o que mais rápido converte procura existente em marcações.

---

*Nota de honestidade: nº exato de avaliações do Google, frequência de publicação no Facebook e a titularidade do perfil de Instagram ficaram por confirmar (login walls / bio vazia) e estão marcados como tal. Durante a auditoria corrigi uma primeira leitura que parecia indicar "sem redes"; ao abrir o site confirmei que o Facebook e o WhatsApp funcionam, e que o gap real é só o Instagram partido.*
