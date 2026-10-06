# Site do Nebula

Página de apresentação do Nebula:
transmissão de tela em até 4K, voz e chat, salas dos amigos ao vivo e mensagens criptografadas, direto de PC para PC.

É uma página estática, sem etapa de build:

- `index.html`: a página inteira (HTML e [Tailwind](https://tailwindcss.com) pelo CDN, fontes Sora e Share Tech Mono do
  Google Fonts). As cores são as do app: o fundo do tema Carta Estelar e as três estrelas da logo.
- `assets/videos/`: os vídeos de cada recurso (MP4 H.264, 1280×720) e as capas em JPEG. Foram gravados com o próprio
  app numa sala de demonstração, com nomes fictícios e telas transmitidas simuladas.
- `assets/nebula-icone.png`: o ícone do app (favicon).

Os vídeos só baixam e tocam quando aparecem na tela; quem pede menos movimento no sistema vê a capa e os controles.

## Ver no PC

Sirva a pasta (os vídeos não tocam abrindo o arquivo direto em alguns navegadores):

```sh
python -m http.server 8123
```

e abra http://localhost:8123.

## Publicar

Em **Settings → Pages** do repositório, escolha "Deploy from a branch", branch `main`, pasta `/ (root)`. O arquivo
`.nojekyll` faz o GitHub servir a página como está.

Os botões de download baixam o instalador (`Nebula.Instalador.exe`), com a versão portátil (`Nebula.exe`) como
alternativa. Fora do Windows, levam à pergunta das plataformas.
