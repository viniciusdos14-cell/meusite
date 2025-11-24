# MeuSite — Landing Page

Este repositório contém uma landing page simples e responsiva construída com HTML, CSS e JavaScript puro.

## Estrutura

- `index.html` — arquivo principal da landing page

## Como pré-visualizar

Escolha uma das opções abaixo para abrir o projeto localmente.

- Abrir direto no navegador (rápido):

```pwsh
# No PowerShell, a partir da pasta do projeto
cd 'c:\Users\Mvini\MeusProjetos\meusite'
Start-Process .\index.html
```

- Usar servidor HTTP simples com Python (recomendado):

```pwsh
cd 'c:\Users\Mvini\MeusProjetos\meusite'
python -m http.server 8000
# Depois abra http://localhost:8000
```

- Usar `http-server` (Node.js):

```pwsh
npm install -g http-server
cd 'c:\Users\Mvini\MeusProjetos\meusite'
http-server -c-1 -p 8000
# Depois abra http://localhost:8000
```

## Comportamento dos formulários

Os formulários de contato e teste grátis usam `alert()` no frontend apenas para demonstração — não enviam dados para nenhum servidor.

Se quiser capturar leads reais, sugerimos integrar com um serviço como Formspree, Netlify Forms ou um backend próprio.

Exemplo rápido com Formspree:

1. Crie uma conta em https://formspree.io e obtenha o endpoint de formulário.
2. Substitua o atributo `onsubmit` do formulário por um `action` para o endpoint e `method="POST"`.

## Próximos passos recomendados

- Integrar captura de leads (Formspree, Netlify, ou API própria)
- Adicionar imagens e logo otimizados
- Configurar meta tags para SEO e OpenGraph
- Automatizar build (se transformar em projeto com bundler)

## Vídeo de fundo (sem direitos autorais)

Você pode adicionar um vídeo de fundo em loop colocando um arquivo `MP4` em `assets/bg.mp4` e um `poster` em `assets/bg-poster.jpg`.

Fontes gratuitas e sem direitos autorais (verifique a licença específica antes de usar):

- Pexels Videos (https://www.pexels.com/videos/) — muitos vídeos gratuitos para uso comercial.
- Pixabay Videos (https://pixabay.com/videos/) — vídeos com licença Pixabay (uso livre).
- Coverr (https://coverr.co/) — vídeos para fundos de sites, gratuitos.

Recomendações de formato:

- Formato: `MP4` (H.264) para melhor compatibilidade.
- Resolução: 720p ou 1080p (1080p para melhor qualidade, mas aumenta o tamanho).
- Otimização: compacte o vídeo para web (criar versão ~1–5MB dependendo da duração).

Exemplo de uso:

1. Baixe um vídeo de uma das fontes acima e salve como `assets/bg.mp4`.
2. (Opcional) Gere uma imagem `assets/bg-poster.jpg` para fallback quando o vídeo não for reproduzido.
3. Abra `index.html` — a página já inclui a marcação para usar `assets/bg.mp4` como fundo.

Se preferir não hospedar o arquivo localmente, você pode apontar o `src` para uma URL externa de um vídeo (nem todos os hosts permitem hotlinking).

Se quiser, eu posso:

- Buscar um vídeo CC0/gratuito e adicioná-lo ao projeto (faça upload ou autorize que eu adicione o link)
- Gerar uma versão otimizada do vídeo (recomendado para performance)


## Contato

Se quiser, posso:

- Integrar a captura de leads com Formspree (configuro o formulário)
- Gerar arquivos de imagem/ícone e melhorar o design
- Converter para um projeto com React/Vite

Diga o que prefere que eu faça a seguir.
