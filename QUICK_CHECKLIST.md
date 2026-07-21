# ✅ QUICK CHECKLIST - DEPLOY VERCEL

**Copy and paste para acompanhar o deploy em tempo real**

---

## 🎯 PRÉ-DEPLOYMENT (30 minutos)

- [ ] `git init`
- [ ] `git add .`
- [ ] `git commit -m "feat: Initial commit - Iron Wood Decor landing v01"`
- [ ] Criar repo no GitHub
- [ ] `git remote add origin https://github.com/seu-usuario/iron-wood-decor.git`
- [ ] `git push -u origin main`
- [ ] Acessar https://vercel.com
- [ ] Login com GitHub
- [ ] "New Project"
- [ ] Selecionar repositório
- [ ] Settings → Project Name: `iron-wood-decor`
- [ ] Deploy! 🚀

---

## 🌐 PÓS-DEPLOYMENT AUTOMÁTICO (15 minutos)

- [ ] Copiar URL de preview (ex: iron-wood-decor.vercel.app)
- [ ] Testar em desktop
- [ ] Testar em mobile (Chrome DevTools)
- [ ] Testar navbar responsiva
- [ ] Testar form submission (WhatsApp)
- [ ] Verificar console (sem erros)
- [ ] Verificar Network tab (imagens carregam)

---

## 🔗 CONFIGURAÇÃO DE DOMÍNIO (10 minutos)

Se já tem domínio:

- [ ] Vercel Settings → Domains
- [ ] "Add" → `ironwooddecor.com`
- [ ] Vai gerar registros DNS (anotar)
- [ ] Ir para seu provedor de domínio (Namecheap/Google Domains)
- [ ] Coloca registros DNS fornecidos pela Vercel
- [ ] Aguarda 24-48h de propagação
- [ ] Testar https://ironwooddecor.com

Se não tem domínio ainda:

- [ ] Comprar em https://domains.google.com ou Namecheap
- [ ] Seguir passos acima depois

---

## 📊 VERIFICAÇÃO DE PERFORMANCE (5 minutos)

- [ ] Abrir https://pagespeed.web.dev
- [ ] Colar URL: iron-wood-decor.vercel.app
- [ ] Executar análise
- [ ] Performance score (alvo: 85+)
- [ ] Anotar recomendações
- [ ] Anotar próximas otimizações

---

## 🔐 CONFIGURAÇÃO DE SEGURANÇA (5 minutos)

- [ ] Vercel Settings → Security
- [ ] Ativar "Automatic HTTPS" ✅
- [ ] Revisar vercel.json headers ✅
- [ ] CORS configurado ✅

---

## 📈 ANALYTICS & SEO (15 minutos)

### Google Analytics
- [ ] Ir para https://analytics.google.com
- [ ] Create new property
- [ ] Copiar ID (ex: G-XXXXX)
- [ ] Adicionar ao `<head>` do HTML
- [ ] Aguardar 24h para dados aparecerem

### Google Search Console
- [ ] Ir para https://search.google.com/search-console
- [ ] Add property: ironwooddecor.com
- [ ] Verify ownership (DNS TXT record)
- [ ] Submit sitemap.xml
- [ ] Solicitar indexação

### Bing Webmaster
- [ ] Ir para https://www.bing.com/webmaster
- [ ] Add site
- [ ] Verify
- [ ] Submit sitemap.xml

---

## 📱 TESTES FINAIS (10 minutos)

### Desktop
- [ ] Chrome
- [ ] Firefox
- [ ] Safari

### Mobile
- [ ] iPhone (SE, 11, 13, 15)
- [ ] Android (Samsung, Pixel)
- [ ] Tablet

### Conexões
- [ ] 4G
- [ ] WiFi
- [ ] 3G slow (DevTools throttling)

### Funcionalidades
- [ ] Menu mobile abre/fecha
- [ ] Links internos funcionam
- [ ] Form envia corretamente
- [ ] WhatsApp link funciona
- [ ] Instagram link funciona
- [ ] Animations suaves

---

## 📝 TESTE DO FORM

1. Abrir página
2. Ir para seção "Contato"
3. Preencher:
   - Nome: Test User
   - WhatsApp: +5592981065678
   - Tipo: Mesa em madeira maciça
   - Cidade: Manaus
   - Mensagem: Teste de envio
4. Clicar "Enviar minha ideia pelo WhatsApp"
5. Verificar se abre WhatsApp

---

## 🎉 SUCESSO?

Se todos os checks passaram:

```
✅ Parabéns! Seu site está LIVE!
✅ URL: https://ironwooddecor.com
✅ HTTPS: Ativo
✅ Performance: Otimizada
✅ SEO: Indexado
✅ Analytics: Rastreando
```

---

## ⏰ TIMELINE ESTIMADO

| Tarefa | Tempo | Quando |
|--------|-------|--------|
| Setup Git | 5 min | Agora |
| Deploy Vercel | 10 min | Agora |
| Testes | 10 min | Agora |
| Domínio | 10 min | Agora |
| Analytics | 10 min | Hoje |
| Propagação DNS | 24-48h | Amanhã |
| **TOTAL** | **1h** | **Hoje** |

---

## 🆘 PROBLEMAS COMUNS

**"Erro 404 ao acessar"**
- Verificar se o push ao GitHub foi bem-sucedido
- Conferir branch é `main`

**"DNS não resolve"**
- Registros DNS levam até 48h
- Usar https://dnschecker.org para verificar

**"Form não envia"**
- Testar em preview URL primeiro
- Verificar console para erros

**"Imagens não carregam"**
- Verificar caminho relativo das imagens
- Usar `/public/` antes do caminho

---

## 📞 SUPORTE

- Vercel Docs: https://vercel.com/docs
- Status Page: https://vercel-status.com/
- Help: https://vercel.com/support

---

**Gerado:** 20/07/2026  
**Status:** Ready to Deploy ✅  
**Boa sorte! 🚀**
