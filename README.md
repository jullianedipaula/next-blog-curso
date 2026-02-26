# 📝 Site.Set - Blog & Landing Page

Um site moderno com blog construído com Next.js 15, TypeScript e Contentlayer, focado em vendas de produtos como afiliado.

## 🚀 Sobre o Projeto

Site.Set é uma plataforma completa que combina uma landing page atrativa com um sistema de blog gerenciado por arquivos Markdown. O projeto oferece uma experiência moderna e responsiva para promover e vender produtos digitais.

### ✨ Funcionalidades

- 🏠 **Landing Page**: Página inicial com seções para apresentação de produtos e serviços
- 📄 **Blog Dinâmico**: Sistema de blog com posts em Markdown
- 🎨 **Design Responsivo**: Interface adaptável para todos os dispositivos
- 🔍 **SEO Otimizado**: Meta tags e Open Graph configurados
- 📱 **Componentes Reutilizáveis**: Biblioteca de componentes modulares
- 🎯 **Sistema de Rotas**: App Router do Next.js para navegação otimizada
- 📝 **Markdown Suportado**: Posts com suporte a GitHub Flavored Markdown
- 🎭 **Componentes UI**: Elementos de interface com Radix UI e Tailwind CSS

## 🛠️ Tecnologias Utilizadas

- **[Next.js 15](https://nextjs.org/)** - Framework React com App Router
- **[React 19](https://react.dev/)** - Biblioteca JavaScript para interfaces
- **[TypeScript](https://www.typescriptlang.org/)** - Superset JavaScript com tipagem estática
- **[Contentlayer](https://contentlayer.dev/)** - Gerenciamento de conteúdo em Markdown
- **[Tailwind CSS](https://tailwindcss.com/)** - Framework CSS utility-first
- **[Biome](https://biomejs.dev/)** - Linter e formatter rápido
- **[React Markdown](https://remarkjs.github.io/react-markdown/)** - Renderização de Markdown
- **[Lucide React](https://lucide.dev/)** - Ícones modulares
- **[Radix UI](https://www.radix-ui.com/)** - Componentes acessíveis e não estilizados

## 📁 Estrutura do Projeto

```
site-blog/
├── posts/                    # Arquivos Markdown dos posts
│   ├── primeiro-post.md
│   └── segundo-post.md
├── public/                   # Arquivos estáticos
│   └── assets/              # Imagens e recursos
├── src/
│   ├── app/                 # App Router do Next.js
│   │   ├── blog/           # Páginas do blog
│   │   │   ├── [slug]/    # Posts dinâmicos
│   │   │   └── page.tsx
│   │   ├── layout.tsx
│   │   ├── page.tsx
│   │   └── ...
│   ├── components/          # Componentes reutilizáveis
│   │   ├── active-link/
│   │   ├── avatar/
│   │   ├── layout/
│   │   ├── logo/
│   │   ├── markdown/
│   │   ├── search/
│   │   └── ui/
│   ├── hooks/               # Custom hooks
│   │   ├── use-clipboard/
│   │   └── use-share/
│   ├── lib/                 # Utilitários
│   ├── templates/           # Templates de páginas
│   │   ├── blog/
│   │   └── landing-page/
│   └── styles/              # Estilos globais
├── contentlayer.config.ts   # Configuração do Contentlayer
├── tailwind.config.ts       # Configuração do Tailwind
├── biome.json              # Configuração do Biome
├── next.config.ts          # Configuração do Next.js
└── package.json
```

## 🚦 Começando

### Pré-requisitos

- Node.js 20+ instalado
- pnpm (recomendado) ou npm

### Instalação

1. Clone o repositório:
```bash
git clone <url-do-repositorio>
cd site-blog
```

2. Instale as dependências:
```bash
pnpm install
# ou
npm install
```

3. Execute o servidor de desenvolvimento:
```bash
pnpm dev
# ou
npm run dev
```

4. Abra [http://localhost:3000](http://localhost:3000) no navegador.

## 📜 Scripts Disponíveis

```bash
pnpm dev       # Inicia o servidor de desenvolvimento
pnpm build     # Cria build de produção
pnpm start     # Inicia o servidor de produção
pnpm lint      # Executa o linter do Next.js
pnpm format    # Formata o código com Biome
```

## ✍️ Como Criar um Novo Post

1. Crie um novo arquivo `.md` na pasta `posts/`
2. Adicione o frontmatter no topo do arquivo:

```markdown
---
title: Título do seu post
description: Breve descrição do post
date: 2026/02/26 10:00:00
image: /assets/imagem.png
author:
  name: Seu Nome
  avatar: /avatar.png
---

Seu conteúdo em Markdown aqui...
```

3. O post será automaticamente processado pelo Contentlayer e estará disponível no blog.

## 🎨 Personalização

### Cores e Tema

As cores e estilos podem ser personalizados no arquivo [tailwind.config.ts](tailwind.config.ts).

### Componentes

Os componentes estão organizados em pastas modulares dentro de [src/components/](src/components/). Cada componente possui seu próprio arquivo de índice para facilitar importações.

### Metadados SEO

Configure os metadados em cada página usando o objeto `metadata` do Next.js.

## 📦 Build para Produção

```bash
pnpm build
pnpm start
```

O build otimizado será criado na pasta `.next/`.
