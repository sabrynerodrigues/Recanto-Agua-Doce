# Recanto Água Doce — pasta pronta para deploy

Domínio: **recantoaguadoce.com.br** · Deploy: Vercel ligado ao repositório do GitHub
(cada push republica sozinho).

## O que tem aqui

- `index.html` — a home inteira, sem dependência externa além das fontes do Google
- `img/` — as 17 fotos, em arquivos separados
- `guia/agua-doce-2026/index.html` — o guia do hóspede
- `favicon.svg` — o emblema do brandkit, em sálvia sobre areia
- `robots.txt` — libera o site e **bloqueia `/guia/`**
- `sitemap.xml` — só a home, que é a única página pública
- `vercel.json` — cache longo nas imagens e `noindex` em tudo que estiver sob `/guia/`

## Como atualizar o site

Substitua os arquivos no repositório mantendo a mesma estrutura de pastas e dê push.
A pasta `guia/` fica na **raiz**, do lado do `index.html` e da pasta `img/`. A foto de capa do
guia é buscada em `/img/escada-rio.jpg`, então a pasta `img/` precisa continuar na raiz.

## O guia do hóspede

Endereço: `recantoaguadoce.com.br/guia/agua-doce-2026`

**Não listado, de propósito:** o guia carrega o endereço exato, a senha do Wi-Fi e o vídeo do
trajeto. Por isso ele **não é linkado de lugar nenhum do site**, está bloqueado no `robots.txt` e
recebe `noindex` pelo `vercel.json`. O link vai para o hóspede junto com o contrato, depois da
reserva confirmada.

Se um dia o link vazar, é só renomear a pasta `agua-doce-2026` — o endereço muda e o antigo morre.

O guia aponta para dois links externos:

- vídeo do trajeto, no Google Drive — precisa estar como "qualquer pessoa com o link", senão o
  hóspede recebe pedido de acesso em vez do vídeo;
- localização da caçamba do bairro, no Google Maps.

## Cuidado ao trocar uma foto

As imagens são servidas com cache de um ano (`immutable`). Se você substituir uma foto mantendo o
mesmo nome de arquivo, quem já visitou o site continua vendo a antiga por muito tempo.
**Ao trocar uma foto, mude o nome do arquivo** e atualize a referência no `index.html`.

## Ainda para testar

No celular, a seção "Consultar disponibilidade": o botão precisa abrir o WhatsApp com a mensagem
escrita e terminando na última frase, sem nada colado no fim.
