# 🏢 Sistema de Gestão de Funcionários v2.0

Sistema completo e otimizado de RH para gestão de funcionários CLT e terceiros, com todas as funcionalidades solicitadas.

![Status](https://img.shields.io/badge/status-pronto-success.svg)
![Version](https://img.shields.io/badge/version-2.0.0-blue.svg)

## 🎉 NOVIDADES DA VERSÃO 2.0

### ✅ Correções Implementadas

**1. Todos os Estados Brasileiros ✓**
- 27 estados completos (AC, AL, AP, AM, BA, CE, DF, ES, GO, MA, MT, MS, MG, PA, PB, PR, PE, PI, RJ, RN, RS, RO, RR, SC, SP, SE, TO)
- Implementado tanto no cadastro de empresas quanto de funcionários

**2. Sistema de Rendimentos Reformulado ✓**
- **Campos Manuais** (sem cálculo automático):
  - Salário Mensalista
  - Auxílio Combustível
  - Prêmio Motivacional
  - Arredondamento Provento Folha
  - INSS
  - IR
- **Upload de Holerite**: Anexar PDF/imagem do holerite original
- **Download**: Funcionário pode baixar o arquivo anexado
- **Visualização Profissional**: Layout baseado no holerite real da empresa

**3. Registro de Jornada Avançado ✓**
- **Filtros Completos**:
  - Por funcionário
  - Por data (início e fim)
  - Por empresa
- **Edição de Registros**: Admin pode editar tipo, data e hora
- **Criação Manual**: Admin pode criar registros e vincular a funcionários
- **Geração de PDF**: 
  - Cabeçalho com dados da empresa
  - Dados do funcionário
  - Tabela completa de registros
  - Período filtrado

**4. Sistema de Avisos Melhorado ✓**
- **Marcação de Lido**: Funcionários marcam avisos como lidos
- **Badge de Notificação**: Contador de avisos não lidos no menu
- **Filtros**: Todos / Lidos / Não Lidos
- **Destaque Visual**: Avisos não lidos com fundo diferenciado

**5. Gestão de Férias Completa ✓**
- **Cálculo Automático**: 
  - Período aquisitivo
  - Meses restantes até vencimento
  - Data de vencimento
- **Solicitações**: Funcionários solicitam férias
- **Aprovações**: Admin aprova ou rejeita solicitações
- **Férias Coletivas**: 
  - 15 dias em dezembro (fixo)
  - 15 dias de livre escolha do funcionário
- **Status**: Pendente / Aprovado / Rejeitado

**6. Controle de Feriados ✓**
- **Feriados Nacionais 2025**: Lista completa pré-cadastrada
- **Pontos Facultativos**: Admin marca dias sem expediente (emendas)
- **Notificações Automáticas**: 
  - Alerta até 5 dias antes do feriado
  - Alertas diários até passar a data
- **Calendário Anual**: Visualização por ano

**7. Gestão de Documentos ✓**
- **Upload de Arquivos**: PDF, imagens, Word, etc
- **Armazenamento Seguro**: Base64 no localStorage
- **Download**: Baixar documentos enviados
- **Organização**: Por funcionário
- **Informações**: Nome, tamanho, data de envio

## 📋 Funcionalidades Completas

### 👑 Para Administradores

- ✅ Dashboard com métricas em tempo real
- ✅ Cadastro de Empresas (todos os estados)
- ✅ Cadastro de Funcionários (todos os estados, CLT e Terceiros)
- ✅ **Gestão de Holerites**:
  - Cadastrar valores manualmente
  - Anexar arquivo do holerite
  - Visualizar holerites cadastrados
- ✅ **Registro de Ponto**:
  - Filtrar por funcionário, data, empresa
  - Criar registros manualmente
  - Editar registros existentes
  - Gerar PDF com filtros
  - Excluir registros
- ✅ **Gestão de Férias**:
  - Ver todas as solicitações
  - Aprovar ou rejeitar
  - Controle de períodos
- ✅ **Feriados**:
  - Visualizar feriados nacionais
  - Marcar pontos facultativos (emendas)
  - Gerenciar calendário
- ✅ **Avisos**:
  - Publicar comunicados
  - Ver quantos leram
  - Excluir avisos
- ✅ **Documentos**:
  - Upload de arquivos
  - Gerenciar documentos
  - Download

### 👤 Para Funcionários

- ✅ Dashboard personalizado
- ✅ **Holerites**:
  - Visualizar holerites mensais
  - Baixar arquivo anexado
  - Imprimir
- ✅ **Ponto Eletrônico**:
  - Registrar entrada, saída, intervalos
  - Ver registros do dia
  - Histórico completo
- ✅ **Férias**:
  - Ver prazo de vencimento
  - Solicitar férias
  - Acompanhar status das solicitações
- ✅ **Feriados**:
  - Ver feriados do ano
  - Notificações de dias sem expediente
- ✅ **Avisos**:
  - Ler avisos da empresa
  - Marcar como lido
  - Filtrar lidos/não lidos
- ✅ **Documentos**:
  - Enviar documentos atualizados
  - Download dos documentos

## 🚀 Como Usar

### Instalação

1. Baixe o arquivo `index.html`
2. Abra diretamente no navegador
3. Pronto! O sistema já está funcionando

**Não precisa de:**
- ❌ Servidor
- ❌ Banco de dados
- ❌ Instalação
- ❌ Configuração

### Credenciais Padrão

**Administrador:**
- Usuário: `admin`
- Senha: `admin123`

**Funcionário:**
- Usuário: `CPF do funcionário cadastrado`
- Senha: `func123`

> ⚠️ **Importante**: Altere as senhas em produção!

## 💾 Armazenamento

- **Tecnologia**: LocalStorage (navegador)
- **Capacidade**: Até 10MB de dados
- **Persistência**: Dados salvos automaticamente
- **Backup**: Recomendado exportar dados periodicamente

## 🎯 Estrutura de Dados

O sistema armazena:
- Empresas
- Funcionários
- Holerites (com arquivos em Base64)
- Registros de Ponto
- Solicitações de Férias
- Feriados e Pontos Facultativos
- Avisos
- Documentos (em Base64)

## 📱 Compatibilidade

- ✅ Chrome 90+
- ✅ Firefox 88+
- ✅ Edge 90+
- ✅ Safari 14+
- ✅ Dispositivos móveis
- ✅ Tablets

## 🔒 Segurança

- Dados armazenados localmente (privacidade)
- Validação de CPF e CNPJ
- Controle de acesso por tipo de usuário
- Sem exposição de dados a servidores externos

## 🎨 Interface

- Design moderno com Tailwind CSS
- Responsivo (mobile-first)
- Ícones Font Awesome
- Cores intuitivas para status
- Feedback visual em todas as ações

## 📊 Performance

- Otimizado para até 1000 funcionários
- Carregamento instantâneo
- Busca e filtros rápidos
- Geração de PDF otimizada

## 🆕 Mudanças em Relação à Versão 1.0

### Removido
- ❌ Cálculo automático de rendimentos

### Adicionado
- ✅ Todos os 27 estados brasileiros
- ✅ Upload de arquivos de holerite
- ✅ Campos manuais para holerite (conforme contabilidade)
- ✅ Edição de registros de ponto
- ✅ Criação manual de ponto pelo admin
- ✅ Filtros avançados de jornada
- ✅ Geração de PDF de ponto
- ✅ Sistema completo de férias
- ✅ Controle de feriados e pontos facultativos
- ✅ Notificações de feriados próximos
- ✅ Avisos com marcação de lido/não lido
- ✅ Upload e download de documentos
- ✅ Badge de notificações

### Melhorado
- ✅ Performance geral
- ✅ Interface do usuário
- ✅ Organização do código
- ✅ Armazenamento de dados
- ✅ Dashboard personalizado

## 📝 Exemplo de Uso - Holerite

### Fluxo Admin:
1. Acessa "Rendimentos"
2. Seleciona funcionário e mês/ano
3. Clica em "Cadastrar Holerite"
4. Preenche os valores recebidos da contabilidade:
   - Salário Mensalista: 2.375,40
   - Auxílio Combustível: 529,90
   - Prêmio Motivacional: 900,00
   - Arredondamento: 0,67
   - INSS: 191,01
   - IR: 17,96
5. Anexa o PDF do holerite
6. Salva

### Fluxo Funcionário:
1. Acessa "Holerites"
2. Seleciona mês/ano
3. Visualiza o holerite formatado
4. Baixa o arquivo PDF anexado
5. Pode imprimir

## 🔧 Próximas Melhorias Sugeridas

- [ ] Exportação para Excel
- [ ] Backup e restauração
- [ ] Relatórios gerenciais
- [ ] Gráficos de evolução
- [ ] App PWA (offline)
- [ ] Integração com e-Social (futuro)

## 📞 Suporte

- Email: suporte@empresa.com.br
- Telefone: (67) 3333-4444
- Horário: Segunda a Sexta, 8h às 18h

## 📄 Licença

MIT License - Uso livre

---

**Desenvolvido com ❤️ para facilitar a gestão de RH**

**Versão**: 2.0.0  
**Data**: Dezembro 2024  
**Status**: ✅ Produção
