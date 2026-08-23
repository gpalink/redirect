# Como usar seu redirecionador

Você tem 2 arquivos principais:

- **index.html** → a página que redireciona (não precisa mexer nela nunca)
- **destino.js** → o único arquivo que você edita quando quiser trocar o link

## Passo 1 — Colocar online (grátis, via GitHub Pages)

1. Crie uma conta gratuita em https://github.com (se ainda não tiver).
2. Crie um novo repositório (pode ser público), ex: `meu-redirect`.
3. Faça upload dos dois arquivos (`index.html` e `destino.js`) para esse repositório.
4. Vá em **Settings > Pages**, e em "Branch" selecione `main` e salve.
5. Em alguns minutos, o GitHub vai te dar um link tipo:
   `https://seu-usuario.github.io/meu-redirect/`

Esse link é o que você vai colocar no QR code.

## Passo 2 — Gerar o QR code

Use qualquer gerador (ex: qrcode-monkey.com, ou eu mesmo posso gerar aqui) apontando
para o link do GitHub Pages acima. Você só cria o QR code **uma vez**.

## Passo 3 — Trocar o destino quando quiser

Sempre que precisar mudar para onde o QR code leva:

1. No GitHub, abra o arquivo `destino.js`.
2. Edite a linha:
   ```js
   const DESTINO = "https://www.google.com";
   ```
   trocando pela nova URL.
3. Salve (commit). Em segundos a mudança já vale — o QR code continua o mesmo.

Pronto — o QR code nunca muda, só o conteúdo de `destino.js`.
