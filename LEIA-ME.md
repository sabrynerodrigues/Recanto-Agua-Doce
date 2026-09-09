# Site do Recanto Água Doce — pasta pronta para deploy

Domínio: **recantoaguadoce.com.br**

## O que tem aqui

- `index.html` — a home inteira, sem dependência externa além das fontes do Google
- `img/` — as 17 fotos, em arquivos separados
- `favicon.svg` — o emblema do brandkit, em sálvia sobre areia
- `robots.txt` — libera o site e **bloqueia `/guia/`**
- `sitemap.xml` — só a home, que é a única página pública
- `vercel.json` — cache longo nas imagens e `noindex` em tudo que estiver sob `/guia/`

## Como subir no Vercel

1. No painel do Vercel: **Add New > Project > Deploy** (ou arraste esta pasta em vercel.com/new).
2. Framework preset: **Other**. Sem build command, sem output directory.
3. Em **Settings > Domains**, adicione `recantoaguadoce.com.br` e `www.recantoaguadoce.com.br`.
4. No registrador do domínio, aponte os registros que o Vercel indicar (normalmente um `A` para o apex e um `CNAME` para o www).

## O guia do hóspede

Quando ficar pronto, ele entra como `guia/agua-doce-2026/index.html` e fica acessível em
`recantoaguadoce.com.br/guia/agua-doce-2026`.

**Endereço não listado, de propósito:** o guia carrega o endereço exato, a senha do Wi-Fi e o vídeo
do trajeto. Por isso ele **não é linkado de lugar nenhum do site**, está bloqueado no `robots.txt` e
recebe `noindex` pelo `vercel.json`. O link vai para o hóspede junto com o contrato, depois da
reserva confirmada.

Se um dia o link vazar, é só renomear a pasta — o endereço muda e o antigo morre.

## Antes de apontar o domínio

Teste no celular a seção "Consultar disponibilidade": o botão precisa abrir o WhatsApp com a
mensagem escrita e terminando na última frase, sem nada colado no fim.
