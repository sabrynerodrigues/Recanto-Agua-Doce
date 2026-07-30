# Site do Sítio Recanto Água Doce — como usar

Você tem duas páginas prontas:

- **index.html** — a página principal
- **regras.html** — regras e informações completas

Para ver o site, é só dar dois cliques no `index.html`. Ele abre no navegador e funciona sem internet (só as fontes e o feed dependem de conexão).

---

## 1. Colocar as fotos

Dentro desta pasta existe uma pasta chamada **`fotos`**. É só colocar as suas fotos lá dentro **com exatamente estes nomes** — o site encontra sozinho, sem precisar mexer no código.

Enquanto a foto não estiver lá, aparece uma moldura tracejada dizendo qual foto vai naquele lugar. Isso é proposital: assim você vê o site inteiro funcionando e vai preenchendo aos poucos.

| Nome do arquivo | Onde aparece | O que deve mostrar |
|---|---|---|
| `01-capa.jpg` | Capa, tela cheia | A melhor foto do sítio. Piscina com verde ao redor, ou o rio. **Horizontal e bem larga.** É a mais importante de todas |
| `02-piscina.jpg` | O sítio → A piscina | Piscina, ângulo amplo, dia de sol |
| `03-rio.jpg` | O sítio → O rio | O rio, com a água correndo e o verde em volta |
| `04-quarto.jpg` | O sítio → Os quartos | Um quarto, mostrando camas e beliches. Luz natural |
| `05-banheiro.jpg` | O sítio → Os banheiros | Um banheiro. Pode ser simples — o importante é ser real |
| `06-salao.jpg` | O sítio → O salão | O salão, ângulo amplo. Se tiver foto dele montado para evento, melhor ainda |
| `07-area-externa.jpg` | O sítio → Área externa | Forno e fogão a lenha, verde, sombra |
| `08-fim-de-tarde.jpg` | Galeria (foto grande) | Fim de tarde no sítio, ou a vista mais bonita que você tiver |
| `09-churrasqueira.jpg` | Galeria | A churrasqueira |
| `10-cozinha.jpg` | Galeria | A cozinha inteira |
| `11-eletrodomesticos.jpg` | Galeria | Bancada com os eletrodomésticos à vista |
| `12-quarto-2.jpg` | Galeria | Segundo quarto (beliches) |
| `13-quarto-3.jpg` | Galeria | Terceiro quarto |
| `14-sala.jpg` | Galeria | Sala / estar da casa |
| `15-banheiro-2.jpg` | Galeria | Outro banheiro |
| `16-varanda.jpg` | Galeria | Varanda ou área de convivência |
| `17-piscina-2.jpg` | Galeria | Outro ângulo da piscina |
| `18-rio-2.jpg` | Galeria | Outro ângulo do rio |
| `19-acesso-rio.jpg` | Galeria | A escada de acesso ao rio |
| `20-um-dia.jpg` | Seção "Um dia por aqui" | **Vertical.** A piscina, o rio ou o salão cheio — a que melhor mostrar o clima de um dia no sítio |
| `21-caminho.jpg` | A região | A chegada, a porteira ou a estrada — **vertical** |
| `22-insta-1.jpg` a `25-insta-4.jpg` | Instagram | Quatro fotos do perfil |

### Três cuidados com as fotos

1. **Nenhuma foto pode identificar o endereço.** Sem placa, número, nome de estrada ou vista que entregue a localização. O site inteiro foi feito para não revelar onde fica.
2. **Comprima antes de subir.** Foto direto do celular pesa 5 MB e deixa o site lento no 4G — que é como quase todo mundo vai abrir. Use o [squoosh.app](https://squoosh.app) (gratuito, no navegador) e deixe cada foto com no máximo **300 KB**. Para a capa, até 500 KB.
3. **Tem que ser `.jpg`.** Se a sua foto for `.jpeg`, `.png` ou `.HEIC`, renomeie ou converta — o nome precisa bater exatamente.

---

## 2. O terceiro depoimento

Os depoimentos do Zenildo e da Isabela já estão no site. Falta só o terceiro.

Abra o `index.html` em qualquer editor de texto (o Bloco de Notas serve) e procure por `COLE AQUI`. Você vai achar isto:

```html
<p>[COLE AQUI o terceiro depoimento...]</p>
<cite>Nome<small>Hóspede do Recanto</small></cite>
```

Substitua pelo texto real e pelo primeiro nome da pessoa. Se quiser trocar o "Hóspede do Recanto" por um mês e ano, também dá.

**Não invente depoimento.** O site inteiro existe para gerar confiança — um depoimento falso derruba isso na hora, e as pessoas percebem.

---

## 3. Publicar

O site é estático: não precisa de servidor, banco de dados nem mensalidade. O único custo é o domínio.

**Domínio** — registre no [registro.br](https://registro.br) em nome da S & B. Custa cerca de R$ 40 por ano. Sugestões:

- `recantoaguadoce.com.br`
- `sitiorecantoaguadoce.com.br`

**Hospedagem gratuita** — a opção mais simples é o [Netlify Drop](https://app.netlify.com/drop): você arrasta esta pasta inteira para a página e o site fica no ar em segundos, já com cadeado de segurança (HTTPS). Depois é só apontar o seu domínio nas configurações. O [Cloudflare Pages](https://pages.cloudflare.com) e o [Vercel](https://vercel.com) funcionam do mesmo jeito.

---

## 4. Depois de publicar

**Google Meu Negócio** é provavelmente o que mais vai trazer contato novo — mais até que o site. É o que faz o sítio aparecer quando alguém pesquisa "sítio para alugar Cruzeiro SP".

> ⚠️ **Importante:** ao cadastrar, escolha a opção de **negócio que atende em uma área de serviço**, e não a de negócio com endereço físico. Se escolher errado, o Google publica o endereço do sítio no mapa — exatamente o que o site foi feito para evitar.

Depois, cadastre o site no **Google Search Console** e instale o **Google Analytics** (os dois são gratuitos) para acompanhar quantas pessoas clicam no WhatsApp.

---

## O que o site propositalmente NÃO tem

Nada disso é esquecimento — foi decidido assim:

- **Preços.** Todo orçamento sai pelo WhatsApp, pernoite e evento. Os botões já vão com mensagem diferente para cada um, então você recebe a conversa já sabendo qual é
- **Endereço, mapa ou coordenada.** Só a região e os tempos de deslocamento. O endereço e o vídeo do caminho vão no guia do hóspede, depois da reserva confirmada
- **Calendário de disponibilidade e reserva online.** Aumentaria muito a manutenção sem resolver nada que o WhatsApp não resolva

---

## Se quiser mudar alguma coisa

Todos os textos estão dentro dos próprios arquivos `.html`, em português e sem código no meio. Dá para abrir no Bloco de Notas e editar direto. As cores estão todas no começo do arquivo, no bloco `:root` — mudar ali muda o site inteiro de uma vez.

**Antes de mexer, faça uma cópia do arquivo.** Se algo quebrar, você volta.
