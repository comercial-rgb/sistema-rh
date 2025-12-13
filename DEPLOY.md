# 🚀 Guia de Deploy no GitHub

Este guia mostra como publicar o Sistema de Gestão de Funcionários no GitHub.

## 📋 Pré-requisitos

- Conta no GitHub (gratuita)
- Git instalado em seu computador
- Arquivos do sistema baixados

---

## 🎯 Passo a Passo

### 1️⃣ Criar Repositório no GitHub

1. Acesse [GitHub.com](https://github.com) e faça login
2. Clique no botão **"New"** (ou ícone +) no canto superior direito
3. Selecione **"New repository"**
4. Preencha:
   - **Repository name:** `sistema-rh` (ou nome de sua preferência)
   - **Description:** "Sistema de Gestão de Funcionários CLT e Terceiros"
   - Marque **"Public"** (para usar GitHub Pages gratuitamente)
   - ✅ NÃO marque "Add a README file" (já temos um)
5. Clique em **"Create repository"**

### 2️⃣ Preparar Arquivos Localmente

Abra o terminal/prompt de comando na pasta do projeto e execute:

```bash
# Inicializar repositório Git
git init

# Adicionar todos os arquivos
git add .

# Fazer o primeiro commit
git commit -m "feat: Sistema de gestão de funcionários v1.0"

# Renomear branch para main (padrão do GitHub)
git branch -M main
```

### 3️⃣ Conectar ao GitHub

No GitHub, copie a URL do seu repositório. Ela será algo como:
```
https://github.com/SEU-USUARIO/sistema-rh.git
```

No terminal, execute:

```bash
# Adicionar remote (substitua SEU-USUARIO pelo seu usuário)
git remote add origin https://github.com/SEU-USUARIO/sistema-rh.git

# Enviar código para o GitHub
git push -u origin main
```

### 4️⃣ Ativar GitHub Pages

1. No repositório do GitHub, clique em **"Settings"** (Configurações)
2. No menu lateral, clique em **"Pages"**
3. Em **"Source"**, selecione:
   - Branch: `main`
   - Folder: `/ (root)`
4. Clique em **"Save"**
5. Aguarde 1-2 minutos

**🎉 Pronto!** Seu sistema estará disponível em:
```
https://SEU-USUARIO.github.io/sistema-rh
```

---

## 🔧 Comandos Úteis

### Fazer Alterações e Atualizar

```bash
# Ver status das alterações
git status

# Adicionar arquivos modificados
git add .

# Fazer commit
git commit -m "descrição das alterações"

# Enviar para o GitHub
git push
```

### Ver Histórico

```bash
# Ver commits anteriores
git log

# Ver diferenças
git diff
```

### Desfazer Alterações

```bash
# Descartar alterações em um arquivo
git checkout -- nome-do-arquivo

# Voltar ao último commit
git reset --hard HEAD
```

---

## 🌐 Opções de Deploy Alternativas

### Opção 1: Vercel (Recomendado)

1. Acesse [Vercel.com](https://vercel.com)
2. Faça login com GitHub
3. Clique em **"New Project"**
4. Selecione seu repositório
5. Clique em **"Deploy"**

✅ **Vantagens:** 
- Deploy automático a cada push
- HTTPS automático
- Mais rápido que GitHub Pages

### Opção 2: Netlify

1. Acesse [Netlify.com](https://netlify.com)
2. Faça login com GitHub
3. Clique em **"New site from Git"**
4. Selecione GitHub e seu repositório
5. Clique em **"Deploy site"**

✅ **Vantagens:**
- Interface simples
- Deploy automático
- Formulários e funções serverless

### Opção 3: Render

1. Acesse [Render.com](https://render.com)
2. Faça login com GitHub
3. Clique em **"New Static Site"**
4. Conecte seu repositório
5. Configure e deploy

---

## 📝 Mensagens de Commit Recomendadas

Siga o padrão de commits semânticos:

```bash
# Nova funcionalidade
git commit -m "feat: adiciona exportação de holerites"

# Correção de bug
git commit -m "fix: corrige validação de CPF"

# Documentação
git commit -m "docs: atualiza README com novas instruções"

# Refatoração
git commit -m "refactor: reorganiza estrutura de pastas"

# Estilo/formatação
git commit -m "style: ajusta espaçamento do header"

# Teste
git commit -m "test: adiciona testes para validação de CNPJ"
```

---

## 🔒 Segurança

### Antes de Publicar:

✅ Remova credenciais hardcoded (senhas padrão)
✅ Não commite arquivos sensíveis
✅ Verifique o .gitignore
✅ Revise o código para dados pessoais

### Dados Sensíveis:

- Senhas devem ser alteradas em produção
- CPF/CNPJ de teste devem ser fictícios
- Dados de exemplo não devem ser reais

---

## 🆘 Solução de Problemas

### Erro: "Permission denied"
```bash
# Verifique suas credenciais do GitHub
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"
```

### Erro: "Updates were rejected"
```bash
# Puxe as alterações primeiro
git pull origin main --rebase

# Depois envie
git push
```

### Erro: "GitHub Pages não atualiza"
- Aguarde 5-10 minutos
- Limpe o cache do navegador (Ctrl + F5)
- Verifique se o arquivo se chama `index.html`

---

## 📚 Recursos Adicionais

- [Git - Guia Básico](https://rogerdudler.github.io/git-guide/index.pt_BR.html)
- [GitHub Docs](https://docs.github.com/pt)
- [GitHub Pages](https://pages.github.com/)
- [Markdown Guide](https://www.markdownguide.org/)

---

## 🎓 Próximos Passos

Após o deploy bem-sucedido:

1. ⭐ Adicione badges no README (build, version, etc)
2. 📄 Crie uma licença (MIT recomendada)
3. 🐛 Configure Issues para reportar bugs
4. 📊 Adicione analytics (Google Analytics, etc)
5. 🚀 Configure CI/CD (GitHub Actions)
6. 📱 Transforme em PWA (Progressive Web App)

---

**Precisa de ajuda?** Abra uma [Issue](https://github.com/SEU-USUARIO/sistema-rh/issues) no GitHub!

**Boa sorte com seu projeto! 🚀**
