# Site do Tela P2P

Página de apresentação do [Tela P2P](https://github.com/MateusMunhoz/AmostradinhoScreenShare): transmissão de tela em até
4K, voz e chat, direto de PC para PC.

É uma página estática, sem etapa de build:

- `index.html`: a página inteira (HTML e [Tailwind](https://tailwindcss.com) pelo CDN, fontes Geist do Google Fonts).
- `assets/`: capturas do app em WebP. Foram geradas com o próprio app numa sala de teste, com nomes fictícios.

## Ver no PC

Abra o `index.html` no navegador, ou sirva a pasta:

```sh
python -m http.server 8123
```

e abra http://localhost:8123.

## Publicar

Em **Settings → Pages** do repositório, escolha "Deploy from a branch", branch `main`, pasta `/ (root)`. O arquivo
`.nojekyll` faz o GitHub servir a página como está.

Os botões de download apontam para a última versão em
[Releases](https://github.com/MateusMunhoz/AmostradinhoScreenShare/releases/latest).
