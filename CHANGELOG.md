# 📋 Changelog

Todas as mudanças notáveis neste projeto serão documentadas neste arquivo.

O formato é baseado em [Keep a Changelog](https://keepachangelog.com/pt-BR/1.0.0/),
e este projeto adere ao [Semantic Versioning](https://semver.org/lang/pt-BR/).

## [Não Publicado]

### Planejado para v1.1.0
- Exportação de relatórios em Excel
- Geração de PDF para holerites
- Sistema de backup/restauração
- Controle de férias
- Histórico de alterações salariais
- Gráficos de evolução

---

## [1.0.0] - 2024-12-13

### 🎉 Lançamento Inicial

#### ✨ Adicionado
- Sistema de autenticação com dois níveis de acesso (Admin/Funcionário)
- Dashboard com métricas em tempo real
- Gestão completa de empresas
  - Cadastro com validação de CNPJ
  - Edição e exclusão
  - Busca e filtros
- Gestão completa de funcionários
  - Cadastro CLT e Terceiros
  - Status (Ativo, Inativo, Férias, Afastado)
  - Validação automática de CPF
  - Campos completos (CTPS, PIS, CBO, etc)
  - Busca por nome, CPF e cargo
  - Filtro por status
- Sistema de Rendimentos
  - Geração automática de holerites
  - Cálculo de INSS (11%)
  - Cálculo de IRRF (7,5%)
  - Cálculo de Vale Transporte (6%)
  - Vale Alimentação (R$ 500 fixo)
  - Seleção de período (mês/ano)
- Registro de Jornada
  - Ponto eletrônico completo
  - Entrada, Saída Intervalo, Retorno, Saída
  - Histórico de registros
  - Visualização de registros do dia
- Sistema de Avisos
  - Publicação de comunicados
  - Categorização (Info, Atenção, Urgente, Sucesso)
  - Exclusão de avisos
- Página de Informações
  - Guia rápido de uso
  - Documentação de funcionalidades
  - Contatos de suporte
- Interface moderna e responsiva
  - Design com Tailwind CSS
  - Ícones Font Awesome
  - Compatível com mobile/tablet/desktop
- Armazenamento local (LocalStorage)
  - Persistência automática de dados
  - Funciona 100% offline

#### 🔧 Técnico
- React 18 para interface
- Tailwind CSS para estilização
- LocalStorage API para persistência
- Validação de CPF com algoritmo oficial
- Validação de CNPJ com algoritmo oficial
- Formatação automática de moeda (BRL)
- Formatação automática de documentos

#### 📚 Documentação
- README.md completo
- Manual do Usuário detalhado
- Guia de Deploy (GitHub Pages)
- Licença MIT
- .gitignore configurado
- CHANGELOG iniciado

---

## Tipos de Mudanças

- **Adicionado** - para novas funcionalidades
- **Modificado** - para mudanças em funcionalidades existentes
- **Obsoleto** - para funcionalidades que serão removidas
- **Removido** - para funcionalidades removidas
- **Corrigido** - para correções de bugs
- **Segurança** - em caso de vulnerabilidades

---

## Formato de Versionamento

```
MAJOR.MINOR.PATCH

MAJOR - Mudanças incompatíveis na API
MINOR - Novas funcionalidades compatíveis
PATCH - Correções de bugs compatíveis
```

Exemplos:
- `1.0.0` → `1.0.1` (correção de bug)
- `1.0.1` → `1.1.0` (nova funcionalidade)
- `1.1.0` → `2.0.0` (mudança incompatível)

---

## Links

- [1.0.0] - 2024-12-13 (Inicial)
- [Repositório](https://github.com/seu-usuario/sistema-rh)
- [Issues](https://github.com/seu-usuario/sistema-rh/issues)
- [Releases](https://github.com/seu-usuario/sistema-rh/releases)

---

**Mantido por:** Equipe de Desenvolvimento  
**Última atualização:** 13 de dezembro de 2024
