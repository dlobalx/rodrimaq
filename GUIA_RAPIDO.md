# 🚀 Guia Rápido - TransMaq Website

## ⚡ Começar Agora (3 passos)

### 1️⃣ Abrir o Site
Clique duas vezes no arquivo `index.html` - pronto! O site abrirá no seu navegador.

### 2️⃣ Personalizar
Edite o arquivo `index.html` e altere:
- Nome da empresa (linha 17 e 45)
- Telefones (linhas 265-290)
- Email (linhas 265-290)
- Endereço (linhas 265-290)
- Número do WhatsApp (linha 377)

### 3️⃣ Adicionar Suas Imagens
Coloque suas fotos na pasta `images/` e substitua os placeholders no HTML.

---

## 📝 Personalizações Essenciais

### Mudar as Cores
Abra `css/style.css` e edite as linhas 10-18:

```css
--primary-color: #ff6b00;      /* Sua cor principal */
--secondary-color: #1a1a1a;    /* Sua cor secundária */
```

### Configurar WhatsApp
No arquivo `index.html`, linha 377:
```html
<a href="https://wa.me/5511987654321"
```
Troque `5511987654321` por: **55** + **DDD** + **seu número**

Exemplo: 55 11 98765-4321 = 5511987654321

### Configurar Formulário de Contato

**Opção Fácil - Formspree (Gratuito):**

1. Acesse: https://formspree.io/
2. Crie uma conta grátis
3. Crie um novo formulário
4. Copie o código que eles fornecem
5. No `index.html`, linha 292, substitua:

```html
<!-- De: -->
<form class="contact-form" id="contactForm">

<!-- Para: -->
<form action="https://formspree.io/f/SEU_ID_AQUI" method="POST" class="contact-form">
```

Pronto! Os emails chegarão na sua caixa de entrada.

---

## 🎨 Adicionar Suas Imagens

### Passo 1: Prepare as Imagens
- Formato: JPG ou PNG
- Tamanho recomendado: 
  - Projetos: 800x600px
  - Sobre: 600x400px
- Otimize em: https://tinypng.com/

### Passo 2: Coloque na Pasta
Copie suas imagens para a pasta `images/`

### Passo 3: Substitua no HTML
Procure por `<div class="image-placeholder">` e substitua por:

```html
<img src="images/sua-foto.jpg" alt="Descrição da imagem">
```

**Exemplo - Seção Sobre (linha 220):**
```html
<!-- Antes: -->
<div class="image-placeholder">
    <i class="fas fa-truck-loading"></i>
</div>

<!-- Depois: -->
<img src="images/empresa.jpg" alt="TransMaq Transportes">
```

---

## 🌐 Publicar na Internet

### Opção 1: GitHub Pages (Gratuito e Fácil)

1. Crie conta em: https://github.com/
2. Clique em "New repository"
3. Nome: `transmaq-website`
4. Marque "Public"
5. Clique em "Create repository"
6. Faça upload de todos os arquivos
7. Vá em: Settings > Pages
8. Em "Source", selecione "main"
9. Clique em "Save"
10. Seu site estará em: `https://seu-usuario.github.io/transmaq-website`

### Opção 2: Netlify (Mais Fácil Ainda)

1. Acesse: https://www.netlify.com/
2. Crie uma conta grátis
3. Arraste a pasta `transporte-maquinas` para o site
4. Pronto! Seu site está no ar em segundos

### Opção 3: Hospedagem Tradicional

Se você já tem uma hospedagem:
1. Acesse via FTP (FileZilla, por exemplo)
2. Faça upload de todos os arquivos
3. Acesse seu domínio

---

## 📱 Testar no Celular

### Método 1: Servidor Local
1. Abra o terminal na pasta do projeto
2. Execute: `python -m http.server 8000`
3. No celular, acesse: `http://SEU-IP:8000`
   - Para descobrir seu IP: 
     - Windows: `ipconfig`
     - Mac/Linux: `ifconfig`

### Método 2: Publicar Online
Publique no GitHub Pages ou Netlify e acesse pelo celular.

---

## ✅ Checklist de Personalização

- [ ] Alterar nome da empresa
- [ ] Atualizar telefones
- [ ] Atualizar emails
- [ ] Atualizar endereço
- [ ] Configurar WhatsApp
- [ ] Adicionar logo (se tiver)
- [ ] Adicionar fotos reais
- [ ] Configurar formulário de contato
- [ ] Testar em diferentes navegadores
- [ ] Testar no celular
- [ ] Publicar online

---

## 🆘 Problemas Comuns

### O site não abre
- Certifique-se de abrir o arquivo `index.html`
- Tente outro navegador (Chrome, Firefox)

### As cores não mudaram
- Salve o arquivo CSS após editar
- Limpe o cache do navegador (Ctrl+F5)

### O formulário não envia
- Configure o Formspree conforme instruções acima
- Ou use outro serviço de formulário

### O site não fica bonito no celular
- O site já é responsivo! Teste em um celular real
- Limpe o cache do navegador mobile

---

## 💡 Dicas Profissionais

1. **Use imagens de qualidade** - Fotos profissionais fazem diferença
2. **Otimize as imagens** - Use TinyPNG antes de adicionar
3. **Teste em vários dispositivos** - Celular, tablet, desktop
4. **Mantenha atualizado** - Atualize projetos e informações regularmente
5. **Adicione Google Analytics** - Para ver quantas visitas você tem

---

## 📞 Precisa de Ajuda?

- Revise o arquivo `README.md` para mais detalhes
- Consulte os comentários no código
- Teste as funcionalidades no navegador

---

**Boa sorte com seu website! 🚀**

Se tiver dúvidas, revise os arquivos ou teste as funcionalidades passo a passo.