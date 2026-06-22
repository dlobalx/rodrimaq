# 🚚 TransMaq - Website de Transporte de Máquinas

Website profissional desenvolvido do zero (sem WordPress ou frameworks) para empresa de transporte de máquinas e equipamentos pesados.

## 📋 Características

- ✅ Design moderno e profissional
- ✅ 100% responsivo (mobile, tablet, desktop)
- ✅ Desenvolvido com HTML5, CSS3 e JavaScript puro
- ✅ Animações suaves e interativas
- ✅ Formulário de contato funcional
- ✅ Menu mobile hamburger
- ✅ Botão WhatsApp flutuante
- ✅ Seções: Home, Serviços, Sobre, Projetos, Contato
- ✅ SEO otimizado
- ✅ Performance otimizada

## 📁 Estrutura do Projeto

```
transporte-maquinas/
│
├── index.html          # Página principal
├── css/
│   └── style.css      # Estilos do site
├── js/
│   └── script.js      # JavaScript e interatividade
├── images/            # Pasta para suas imagens
└── pages/             # Pasta para páginas adicionais (futuro)
```

## 🚀 Como Usar

### 1. Abrir o Site

Simplesmente abra o arquivo `index.html` em qualquer navegador moderno:
- Chrome
- Firefox
- Safari
- Edge

Ou clique duas vezes no arquivo `index.html`.

### 2. Testar Localmente

Para melhor experiência de desenvolvimento, use um servidor local:

**Opção 1 - Python:**
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

**Opção 2 - Node.js (http-server):**
```bash
npx http-server -p 8000
```

**Opção 3 - VS Code:**
Instale a extensão "Live Server" e clique com botão direito em `index.html` > "Open with Live Server"

Depois acesse: `http://localhost:8000`

## 🎨 Personalização

### Alterar Cores

Edite as variáveis CSS no arquivo `css/style.css` (linhas 10-18):

```css
:root {
    --primary-color: #ff6b00;      /* Cor principal (laranja) */
    --secondary-color: #1a1a1a;    /* Cor secundária (preto) */
    --accent-color: #ffa500;       /* Cor de destaque */
    --text-color: #333;            /* Cor do texto */
    --light-bg: #f8f9fa;           /* Fundo claro */
    /* ... */
}
```

### Alterar Textos

Edite o arquivo `index.html` e modifique:
- Nome da empresa (linha 17 e 45)
- Títulos e descrições
- Informações de contato (linhas 265-290)
- Serviços oferecidos
- Estatísticas da empresa

### Adicionar Imagens

1. Coloque suas imagens na pasta `images/`
2. Substitua os placeholders no HTML:

```html
<!-- De: -->
<div class="image-placeholder">
    <i class="fas fa-truck-loading"></i>
</div>

<!-- Para: -->
<img src="images/sua-imagem.jpg" alt="Descrição">
```

### Configurar WhatsApp

Edite a linha 377 do `index.html`:

```html
<a href="https://wa.me/5511987654321" class="whatsapp-float" target="_blank">
```

Substitua `5511987654321` pelo seu número (código do país + DDD + número).

### Configurar Email

Para o formulário de contato funcionar com envio real de emails, você precisa:

**Opção 1 - Serviço de Email (Recomendado):**
Use serviços como:
- [Formspree](https://formspree.io/) - Gratuito até 50 envios/mês
- [EmailJS](https://www.emailjs.com/) - Gratuito até 200 envios/mês
- [Web3Forms](https://web3forms.com/) - Gratuito ilimitado

**Opção 2 - Backend Próprio:**
Descomente e configure o código no arquivo `js/script.js` (linhas 127-149).

**Opção 3 - Formspree (Exemplo):**

1. Crie conta em https://formspree.io/
2. Crie um novo formulário
3. Copie o endpoint
4. Modifique o formulário no HTML:

```html
<form action="https://formspree.io/f/SEU_ID" method="POST" class="contact-form">
```

## 📱 Responsividade

O site é totalmente responsivo e se adapta a:
- 📱 Smartphones (320px+)
- 📱 Tablets (768px+)
- 💻 Desktops (1024px+)
- 🖥️ Telas grandes (1920px+)

## 🌐 Publicação Online

### Opção 1 - GitHub Pages (Gratuito)

1. Crie uma conta no GitHub
2. Crie um novo repositório
3. Faça upload dos arquivos
4. Vá em Settings > Pages
5. Selecione a branch main
6. Seu site estará em: `https://seu-usuario.github.io/nome-repositorio`

### Opção 2 - Netlify (Gratuito)

1. Crie conta em https://netlify.com
2. Arraste a pasta do projeto
3. Pronto! Site publicado

### Opção 3 - Vercel (Gratuito)

1. Crie conta em https://vercel.com
2. Importe o projeto
3. Deploy automático

### Opção 4 - Hospedagem Tradicional

Faça upload via FTP para qualquer hospedagem que suporte HTML/CSS/JS.

## 🔧 Funcionalidades JavaScript

- ✅ Menu mobile responsivo
- ✅ Scroll suave entre seções
- ✅ Destaque automático do menu ativo
- ✅ Animações ao scroll
- ✅ Validação de formulário
- ✅ Máscara de telefone
- ✅ Sistema de notificações
- ✅ Contador animado de estatísticas
- ✅ Lazy loading de imagens

## 📊 SEO e Performance

O site já está otimizado com:
- Meta tags apropriadas
- Descrições semânticas
- HTML5 semântico
- CSS otimizado
- JavaScript eficiente
- Imagens otimizadas (quando adicionar)

### Melhorias Adicionais de SEO:

1. **Adicione um sitemap.xml:**
```xml
<?xml version="1.0" encoding="UTF-8"?>
<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
  <url>
    <loc>https://seusite.com/</loc>
    <lastmod>2026-06-22</lastmod>
    <priority>1.0</priority>
  </url>
</urlset>
```

2. **Adicione robots.txt:**
```
User-agent: *
Allow: /
Sitemap: https://seusite.com/sitemap.xml
```

3. **Google Analytics:**
Adicione antes do `</head>`:
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

## 🎯 Próximos Passos

1. ✅ Adicione suas próprias imagens na pasta `images/`
2. ✅ Personalize textos e informações
3. ✅ Configure o número do WhatsApp
4. ✅ Configure o formulário de contato
5. ✅ Adicione seu logo
6. ✅ Teste em diferentes dispositivos
7. ✅ Publique online

## 📞 Suporte

Para dúvidas ou sugestões sobre o código:
- Revise os comentários no código
- Consulte a documentação do HTML/CSS/JS
- Teste as funcionalidades no navegador

## 📝 Licença

Este projeto é de código aberto. Sinta-se livre para usar e modificar conforme necessário.

## 🎨 Créditos

- Ícones: Font Awesome 6.4.0
- Fontes: Segoe UI (sistema)
- Design: Desenvolvido do zero

---

**Desenvolvido com ❤️ para TransMaq**

Boa sorte com seu website! 🚀