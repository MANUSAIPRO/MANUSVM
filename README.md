# HotWallet - Aplicativo de Carteira de Criptomoedas

## Resumo do Projeto

O HotWallet é um aplicativo móvel de carteira de criptomoedas seguro e descentralizado, desenvolvido especificamente para o mercado brasileiro. O projeto foi implementado usando React Native com TypeScript e Expo, seguindo as especificações detalhadas fornecidas nos documentos de requisitos.

## Funcionalidades Implementadas

### 1. Telas Principais
- **OnboardingScreen**: Tela de boas-vindas com opções para criar nova carteira ou restaurar existente
- **SeedPhraseScreen**: Geração e exibição segura de frases semente usando bip39
- **AuthScreen**: Autenticação multi-fator com biometria e PIN
- **DashboardScreen**: Painel principal com saldo da carteira e histórico de transações
- **TransactionScreen**: Interface para envio de transações
- **SettingsScreen**: Configurações de segurança e gerenciamento de dados

### 2. Serviços de Backend
- **WalletService**: Gerenciamento de carteiras, geração de seed phrases e criação de chaves
- **BlockchainService**: Integração com redes blockchain (Ethereum, Bitcoin, Solana)
- **EncryptionService**: Criptografia AES-256 e funções de segurança
- **SecureStoreUtil**: Armazenamento seguro usando Expo SecureStore

### 3. Recursos de Segurança
- Geração segura de frases semente sem armazenamento permanente
- Criptografia AES-256 para dados em memória
- Autenticação biométrica e por PIN
- Limpeza automática de dados sensíveis
- Armazenamento seguro nativo do dispositivo

## Estrutura do Projeto

```
HotWalletApp/
├── src/
│   ├── screens/          # Telas do aplicativo
│   ├── services/         # Serviços de backend
│   ├── utils/           # Utilitários (armazenamento seguro)
│   └── navigation/      # Configuração de navegação
├── App.tsx              # Componente principal
├── package.json         # Dependências do projeto
└── tsconfig.json        # Configuração TypeScript
```

## Dependências Principais

- **React Native + Expo**: Framework de desenvolvimento
- **@react-navigation**: Sistema de navegação
- **expo-local-authentication**: Autenticação biométrica
- **expo-secure-store**: Armazenamento seguro
- **bip39**: Geração de frases semente
- **ethers**: Integração com Ethereum
- **crypto-js**: Funções criptográficas

## Paleta de Cores

O aplicativo segue a paleta especificada:
- Verde (#4CAF50): Ações positivas
- Amarelo (#FFC107): Ações secundárias
- Preto (#000): Fundo principal
- Branco (#FFF): Texto principal

## Status do Desenvolvimento

✅ **Concluído:**
- Estrutura base do projeto
- Todas as telas principais
- Serviços de segurança e blockchain
- Sistema de navegação
- Integração de dependências

⚠️ **Pendente:**
- Resolução de conflitos de dependências para execução web
- Testes em dispositivos móveis reais
- Integração completa com redes blockchain
- Deploy para lojas de aplicativos

## Próximos Passos

1. Resolver problemas de compatibilidade de dependências
2. Implementar testes unitários
3. Configurar CI/CD pipeline
4. Realizar auditoria de segurança
5. Preparar para deploy em produção

## Observações Técnicas

O projeto foi desenvolvido seguindo as melhores práticas de segurança especificadas nos documentos de requisitos, incluindo:
- Não armazenamento permanente de frases semente
- Criptografia de dados sensíveis
- Isolamento de sessões
- Limpeza automática de memória

