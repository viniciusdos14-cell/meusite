# MeuSite — Landing Page

Este repositório contém uma landing page simples e responsiva construída com HTML, CSS e JavaScript puro.

## 📋 Sumário

- [Visão Geral](#visão-geral)
- [Pré-requisitos](#pré-requisitos)
- [Passo a Passo para Construir o Site](#passo-a-passo-para-construir-o-site)
- [Estrutura do Projeto](#estrutura-do-projeto)
- [Personalizações](#personalizações)
- [Deploy](#deploy)

## 🎯 Visão Geral

Uma landing page moderna com:
- ✅ Design responsivo e profissional
- ✅ Vídeo de fundo com overlay
- ✅ Seção hero com call-to-action
- ✅ Recursos/features
- ✅ Planos de preços
- ✅ Depoimentos de clientes
- ✅ Formulários de contato e lead generation
- ✅ Otimização SEO
- ✅ Performance rápida

## ⚙️ Pré-requisitos

Antes de começar, você precisa ter:
- Um editor de código (VS Code, Sublime, etc.)
- Um navegador web moderno
- Git (opcional, mas recomendado)
- Node.js com npm (opcional, se quiser usar ferramentas de build)

## 🚀 Passo a Passo para Construir o Site

### Passo 1: Clonar ou Preparar o Repositório

```bash
# Se você quer clonar este repositório:
git clone https://github.com/viniciusdos14-cell/meusite.git
cd meusite

# Ou, se for criar do zero:
mkdir meusite
cd meusite
git init
```

### Passo 2: Criar a Estrutura de Pastas

```
meusite/
├── index.html          # Arquivo HTML principal
├── style.css           # Estilos da página
├── README.md           # Este arquivo
└── assets/             # Pasta para imagens e mídia
    ├── bg.mp4          # Vídeo de fundo
    └── bg-poster.jpg   # Imagem de poster do vídeo
```

Crie a pasta `assets/`:

```bash
mkdir assets
```

### Passo 3: Criar o Arquivo HTML Principal

1. Crie um arquivo chamado `index.html` na raiz do projeto
2. Este arquivo contém a estrutura HTML com:
   - **Header**: Logo, navegação
   - **Hero Section**: Título principal, subtítulo, CTA, formulário de lead
   - **Features**: Seção de recursos
   - **Pricing**: Planos de preços
   - **Testimonials**: Depoimentos de clientes
   - **Contact**: Seção de contato com formulário
   - **Footer**: Rodapé

O arquivo `index.html` já está pronto neste repositório com todos os comentários explicativos.

### Passo 4: Criar o Arquivo CSS

1. Crie um arquivo chamado `style.css` na raiz do projeto
2. Este arquivo define:
   - **Variáveis CSS**: Cores, fontes, tamanhos
   - **Layout**: Grid, flexbox, responsividade
   - **Componentes**: Botões, cards, formulários
   - **Animações**: Transições suaves
   - **Media Queries**: Ajustes para dispositivos móveis

O arquivo `style.css` já está pronto com todos os estilos necessários.

### Passo 5: Adicionar Mídia (Vídeo de Fundo)

1. Coloque um arquivo de vídeo MP4 na pasta `assets/` com o nome `bg.mp4`
2. Também adicione uma imagem de poster em `assets/bg-poster.jpg` (será exibida enquanto o vídeo carrega)

**Onde encontrar vídeos:**
- Pixabay (pixabay.com) - Vídeos grátis em 4K
- Pexels (pexels.com/videos) - Vídeos grátis de alta qualidade
- Unsplash (unsplash.com) - Alguns vídeos grátis

**Tamanho recomendado:**
- Comprimento: 10-30 segundos
- Formato: MP4 H.264
- Tamanho: 2-5 MB (para não deixar o site muito pesado)

### Passo 6: Personalizar o Conteúdo

Abra o `index.html` e edite:

**Logo e Branding:**
```html
<div class="logo">LS</div>  <!-- Mude "LS" para suas iniciais -->
<div style="font-weight:700">Land Page Do futuro</div>  <!-- Título da sua empresa -->
```

**Textos da Hero Section:**
```html
<h1>Seu título principal aqui</h1>
<p>Sua descrição aqui</p>
```

**Recursos:**
Edite os 3 cards de features com seu conteúdo:
```html
<h3>Seu recurso aqui</h3>
<p style="color:var(--muted)">Descrição do recurso</p>
```

**Planos de Preço:**
Atualize os preços e descrições dos 3 planos:
```html
<strong>Nome do Plano</strong>
<div style="color:var(--muted);margin:8px 0">Descrição do plano</div>
```

**Depoimentos:**
Adicione depoimentos reais de clientes:
```html
"Seu depoimento aqui"
<div style="color:var(--muted);margin-top:8px">— Nome, Segmento</div>
```

**Contato:**
Atualize seus dados de contato:
```html
<p style="color:var(--muted);margin-top:8px">Email: seu-email@exemplo.com</p>
<p style="color:var(--muted);margin-top:4px">Telefone: +55 11 99999-9999</p>
```

### Passo 7: Testar Localmente

1. Abra o arquivo `index.html` no seu navegador:
   - Duplo clique no arquivo, OU
   - Clique com botão direito → "Abrir com" → Seu navegador

2. Verifique se tudo está funcionando:
   - ✅ Vídeo de fundo aparece
   - ✅ Menu de navegação está responsivo
   - ✅ Formulários funcionam
   - ✅ Botões abrem seções corretas
   - ✅ Layout adapta em celular

**Dica**: Use a ferramenta de desenvolvedor (F12) para testar em diferentes resoluções.

### Passo 8: Funcionalidades JavaScript

O arquivo `index.html` já contém funções JavaScript para:

- **submitLead()**: Processa o formulário de lead generation (seção hero)
- **submitContact()**: Processa o formulário de contato

Atualmente, exibem um alerta. Para integração real com backend/API:
```javascript
// Enviar dados para seu servidor/API
fetch('https://seu-api.com/leads', {
  method: 'POST',
  headers: { 'Content-Type': 'application/json' },
  body: JSON.stringify({ name, email })
})
```

### Passo 9: Publicar na Web

**Opção 1: Netlify (Recomendado - Grátis)**
1. Acesse [netlify.com](https://netlify.com)
2. Faça login com GitHub
3. Clique em "New site from Git"
4. Selecione seu repositório
5. Configure:
   - Build command: (deixe em branco)
   - Publish directory: `.` (raiz)
6. Clique em "Deploy site"

**Opção 2: Vercel**
1. Acesse [vercel.com](https://vercel.com)
2. Conecte seu repositório GitHub
3. Clique em "Import"
4. Vercel fará deploy automático

**Opção 3: GitHub Pages**
1. Push seu código para GitHub
2. Vá em Settings → Pages
3. Selecione "Deploy from a branch"
4. Escolha branch `main` e pasta `/root`
5. Seu site estará em `https://seu-usuario.github.io/meusite`

### Passo 10: Domínio Personalizado (Opcional)

1. Compre um domínio em:
   - GoDaddy
   - Namecheap
   - Google Domains
   - Registro.br (se for .br)

2. Configure os nameservers para apontar para sua hospedagem
3. Na plataforma de hospedagem (Netlify/Vercel), adicione o domínio personalizado

## 📁 Estrutura do Projeto

```
meusite/
├── index.html          # Página HTML principal com comentários
├── style.css           # Folha de estilos CSS
├── README.md           # Documentação (este arquivo)
├── .gitignore          # Arquivos ignorados pelo Git
└── assets/             # Pasta de assets (imagens, vídeos)
    ├── bg.mp4          # Vídeo de fundo
    └── bg-poster.jpg   # Imagem de poster
```

## 🎨 Personalizações Recomendadas

### Cores
No `style.css`, localize as variáveis CSS:
```css
:root {
  --primary: #4f46e5;     /* Cor principal */
  --accent: #ec4899;      /* Cor de destaque */
  --background: #0f172a;  /* Fundo */
  --muted: #94a3b8;       /* Texto mutado */
}
```

### Tipografia
Fonts usadas:
- **Principal**: Inter (do Google Fonts)
- Personalize em `style.css` ou `index.html`

### Responsividade
O design é mobile-first e se adapta para:
- 📱 Mobile (320px+)
- 📱 Tablet (768px+)
- 🖥️ Desktop (1024px+)

## 🚀 Deploy

### Checklist pré-deploy:
- ✅ Conteúdo personalizado
- ✅ Vídeo de fundo otimizado
- ✅ Links de navegação funcionam
- ✅ Formulários integrados (opcional)
- ✅ Testado em mobile
- ✅ SEO básico preenchido (title, description, keywords)

### Após deploy:
- Teste em diferentes navegadores
- Verifique performance em mobile
- Valide HTML/CSS com W3C Validator
- Teste velocidade no PageSpeed Insights


