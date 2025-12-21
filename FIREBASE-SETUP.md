# Configuração do Firebase - Sistema RH InstaSolutions

## 1. Regras de Segurança do Firestore

Acesse o [Console do Firebase](https://console.firebase.google.com/), selecione o projeto `sistema-rh-instasolutions`, vá em **Firestore Database** > **Regras** e substitua as regras por:

```javascript
rules_version = '2';
service cloud.firestore {
  match /databases/{database}/documents {
    // Regras para a coleção sistemaRH
    match /sistemaRH/{document=**} {
      // Permite leitura e escrita para todos (modo desenvolvimento)
      // Em produção, recomenda-se implementar autenticação
      allow read, write: if true;
    }
  }
}
```

> ⚠️ **IMPORTANTE**: Essas regras permitem acesso público para facilitar o desenvolvimento. Para produção, implemente autenticação adequada.

## 2. Para Produção (Recomendado)

### Ativar Autenticação
1. No console Firebase, vá em **Authentication** > **Sign-in method**
2. Ative os provedores desejados (Email/Senha, Google, etc.)

### Regras com Autenticação
```javascript
rules_version = '2';
service cloud.firestore {
  match /databases/{database}/documents {
    match /sistemaRH/{document=**} {
      // Permite acesso apenas para usuários autenticados
      allow read, write: if request.auth != null;
    }
  }
}
```

## 3. Estrutura dos Dados no Firestore

O sistema armazena todos os dados em um único documento:

```
sistemaRH/
  └── dados/
      ├── empresas: []
      ├── funcionarios: []
      ├── avisos: []
      ├── registrosPonto: []
      ├── holerites: []
      ├── solicitacoesFerias: []
      ├── historicoFerias: []
      ├── feriadosPontoFacultativo: []
      ├── documentos: []
      ├── planosSaude: []
      └── updatedAt: timestamp
```

## 4. Backup Local

O sistema mantém um backup automático no localStorage do navegador. Se o Firebase falhar, os dados locais são usados como fallback.

## 5. Testando

1. Abra o sistema em dois navegadores diferentes
2. Faça login como admin em ambos
3. Adicione um funcionário em um navegador
4. Recarregue o outro navegador - o funcionário deve aparecer!

## 6. Deploy no GitHub Pages

O sistema está pronto para deploy no GitHub Pages. O Firebase funciona perfeitamente com sites estáticos.

```bash
git add .
git commit -m "Integração Firebase Firestore"
git push origin main
```

Depois, ative o GitHub Pages nas configurações do repositório.
