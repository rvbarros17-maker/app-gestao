# 🍧 Geladinhos Gourmet - Sistema de Gestão PWA

Sistema completo de gestão para negócio de geladinhos gourmet com funcionalidades de PWA (Progressive Web App).

## 📱 Funcionalidades

### ✅ Módulos Completos:
1. **👥 Clientes** - Cadastro, créditos, dívidas
2. **📦 Insumos** - Controle de estoque, entrada, estoque mínimo
3. **📋 Receitas** - Ingredientes fixos e por unidade
4. **🍧 Produtos** - Finais e intermediários
5. **🛒 Vendas** - Dinheiro, Pix, Fiado, uso de crédito
6. **💵 Fluxo de Caixa** - Abertura, fechamento, sangria, reforço
7. **💰 Financeiro** - A receber, recebido, créditos
8. **📊 Relatórios** - Produtos mais vendidos, melhores clientes, lucro
9. **📅 Despesas Recorrentes** - Mensais e parceladas
10. **🛒 Lista de Compras** - Automática baseada em estoque mínimo
11. **🔐 Autenticação** - Login com Firebase

### 🚀 PWA Features:
- ✅ Instalável na tela inicial
- ✅ Funciona offline (cache)
- ✅ Ícone personalizado
- ✅ Experiência de app nativo

## 📦 Arquivos do Projeto

```
geladinhos-pwa/
├── app-final-CORRETO.html    # Aplicação principal
├── manifest.json              # Configuração PWA
├── service-worker.js          # Cache offline
├── icon-192.png              # Ícone 192x192 (criar)
├── icon-512.png              # Ícone 512x512 (criar)
└── INSTRUÇÕES-ICONES.md      # Como criar os ícones
```

## 🚀 Como Usar

### 1. Criar os Ícones
Siga as instruções em `INSTRUÇÕES-ICONES.md` para criar:
- icon-192.png (192x192 pixels)
- icon-512.png (512x512 pixels)

### 2. Hospedar os Arquivos
O PWA precisa de HTTPS. Opções:

**OPÇÃO A - Firebase Hosting (Recomendado):**
```bash
# Instalar Firebase CLI
npm install -g firebase-tools

# Login
firebase login

# Inicializar projeto
firebase init hosting

# Deploy
firebase deploy
```

**OPÇÃO B - Netlify (Mais Fácil):**
1. Acesse netlify.com
2. Arraste a pasta com os arquivos
3. Pronto! URL automático com HTTPS

**OPÇÃO C - Vercel:**
```bash
npm install -g vercel
vercel
```

### 3. Instalar no Celular

1. Abra o site no **Chrome** (celular)
2. Menu (⋮) → **"Adicionar à tela inicial"**
3. Pronto! O app está instalado 🎉

## 🔐 Configuração Firebase

O app já vem configurado com Firebase. Se quiser usar seu próprio:

1. Crie projeto em console.firebase.google.com
2. Ative Authentication (Email/Password)
3. Ative Firestore Database
4. Copie as credenciais
5. Substitua no HTML (linha 16-23):

```javascript
const firebaseConfig = {
  apiKey: "SUA-API-KEY",
  authDomain: "SEU-PROJECT.firebaseapp.com",
  projectId: "SEU-PROJECT-ID",
  // ...
};
```

## 📱 Testado em:

- ✅ Chrome (Desktop e Mobile)
- ✅ Safari (iOS)
- ✅ Firefox
- ✅ Edge

## 🎨 Personalização

### Mudar Cores:
Edite no HTML e manifest.json:
- Cor tema: `#6366f1` (roxo/azul)
- Pode mudar para cores da sua marca

### Mudar Nome:
1. HTML: `<title>` (linha 6)
2. manifest.json: `name` e `short_name`

## 🐛 Troubleshooting

### PWA não aparece para instalar:
- ✅ Verifique se está em HTTPS
- ✅ Confirme que manifest.json está acessível
- ✅ Verifique que os ícones existem
- ✅ Limpe o cache do navegador

### Não funciona offline:
- ✅ Verifique se service-worker.js está registrado
- ✅ Abra DevTools → Application → Service Workers

### Firebase não conecta:
- ✅ Verifique credenciais
- ✅ Ative Authentication e Firestore no console

## 📞 Suporte

Sistema desenvolvido para gestão de negócios de geladinhos gourmet.

## 📄 Licença

Proprietário - Todos os direitos reservados.

---

**🎉 Desenvolvido com ❤️ para empreendedores de geladinhos gourmet!**
