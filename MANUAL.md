# 📚 Manual do Usuário - Sistema de Gestão de Funcionários

## Índice
1. [Introdução](#introdução)
2. [Acesso ao Sistema](#acesso-ao-sistema)
3. [Dashboard](#dashboard)
4. [Gestão de Empresas](#gestão-de-empresas)
5. [Gestão de Funcionários](#gestão-de-funcionários)
6. [Rendimentos](#rendimentos)
7. [Registro de Jornada](#registro-de-jornada)
8. [Avisos](#avisos)
9. [Perguntas Frequentes](#perguntas-frequentes)
10. [Solução de Problemas](#solução-de-problemas)

---

## 1. Introdução

O **Sistema de Gestão de Funcionários** é uma ferramenta completa para gerenciar recursos humanos de sua empresa, incluindo controle de funcionários CLT e terceiros, empresas, rendimentos, jornada de trabalho e comunicados.

### Principais Recursos
- ✅ Cadastro ilimitado de empresas e funcionários
- ✅ Geração automática de holerites
- ✅ Ponto eletrônico integrado
- ✅ Sistema de avisos e comunicados
- ✅ Validação automática de documentos (CPF/CNPJ)
- ✅ Interface moderna e intuitiva

---

## 2. Acesso ao Sistema

### 2.1 Como Acessar

1. Abra o arquivo `index.html` em seu navegador
2. Será exibida a tela de login
3. Digite suas credenciais

### 2.2 Credenciais Padrão

**Administrador:**
- Usuário: `admin`
- Senha: `admin123`

**Funcionário (Exemplo):**
- Usuário: `funcionario`
- Senha: `func123`

> ⚠️ **Importante:** Altere as senhas padrão em ambiente de produção!

### 2.3 Tipos de Usuário

#### 👑 Administrador
Acesso total ao sistema:
- Cadastrar/editar/excluir empresas
- Cadastrar/editar/excluir funcionários
- Visualizar todos os dados
- Publicar avisos
- Acessar todas as funcionalidades

#### 👤 Funcionário
Acesso limitado:
- Visualizar apenas seus próprios dados
- Consultar rendimentos
- Registrar ponto
- Ver avisos publicados

---

## 3. Dashboard

### 3.1 Visão Geral

O Dashboard é a página inicial após o login e apresenta:

- **Cards de Métricas**
  - Total de Empresas
  - Total de Funcionários
  - Funcionários Ativos
  - Funcionários CLT

- **Gráficos**
  - Status dos Funcionários
  - Tipo de Vínculo

- **Últimos Cadastros**
  - Tabela com os 5 funcionários mais recentes

### 3.2 Como Interpretar

- **Verde:** Informações positivas/ativas
- **Vermelho:** Informações negativas/inativas
- **Amarelo:** Alertas/atenção
- **Azul:** Informações neutras

---

## 4. Gestão de Empresas

### 4.1 Cadastrar Nova Empresa

1. Clique em **"Empresas"** no menu lateral
2. Clique no botão **"Nova Empresa"**
3. Preencha os campos obrigatórios:
   - Razão Social *
   - CNPJ * (será validado automaticamente)
4. Preencha os campos opcionais:
   - Endereço
   - Bairro
   - Cidade
   - Estado
5. Clique em **"Salvar"**

### 4.2 Editar Empresa

1. Na lista de empresas, clique no ícone de **editar** (lápis)
2. Modifique os campos desejados
3. Clique em **"Salvar"**

### 4.3 Excluir Empresa

1. Na lista de empresas, clique no ícone de **excluir** (lixeira)
2. Confirme a exclusão na mensagem de confirmação

> ⚠️ **Atenção:** A exclusão é permanente e não pode ser desfeita!

### 4.4 Buscar Empresa

- Use o campo de busca para filtrar por:
  - Razão Social
  - CNPJ

---

## 5. Gestão de Funcionários

### 5.1 Cadastrar Novo Funcionário

1. Clique em **"Funcionários"** no menu lateral
2. Clique no botão **"Novo Funcionário"**
3. Preencha os campos obrigatórios:
   - Nome Completo *
   - CPF * (será validado)
   - Cargo *
   - Data de Admissão *
   - Tipo de Vínculo * (CLT/Terceiro)
   - Status * (Ativo/Inativo/Férias/Afastado)
4. Preencha os campos opcionais:
   - RG, CBO, CTPS, PIS
   - Departamento
   - Salário Base
   - Email, Telefone
   - Endereço completo
   - Empresa
5. Clique em **"Salvar"**

### 5.2 Editar Funcionário

1. Na lista de funcionários, clique no ícone de **editar**
2. Modifique os campos desejados
3. Clique em **"Salvar"**

### 5.3 Excluir Funcionário

1. Na lista de funcionários, clique no ícone de **excluir**
2. Confirme a exclusão

### 5.4 Filtros e Buscas

**Campo de Busca:**
- Nome
- CPF
- Cargo

**Filtro de Status:**
- Todos
- Ativo
- Inativo
- Férias
- Afastado

---

## 6. Rendimentos

### 6.1 Consultar Holerite

1. Clique em **"Rendimentos"** no menu lateral
2. Selecione o **funcionário**
3. Selecione o **mês**
4. Selecione o **ano**
5. O holerite será gerado automaticamente

### 6.2 Entendendo o Holerite

**Proventos:**
- Salário Base
- Vale Alimentação (fixo: R$ 500,00)

**Descontos:**
- INSS (11% do salário base)
- IRRF (7,5% do salário base)
- Vale Transporte (6% do salário base)

**Salário Líquido:**
- = Proventos - Descontos

### 6.3 Ações Disponíveis

- **Baixar PDF** - Download do holerite
- **Imprimir** - Impressão direta

> 💡 **Dica:** Os cálculos são automáticos e seguem as regras trabalhistas padrão

---

## 7. Registro de Jornada

### 7.1 Como Registrar Ponto

1. Clique em **"Jornada"** no menu lateral
2. Confirme a **data** (padrão: hoje)
3. Clique no tipo de registro:
   - **Entrada** (início do expediente)
   - **Saída Intervalo** (início do almoço/intervalo)
   - **Retorno Intervalo** (fim do almoço/intervalo)
   - **Saída** (fim do expediente)

### 7.2 Visualizar Registros

**Registros de Hoje:**
- Painel lateral mostra todos os registros do dia atual

**Histórico Completo:**
- Tabela na parte inferior mostra todos os registros históricos

### 7.3 Cores dos Registros

- 🟢 **Verde:** Entrada
- 🔴 **Vermelho:** Saída
- 🟡 **Amarelo:** Intervalo (saída e retorno)

---

## 8. Avisos

### 8.1 Visualizar Avisos (Todos)

1. Clique em **"Avisos"** no menu lateral
2. Todos os avisos publicados serão exibidos

### 8.2 Criar Aviso (Apenas Administrador)

1. Clique em **"Novo Aviso"**
2. Preencha:
   - **Título:** Assunto do aviso
   - **Tipo:** 
     - Informação (azul)
     - Atenção (amarelo)
     - Sucesso (verde)
     - Urgente (vermelho)
   - **Conteúdo:** Mensagem completa
3. Clique em **"Publicar"**

### 8.3 Excluir Aviso (Apenas Administrador)

1. Clique no ícone de **lixeira** no aviso
2. Confirme a exclusão

---

## 9. Perguntas Frequentes

### 9.1 Geral

**P: Os dados ficam salvos?**
R: Sim! Todos os dados são salvos automaticamente no navegador (LocalStorage).

**P: Posso usar em vários computadores?**
R: Não. Os dados ficam salvos localmente em cada navegador.

**P: Como fazer backup dos dados?**
R: Atualmente não há função de backup. Recomendamos exportar as informações importantes.

**P: O sistema funciona offline?**
R: Sim! Após carregar pela primeira vez, funciona sem internet.

### 9.2 Cadastros

**P: Posso cadastrar quantos funcionários?**
R: Sim! Não há limite de cadastros.

**P: O CPF é obrigatório?**
R: Sim, e precisa ser válido (com validação automática).

**P: Posso ter funcionários CLT e Terceiros?**
R: Sim! Basta selecionar o tipo de vínculo no cadastro.

### 9.3 Rendimentos

**P: Como são calculados os descontos?**
R: INSS 11%, IRRF 7,5%, Vale Transporte 6% do salário base.

**P: Posso alterar as porcentagens?**
R: Atualmente não. Os valores são fixos no sistema.

### 9.4 Jornada

**P: Posso corrigir um registro errado?**
R: Atualmente não há edição de registros. Entre em contato com o administrador.

**P: Quanto tempo ficam salvos os registros?**
R: Permanentemente, enquanto não limpar o cache do navegador.

---

## 10. Solução de Problemas

### 10.1 Problemas Comuns

**Problema: Não consigo fazer login**
- Verifique usuário e senha
- Certifique-se de que está usando as credenciais corretas
- Teste com: admin / admin123

**Problema: Dados desapareceram**
- Verifique se não limpou o cache/cookies do navegador
- Dados são salvos localmente e podem ser perdidos ao limpar o navegador

**Problema: CPF/CNPJ não é aceito**
- Verifique se o número está correto
- O sistema valida automaticamente documentos inválidos

**Problema: Tela fica em branco**
- Atualize a página (F5)
- Limpe o cache do navegador
- Teste em outro navegador

### 10.2 Navegadores Recomendados

✅ Google Chrome (versão 90+)
✅ Mozilla Firefox (versão 88+)
✅ Microsoft Edge (versão 90+)
✅ Safari (versão 14+)

### 10.3 Requisitos Mínimos

- Navegador moderno atualizado
- JavaScript habilitado
- LocalStorage habilitado
- Resolução mínima: 1024x768

---

## 📞 Suporte

Em caso de dúvidas ou problemas:

- 📧 **Email:** suporte@empresa.com.br
- 📞 **Telefone:** (67) 3333-4444
- ⏰ **Horário:** Segunda a Sexta, 8h às 18h

---

**Versão do Manual:** 1.0.0  
**Última Atualização:** Dezembro 2024

*Este manual está em constante atualização. Sugestões são bem-vindas!*
