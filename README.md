# 🌈 CenaSquare

Rede Social LGBTQIAPN+ · Brasília

## 🚀 Publicar no GitHub Pages

### 1. Criar repositório

```bash
# No GitHub: New repository → cenasquare → Public → Create
```

### 2. Subir os arquivos

```bash
git init
git add index.html manifest.json README.md
git commit -m "CenaSquare v1 — deploy inicial"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/cenasquare.git
git push -u origin main
```

### 3. Ativar GitHub Pages

```
Repositório → Settings → Pages
Source: Deploy from a branch
Branch: main  /  (root)
→ Save
```

Em ~2 minutos o app estará em:
**<https://SEU_USUARIO.github.io/cenasquare>**

-----

## 📱 Instalar como app no celular (PWA)

**iPhone (Safari):**
Abrir o link → Compartilhar → Adicionar à Tela de Início

**Android (Chrome):**
Abrir o link → Menu ⋮ → Adicionar à tela inicial

-----

## 🔐 Contas de teste

|Usuário    |Senha     |Papel        |
|-----------|----------|-------------|
|`user`     |`123`     |Membro       |
|`lucas_bsb`|`123`     |Membro       |
|`admin`    |`admin123`|Administrador|

-----

## 🛠️ Próximo passo — Backend real (Supabase)

Para salvar imagens e dados de verdade:

1. Criar conta em [supabase.com](https://supabase.com)
1. Substituir as constantes em `API` no início do `index.html`:

```js
const API = {
  SUPABASE_URL: "https://SEU_PROJETO.supabase.co",
  SUPABASE_KEY: "SUA_ANON_KEY",
  ...
};
```

1. Criar buckets: `avatars`, `posts`, `stories`
1. Substituir `URL.createObjectURL()` pelo upload ao Supabase Storage

-----

## 📋 Funcionalidades

- ✅ Feed com filtro de seguidos
- ✅ Pull-to-refresh
- ✅ Carrossel de fotos nos posts
- ✅ Stories com link e legenda
- ✅ Modo LUST / Anjo
- ✅ Flerte com GPS real (haversine)
- ✅ Chat DM com foto de visualização única (20s)
- ✅ Ingressos e pagamento (PIX / Cartão / Boleto)
- ✅ Perfis, seguir, busca de usuários
- ✅ Editar/deletar posts e comentários
- ✅ Termos LGPD completos + verificação de idade
- ✅ Manter logado (localStorage)
- ✅ PWA — instala no celular como app nativo

-----

*Desenvolvido com React · Brasília · 2026*