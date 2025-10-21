# 🪒 Barbershop Management System - Apresentação

Site de apresentação profissional do projeto Sistema de Gestão de Barbearia.

## 🚀 Sobre o Projeto

Este é um site de portfólio/apresentação que mostra em detalhes o sistema completo de gestão de barbearia, incluindo:

- **Frontend Cliente** (Angular 18)
- **Backoffice Administrativo** (Angular 20)
- **API REST** (Spring Boot 3)

## 🛠️ Tecnologias

- **Angular 20** - Framework frontend
- **TypeScript 5** - Linguagem de programação
- **CSS3** - Estilização moderna com design tokens
- **Vercel** - Deploy e hosting

## 💻 Como Executar Localmente

```bash
# Navegar para a pasta do projeto
cd presentation

# Instalar dependências
npm install

# Executar em modo desenvolvimento
npm start

# Build para produção
npm run build
```

A aplicação estará disponível em: http://localhost:4200

## 🌐 Deploy no Vercel

### Opção 1: Deploy via CLI

```bash
# Instalar Vercel CLI
npm i -g vercel

# Fazer deploy
vercel
```

### Opção 2: Deploy via GitHub

1. Faça push do código para o GitHub
2. Conecte o repositório no [Vercel Dashboard](https://vercel.com)
3. Configure o projeto:
   - **Framework Preset**: Angular
   - **Build Command**: `npm run build:vercel`
   - **Output Directory**: `dist/presentation/browser`
4. Deploy!

## 📁 Estrutura do Projeto

```
presentation/
├── src/
│   ├── app/
│   │   ├── app.ts          # Componente principal
│   │   ├── app.html        # Template HTML
│   │   └── app.css         # Estilos do componente
│   ├── styles/
│   │   └── design-tokens.css  # Design system
│   ├── styles.css          # Estilos globais
│   └── index.html          # HTML principal
├── vercel.json             # Configuração Vercel
└── package.json            # Dependências
```

## 🎨 Features

- ✅ Design moderno e profissional
- ✅ Tema dark com acentos neon
- ✅ Animações CSS suaves
- ✅ 100% responsivo
- ✅ Performance otimizada
- ✅ SEO friendly

## 📝 Conteúdo

O site apresenta:

1. **Hero Section** - Título impactante com estatísticas
2. **Visão Geral** - Descrição das 3 aplicações
3. **Funcionalidades** - Features principais
4. **Stack Tecnológica** - Tecnologias detalhadas
5. **Conceitos** - Padrões e arquitetura aplicados
6. **Links** - Repositórios e demos

## 🔗 Links Úteis

- [Vercel Documentation](https://vercel.com/docs)
- [Angular Documentation](https://angular.dev)

---

**Desenvolvido com ❤️ para apresentar o projeto de forma profissional**
