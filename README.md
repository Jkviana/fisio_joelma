# Fisioterapia Integrativa - Landing Page

Landing page profissional para fisioterapeutas e terapeutas integrativas, desenvolvida com React, Tailwind CSS e design Organic Modernism.

## 📁 Estrutura de Arquivos

```
├── index.html              # Arquivo HTML principal
├── assets/
│   ├── index-DYfRqMfI.js  # JavaScript compilado (React + dependências)
│   └── index-D_Jz3oJT.css # CSS compilado (Tailwind + estilos customizados)
└── README.md              # Este arquivo
```

## 🚀 Como Usar

### Opção 1: Servidor Local (Recomendado)

1. **Python 3:**
```bash
cd /caminho/para/pasta
python3 -m http.server 8000
```
Acesse: `http://localhost:8000`

2. **Node.js (http-server):**
```bash
npm install -g http-server
http-server .
```

3. **PHP:**
```bash
cd /caminho/para/pasta
php -S localhost:8000
```

### Opção 2: Upload para Servidor Web

1. Faça upload de todos os arquivos para seu servidor web
2. Configure o servidor para servir `index.html` como página padrão
3. Acesse via seu domínio

### Opção 3: Hospedagem Gratuita

- **Netlify**: Arraste a pasta para [netlify.com](https://netlify.com)
- **Vercel**: Faça upload para [vercel.com](https://vercel.com)
- **GitHub Pages**: Faça push para GitHub e ative Pages

## 🔧 Configuração do Formulário

O formulário está preparado para integração com Google Sheets. Para ativar:

1. Crie um Google Form em [forms.google.com](https://forms.google.com)
2. Adicione os campos: Nome, Email, Telefone, Mensagem
3. Obtenha os IDs dos campos (veja instruções no arquivo GOOGLE_SHEETS_SETUP.md)
4. Edite o arquivo `index.html` e procure por:
   ```javascript
   const formUrl = "https://docs.google.com/forms/d/e/1FAIpQLSf_EXAMPLE/formResponse";
   ```
5. Substitua pelos dados reais do seu formulário

## 📱 Responsividade

A landing page é totalmente responsiva e funciona em:
- ✅ Desktop (1920px+)
- ✅ Tablet (768px - 1024px)
- ✅ Mobile (320px - 767px)

## 🎨 Personalização

### Mudar Cores
Edite o arquivo `index.html` e procure pela seção de CSS. As cores principais estão definidas como:
- Verde-sálvia: `oklch(0.65 0.08 145)`
- Terracota: `oklch(0.72 0.12 35)`
- Areia: `oklch(0.95 0.01 85)`

### Mudar Textos
Edite diretamente no `index.html` os textos que deseja alterar.

### Mudar Imagens
Substitua a URL da imagem hero no `index.html`:
```html
<img src="sua-imagem-aqui.jpg" alt="Descrição">
```

## 📞 Informações de Contato

Atualize as informações de contato no `index.html`:
- Telefone
- Email
- Instagram
- Endereço

## ⚙️ Requisitos

- Navegador web moderno (Chrome, Firefox, Safari, Edge)
- Conexão com internet (para carregar fontes do Google)
- Servidor web (para servir os arquivos)

## 🔐 Segurança

- Todos os arquivos são estáticos (sem backend)
- Não há armazenamento de dados localmente
- Use HTTPS em produção
- Valide dados do formulário no backend antes de processar

## 📊 Analytics

Para adicionar rastreamento:

1. **Google Analytics:**
```html
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_ID');
</script>
```

2. **Facebook Pixel:**
```html
<script>
  !function(f,b,e,v,n,t,s)
  {if(f.fbq)return;n=f.fbq=function(){n.callMethod?
  n.callMethod.apply(n,arguments):n.queue.push(arguments)};
  // ... código do pixel
</script>
```

## 🐛 Troubleshooting

**Problema**: Imagens não carregam
- **Solução**: Verifique as URLs das imagens e certifique-se de que estão acessíveis

**Problema**: Estilos não aplicam
- **Solução**: Limpe o cache do navegador (Ctrl+Shift+Delete)

**Problema**: Formulário não funciona
- **Solução**: Verifique se o Google Form está configurado corretamente

## 📝 Licença

Este projeto é fornecido como está. Sinta-se livre para personalizar e usar em seu negócio.

## 🤝 Suporte

Para dúvidas sobre implementação ou personalização, consulte a documentação incluída ou entre em contato com o desenvolvedor.

---

**Desenvolvido com ❤️ usando React, Tailwind CSS e Design Organic Modernism**
