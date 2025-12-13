# 🏢 Sistema de Gestão de Funcionários

Sistema completo de RH para gestão de funcionários CLT e terceiros, com controle de empresas, rendimentos, jornada de trabalho e comunicados internos.

![Status](https://img.shields.io/badge/status-active-success.svg)
![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)

## 📋 Índice

- [Sobre](#sobre)
- [Funcionalidades](#funcionalidades)
- [Demonstração](#demonstração)
- [Tecnologias](#tecnologias)
- [Como Usar](#como-usar)
- [Credenciais de Teste](#credenciais-de-teste)
- [Estrutura do Projeto](#estrutura-do-projeto)
- [Roadmap](#roadmap)
- [Contribuindo](#contribuindo)
- [Licença](#licença)
- [Contato](#contato)

## 📖 Sobre

Sistema web desenvolvido para auxiliar departamentos de Recursos Humanos na gestão completa de funcionários. Oferece controle de empresas, cadastro de funcionários CLT e terceiros, geração de holerites, registro de ponto eletrônico e sistema de avisos.

**Características principais:**
- ✅ 100% funcional sem necessidade de backend
- ✅ Armazenamento local (LocalStorage)
- ✅ Interface moderna e responsiva
- ✅ Validação automática de CPF e CNPJ
- ✅ Cálculos automáticos de rendimentos
- ✅ Sistema de permissões (Admin/Funcionário)

## 🚀 Funcionalidades

### 👑 Para Administradores

- **Dashboard Completo**
  - Métricas em tempo real
  - Gráficos de status
  - Últimos cadastros
  
- **Gestão de Empresas**
  - Cadastro completo com validação de CNPJ
  - Endereço e dados de contato
  - Edição e exclusão
  
- **Gestão de Funcionários**
  - Cadastro CLT e Terceiros
  - Controle de status (Ativo, Inativo, Férias, Afastado)
  - Todos os dados trabalhistas (CTPS, PIS, CBO, etc)
  - Filtros e buscas avançadas
  
- **Rendimentos**
  - Geração automática de holerites
  - Cálculo de INSS, IRRF, descontos
  - Exportação e impressão
  
- **Avisos e Comunicados**
  - Publicação de avisos para todos
  - Categorização (Info, Atenção, Urgente, Sucesso)

### 👤 Para Funcionários

- **Meus Dados**
  - Visualização de informações pessoais
  - Dados contratuais
  
- **Meus Rendimentos**
  - Consulta de holerites
  - Histórico de pagamentos
  
- **Registro de Jornada**
  - Ponto eletrônico
  - Entrada, Intervalo, Retorno, Saída
  - Histórico de registros
  
- **Avisos**
  - Visualização de comunicados da empresa

## 🎥 Demonstração

O sistema está disponível em: [Link para GitHub Pages ou Demo]

### Screenshots

#### Dashboard
![Dashboard](docs/images/dashboard.png)

#### Gestão de Funcionários
![Funcionários](docs/images/funcionarios.png)

#### Holerite
![Holerite](docs/images/holerite.png)

## 🛠️ Tecnologias

- **React** 18 - Biblioteca JavaScript para interfaces
- **Tailwind CSS** - Framework CSS utilitário
- **Font Awesome** - Ícones
- **LocalStorage API** - Armazenamento de dados

### Por que sem backend?

Este sistema foi desenvolvido para ser executado 100% no navegador, oferecendo:
- ✅ Instalação instantânea
- ✅ Sem custos de servidor
- ✅ Funcionamento offline
- ✅ Privacidade dos dados (tudo fica no dispositivo)

## 💻 Como Usar

### Opção 1: Uso Direto

1. Clone o repositório:
```bash
git clone https://github.com/seu-usuario/sistema-rh.git
```

2. Abra o arquivo `index.html` em qualquer navegador moderno

Pronto! O sistema já está funcionando.

### Opção 2: Servidor Local

Se preferir usar um servidor local:

```bash
# Com Python 3
python -m http.server 8000

# Com Node.js (http-server)
npx http-server

# Com PHP
php -S localhost:8000
```

Acesse: `http://localhost:8000`

### Opção 3: GitHub Pages

1. Faça fork do repositório
2. Vá em Settings → Pages
3. Selecione a branch `main` como source
4. Aguarde alguns minutos
5. Acesse: `https://seu-usuario.github.io/sistema-rh`

## 🔑 Credenciais de Teste

### Administrador
- **Usuário:** `admin`
- **Senha:** `admin123`
- **Permissões:** Acesso total ao sistema

### Funcionário
- **Usuário:** `funcionario`
- **Senha:** `func123`
- **Permissões:** Visualização de dados pessoais

> ⚠️ **Atenção:** Altere as credenciais em ambiente de produção!

## 📁 Estrutura do Projeto

```
sistema-rh/
├── index.html              # Arquivo principal do sistema
├── README.md              # Este arquivo
├── LICENSE                # Licença do projeto
├── .gitignore            # Arquivos ignorados pelo Git
└── docs/                 # Documentação adicional
    ├── MANUAL.md         # Manual do usuário
    └── images/           # Screenshots
```

## 🎯 Roadmap

### Versão 1.0 (Atual) ✅
- [x] Sistema de autenticação
- [x] Cadastro de empresas
- [x] Cadastro de funcionários
- [x] Geração de holerites
- [x] Registro de ponto
- [x] Sistema de avisos

### Versão 1.1 (Próxima)
- [ ] Exportação para Excel
- [ ] Geração de PDF de holerites
- [ ] Controle de férias
- [ ] Gráficos de evolução salarial
- [ ] Histórico de alterações

### Versão 2.0 (Futuro)
- [ ] Integração com backend (opcional)
- [ ] Sistema de backup/restauração
- [ ] Múltiplos idiomas
- [ ] App mobile (PWA)
- [ ] Assinatura digital
- [ ] Integração com e-Social

## 🤝 Contribuindo

Contribuições são bem-vindas! Para contribuir:

1. Faça um Fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/NovaFuncionalidade`)
3. Commit suas mudanças (`git commit -m 'Adiciona nova funcionalidade'`)
4. Push para a branch (`git push origin feature/NovaFuncionalidade`)
5. Abra um Pull Request

### Diretrizes de Contribuição

- Mantenha o código limpo e comentado
- Siga os padrões de código existentes
- Teste suas alterações antes de enviar
- Atualize a documentação se necessário

## 📝 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 👨‍💻 Autor

**Seu Nome**

- GitHub: [@seu-usuario](https://github.com/seu-usuario)
- LinkedIn: [Seu Perfil](https://linkedin.com/in/seu-perfil)
- Email: seu.email@exemplo.com

## 📞 Contato

Tem alguma dúvida ou sugestão? Entre em contato!

- 📧 Email: suporte@exemplo.com
- 💬 Issues: [GitHub Issues](https://github.com/seu-usuario/sistema-rh/issues)
- 📖 Wiki: [Documentação Completa](https://github.com/seu-usuario/sistema-rh/wiki)

## ⭐ Apoie o Projeto

Se este projeto foi útil para você, considere dar uma ⭐ no repositório!

---

**Desenvolvido com ❤️ para facilitar a gestão de RH**

