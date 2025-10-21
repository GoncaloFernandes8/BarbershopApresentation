# 🚀 Guia de Deploy no Vercel

## Passo a Passo para Deploy

### 1. Preparar o Repositório

```bash
# Navegar para a pasta do projeto
cd /home/gon-alo/Documents/Projetos/BarbershopApresentation

# Inicializar Git (se ainda não foi feito)
git init

# Adicionar todos os arquivos
git add .

# Fazer o primeiro commit
git commit -m "Initial commit: Barbershop presentation site"

# Criar repositório no GitHub e adicionar remote
git remote add origin https://github.com/SEU-USUARIO/barbershop-presentation.git

# Push para GitHub
git push -u origin main
```

### 2. Deploy no Vercel via Dashboard

1. **Acesse** [vercel.com](https://vercel.com) e faça login
2. **Clique** em "Add New Project"
3. **Importe** seu repositório do GitHub
4. **Configure** o projeto:
   ```
   Framework Preset: Angular
   Root Directory: presentation
   Build Command: npm run build
   Output Directory: dist/presentation/browser
   Install Command: npm install
   ```
5. **Deploy!** 🎉

### 3. Deploy via Vercel CLI (Alternativa)

```bash
# Instalar Vercel CLI globalmente
npm install -g vercel

# Navegar para a pasta do projeto
cd presentation

# Login no Vercel
vercel login

# Deploy
vercel

# Para produção
vercel --prod
```

### 4. Variáveis de Ambiente (se necessário)

No Vercel Dashboard:
1. Settings → Environment Variables
2. Adicionar variáveis necessárias

### 5. Domínio Customizado (Opcional)

1. Settings → Domains
2. Adicionar seu domínio custom
3. Configurar DNS conforme instruções

## 📝 Checklist Pré-Deploy

- [ ] Código committed no Git
- [ ] Build local funciona (`npm run build`)
- [ ] Todos os links externos atualizados
- [ ] URLs do GitHub atualizadas no HTML
- [ ] Teste de responsividade feito
- [ ] Performance otimizada

## 🔗 Links Importantes

- **Vercel Dashboard**: https://vercel.com/dashboard
- **Documentação Angular + Vercel**: https://vercel.com/guides/deploying-angular-with-vercel
- **Suporte Vercel**: https://vercel.com/support

## 🎯 Após o Deploy

1. **Teste o site** em produção
2. **Compartilhe o link** no seu CV
3. **Atualize** LinkedIn com o link do projeto
4. **Adicione** o link no README do GitHub

## 🐛 Troubleshooting

### Erro de Build

```bash
# Limpar cache e rebuild
rm -rf node_modules package-lock.json
npm install
npm run build
```

### Erro 404 em Rotas

- Verificar se `vercel.json` tem as rewrites corretas
- Confirmar que `outputDirectory` está correto

### Página em Branco

- Verificar console do navegador
- Confirmar que assets estão sendo carregados
- Testar build local primeiro

---

**Boa sorte com o deploy! 🚀**

