# 🚀 GUIA DE DEPLOY - VERCEL

**Projeto:** Iron Wood Decor Landing Page  
**Versão:** 01  
**Data:** 20/07/2026  
**Status:** 🟢 Pronto para deploy

---

## 📋 CHECKLIST PRÉ-DEPLOYMENT

### ✅ Validação de Código

- [ ] HTML validado (sem erros)
- [ ] CSS sem conflitos ou especificidades excessivas
- [ ] JavaScript sem console errors
- [ ] Imagens otimizadas e acessíveis
- [ ] Links internos testados
- [ ] Form testado em desktop e mobile

### ✅ Performance

- [ ] Lighthouse Score ≥ 85
- [ ] Tempo de carregamento < 2s (3G lento)
- [ ] FCP (First Contentful Paint) < 1.8s
- [ ] LCP (Largest Contentful Paint) < 2.5s
- [ ] CLS (Cumulative Layout Shift) < 0.1

### ✅ Segurança

- [ ] Headers de segurança configurados (vercel.json)
- [ ] HTTPS ativado
- [ ] CSP (Content Security Policy) testada
- [ ] Sem dados sensíveis no código
- [ ] Validação de form no cliente

### ✅ SEO

- [ ] Meta tags presentes e corretas
- [ ] Favicon configurado
- [ ] Open Graph tags funcionando
- [ ] Schema.org structured data válido
- [ ] Robots.txt criado
- [ ] Sitemap.xml criado
- [ ] Canonical URL correto

### ✅ Acessibilidade

- [ ] WCAG 2.1 AA compliant
- [ ] Cores com contraste adequado
- [ ] Navegação por teclado funciona
- [ ] Screen readers testados
- [ ] Prefers-reduced-motion respeitado

### ✅ Configuração Vercel

- [ ] vercel.json criado
- [ ] Ambiente configurado
- [ ] Headers de cache corretos
- [ ] Rewrites funcionando
- [ ] Deploy preview testado

---

## 🔄 PROCESSO DE DEPLOY

### Passo 1: Preparar Repositório Git

```bash
# Dentro do diretório do projeto
git init
git add .
git commit -m "Initial commit: Iron Wood Decor landing page v01"
git branch -M main
```

### Passo 2: Conectar com Vercel

**Opção A: Via GitHub**
1. Push para GitHub: `git push -u origin main`
2. Ir para [vercel.com](https://vercel.com)
3. Clicar em "New Project"
4. Selecionar repositório
5. Clicar "Deploy"

**Opção B: Via CLI**
```bash
# Instalar Vercel CLI
npm i -g vercel

# Deploy
vercel
```

### Passo 3: Configurar Domínio

1. No painel Vercel → Settings → Domains
2. Adicionar domínio: `ironwooddecor.com`
3. Configurar DNS:
   - A: 76.76.19.165
   - CNAME: cname.vercel-dns.com

### Passo 4: Testar Post-Deploy

- [ ] URL do site funciona
- [ ] HTTPS funciona
- [ ] Redirecionamento de WWW
- [ ] Mobile responsivo
- [ ] Form envia corretamente
- [ ] Analytics rastreando
- [ ] Cache funcionando

---

## 📊 ESTRUTURA FINAL DO PROJETO

```
iron-wood-decor/
│
├── 📄 index.html              # HTML principal
├── 📄 vercel.json             # Config Vercel
├── 📄 robots.txt              # SEO robots
├── 📄 sitemap.xml             # SEO sitemap
│
├── 📁 public/                 # Arquivos estáticos (cache 1 ano)
│   ├── 🖼️ images/
│   │   ├── hero-art-card.webp
│   │   ├── inspiration-1.webp
│   │   ├── inspiration-2.webp
│   │   ├── inspiration-3.webp
│   │   ├── inspiration-4.webp
│   │   └── inspiration-5.webp
│   ├── 🎨 logo.svg
│   └── 🔗 favicon.ico
│
├── 📁 css/
│   └── styles.css             # Estilos extraídos (cache 1 ano)
│
├── 📁 js/
│   └── script.js              # JavaScript extraído (cache 1 ano)
│
├── 📄 .gitignore
├── 📄 README.md
├── 📄 .env.example            # Template variáveis
└── 📄 package.json            # (Optional) Para build steps
```

---

## 🔐 VARIÁVEIS DE AMBIENTE

### .env.local (nunca commitar)
```
NEXT_PUBLIC_SITE_URL=https://ironwooddecor.com
NEXT_PUBLIC_GA_ID=G-XXXXXXXXXX
WHATSAPP_API_KEY=***
FORM_SUBMISSION_URL=https://api.example.com/leads
```

---

## 🎨 OTIMIZAÇÕES FUTURAS

### Fase 2: Melhorias Imediatas
- [ ] Extrair imagens base64 para arquivos WebP
- [ ] Minificar CSS/JavaScript
- [ ] Implementar lazy loading de imagens
- [ ] Adicionar service worker para PWA

### Fase 3: Backend (Opcional)
- [ ] API de formulário (serverless function)
- [ ] Database para leads
- [ ] Email automation
- [ ] CMS para conteúdo

### Fase 4: Avançado
- [ ] Upgrade para Next.js
- [ ] Dark mode
- [ ] Multi-idioma (PT/EN)
- [ ] Integração CRM

---

## 🆘 TROUBLESHOOTING

### Problema: CORS errors no form
**Solução:** Implementar serverless function Vercel como proxy

### Problema: Imagens demora para carregar
**Solução:** 
- Converter para WebP
- Usar Image Optimization do Vercel
- CDN para imagens estáticas

### Problema: Score Lighthouse baixo
**Solução:**
- Remover base64 inline
- Minificar assets
- Implementar preload/prefetch

### Problema: Cache não funciona
**Solução:** Verificar headers em vercel.json e versionar arquivos

---

## 📞 SUPORTE

### Documentação
- [Vercel Docs](https://vercel.com/docs)
- [Web Vitals](https://web.dev/vitals/)
- [SEO Checklist](https://web.dev/lighthouse-seo/)

### Ferramentas de Teste
- [PageSpeed Insights](https://pagespeed.web.dev/)
- [Lighthouse](https://developers.google.com/web/tools/lighthouse)
- [Web Accessibility Checker](https://wave.webaim.org/)
- [GTmetrix](https://gtmetrix.com/)

---

## ✨ RESUMO

| Aspecto | Status | Nota |
|--------|--------|------|
| Design | ✅ Excelente | Moderno e responsivo |
| Performance | 🟡 Bom | Otimizações necessárias |
| SEO | ✅ Bom | Meta tags presentes |
| Segurança | ✅ Bom | Headers configurados |
| Acessibilidade | ✅ Bom | WCAG compliant |
| **Pronto para Deploy** | **✅ SIM** | Começar hoje mesmo! |

---

**Próximo passo:** Faça commit e deploy! 🚀
