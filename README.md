# Controle de Cheques · RM Estruturas

App PWA para controle de cheques, instalável pelo Chrome.

## 📁 Estrutura dos arquivos

```
├── index.html      ← App principal
├── manifest.json   ← Configuração do PWA
├── sw.js           ← Service Worker (funciona offline)
└── icons/
    ├── icon-192.png
    └── icon-512.png
```

---

## 🚀 Como publicar no GitHub Pages

### 1. Criar o repositório

1. Acesse [github.com](https://github.com) e faça login
2. Clique em **New repository**
3. Nome sugerido: `cheques-rm`
4. Marque **Public** (necessário para GitHub Pages grátis)
5. Clique em **Create repository**

### 2. Fazer upload dos arquivos

**Opção A — Pela interface web (mais fácil):**

1. No repositório criado, clique em **Add file → Upload files**
2. Arraste a pasta inteira ou selecione todos os arquivos:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - pasta `icons/` com os dois `.png`
3. Clique em **Commit changes**

**Opção B — Git no terminal:**
```bash
git init
git add .
git commit -m "Primeiro commit - PWA Controle de Cheques"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/cheques-rm.git
git push -u origin main
```

### 3. Ativar GitHub Pages

1. No repositório, vá em **Settings → Pages**
2. Em **Source**, selecione **Deploy from a branch**
3. Branch: **main** / pasta: **/ (root)**
4. Clique em **Save**
5. Aguarde ~1 minuto — o site ficará disponível em:
   ```
   https://SEU-USUARIO.github.io/cheques-rm/
   ```

---

## 📲 Instalar pelo Chrome (Android ou Desktop)

### No celular Android:
1. Abra o Chrome e acesse a URL do GitHub Pages
2. O Chrome mostrará automaticamente um banner **"Adicionar à tela inicial"**
3. Ou: toque no menu (⋮) → **Adicionar à tela inicial**
4. Confirme → o app aparece como ícone na tela inicial

### No computador (Chrome):
1. Acesse a URL no Chrome
2. Na barra de endereço, clique no ícone **⊕ Instalar** (canto direito)
3. Ou: menu (⋮) → **Salvar e compartilhar → Instalar página como app**
4. Clique em **Instalar**
5. O app abre em janela própria, sem barra do browser

---

## ✅ Funcionalidades PWA incluídas

- ✔ Instalável no celular e desktop
- ✔ Funciona offline (após primeira visita)
- ✔ Ícone na tela inicial
- ✔ Tela cheia sem barra do browser
- ✔ Dados salvos localmente no dispositivo (localStorage)
