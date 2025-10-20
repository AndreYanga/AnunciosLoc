# AnunciosLoc - Front-end Mobile Web

## 📱 Visão Geral

O **AnunciosLoc** é um sistema de anúncios baseado em localização desenvolvido como aplicação mobile web. Este front-end implementa todas as funcionalidades especificadas no enunciado do projeto, proporcionando uma experiência de utilizador moderna e intuitiva.

## 🎯 Alinhamento com o Enunciado

Este front-end implementa fielmente os requisitos especificados no PDF do projeto:

### ✅ Funcionalidades Base Implementadas (F1-F6)

- **F1 - Registar utilizador**: Formulário completo de registo
- **F2 - Log in/out**: Sistema de autenticação com sessões
- **F3 - Listar/Criar/Remover locais**: Gestão completa de locais
- **F4 - Registar anúncio**: Criação de anúncios com políticas avançadas
- **F5 - Visualizar anúncio**: Interface detalhada para leitura de mensagens
- **F6 - Editar perfil**: Gestão de atributos e informações pessoais

### ✅ Características Técnicas do Enunciado

- **Coordenadas GPS**: Implementado com latitude, longitude e raio
- **WiFi/BLE**: Suporte para identificadores de rede
- **Políticas de visibilidade**: Whitelist, blacklist e janelas de tempo
- **Modos de entrega**: Centralizada (servidor) e Descentralizada (WiFi Direct)
- **Perfis de utilizador**: Atributos key-value para segmentação
- **Localização**: Contexto angolano com locais reais

## 📄 Estrutura das Páginas

### 🏠 **index.html** - Página Inicial
**Função**: Dashboard principal com visão geral do sistema
**Alinhamento com enunciado**: 
- Mostra locais próximos conforme especificado
- Exibe estatísticas do sistema (locais, anúncios, utilizadores)
- Interface para descobrir anúncios baseados em localização
- Suporte para GPS e WiFi Direct conforme requisitos

**Características do Front-end**:
- Hero section com gradiente e informações de localização
- Barra de pesquisa avançada
- Filtros por categoria (Comércio, Educação, Desporto)
- Cards de estatísticas em tempo real
- Lista de locais com status, distância e número de anúncios
- Indicadores de tipo de localização (GPS, WiFi, BLE)

### 🔐 **registro.html** - Registo de Utilizador (F1)
**Função**: Criação de novas contas de utilizador
**Alinhamento com enunciado**:
- Implementa F1 conforme especificado
- Validação de nome de utilizador único
- Campos obrigatórios: nome de utilizador e palavra-passe
- Redirecionamento para login após registo bem-sucedido

**Características do Front-end**:
- Design minimalista e focado
- Validação visual em tempo real
- Confirmação de palavra-passe
- Link direto para página de login
- Responsivo para mobile

### 🔑 **login.html** - Iniciar Sessão (F2)
**Função**: Autenticação de utilizadores existentes
**Alinhamento com enunciado**:
- Implementa F2 conforme especificado
- Validação de credenciais (nome de utilizador e palavra-passe)
- Geração de ID de sessão após login bem-sucedido
- Navegação para funcionalidades principais

**Características do Front-end**:
- Interface limpa e profissional
- Navegação inferior para acesso rápido
- Link para registo de novos utilizadores
- Feedback visual para estados de loading
- Suporte para modo escuro

### 📍 **locais.html** - Gestão de Locais (F3)
**Função**: Listar, criar e remover locais do sistema
**Alinhamento com enunciado**:
- Implementa F3 conforme especificado
- Suporte para coordenadas GPS (latitude, longitude, raio)
- Suporte para IDs WiFi/BLE
- Gestão de locais globais (criados por qualquer utilizador)
- Possibilidade de remover locais de outros utilizadores

**Características do Front-end**:
- Lista visual de locais com ícones categorizados
- Exibição de coordenadas GPS e IDs de rede
- Botão flutuante para criar novos locais
- Interface para gestão (editar/remover)
- Indicadores visuais de tipo de localização

### ➕ **criar_local.html** - Criar Novo Local
**Função**: Formulário para adicionar novos locais ao sistema
**Alinhamento com enunciado**:
- Suporte completo para especificação de locais
- Coordenadas GPS com latitude, longitude e raio
- IDs WiFi/BLE para detecção de rede
- Validação de dados de entrada
- Integração com sistema de locais globais

**Características do Front-end**:
- Formulário multi-seção organizado
- Toggle entre GPS e WiFi/BLE
- Botão para usar localização atual
- Detecção automática de redes próximas
- Configurações de visibilidade e permissões

### 📢 **anuncios.html** - Lista de Anúncios
**Função**: Visualização de todos os anúncios disponíveis
**Alinhamento com enunciado**:
- Exibe anúncios baseados em localização
- Mostra informações do publicador e local
- Suporte para políticas de visibilidade
- Interface para interação (gostar, comentar, guardar)

**Características do Front-end**:
- Filtros interativos (Todos, Próximos, Recentes, Guardados)
- Cards de anúncios com avatares e badges
- Sistema de badges para categorização
- Contadores de interações (gostos, comentários, guardados)
- Links para visualização detalhada

### ✍️ **criar_anuncio.html** - Criar Anúncio (F4)
**Função**: Formulário para publicação de novos anúncios
**Alinhamento com enunciado**:
- Implementa F4 conforme especificado
- Políticas de visibilidade (whitelist, blacklist, janelas de tempo)
- Modos de entrega (centralizada e descentralizada)
- Seleção de local de destino
- Configurações de agendamento

**Características do Front-end**:
- Formulário multi-seção com validação
- Seleção de local com emojis para identificação
- Políticas de visibilidade com descrições claras
- Toggle entre modos de entrega com explicações
- Sistema de agendamento opcional
- Contador de caracteres para mensagem

### 👁️ **visualizar_anuncio.html** - Visualizar Anúncio (F5)
**Função**: Interface detalhada para leitura de anúncios
**Alinhamento com enunciado**:
- Implementa F5 conforme especificado
- Exibe conteúdo completo da mensagem
- Mostra nome do publicador e hora de publicação
- Informações de localização
- Sistema de interações

**Características do Front-end**:
- Layout focado na leitura
- Header com informações do publicador
- Conteúdo da mensagem bem formatado
- Barra de interações (gostar, comentar, guardar)
- Botão para guardar anúncio
- Navegação inferior consistente

### 👤 **perfil.html** - Perfil do Utilizador (F6)
**Função**: Visualização e gestão do perfil pessoal
**Alinhamento com enunciado**:
- Implementa F6 conforme especificado
- Exibe atributos do perfil (key-value pairs)
- Informações pessoais e de contacto
- Acesso às configurações
- Opção de logout

**Características do Front-end**:
- Seções organizadas (Informações Pessoais, Atributos, Ações)
- Cards informativos com ícones
- Links para edição e configurações
- Botão de logout destacado
- Navegação inferior com perfil ativo

### ✏️ **editar_perfil.html** - Editar Perfil
**Função**: Formulário para modificação de dados pessoais
**Alinhamento com enunciado**:
- Permite alteração de atributos do perfil
- Adição/remoção de pares key-value
- Gestão de informações pessoais
- Configurações de privacidade

**Características do Front-end**:
- Upload de foto de perfil
- Formulário organizado por seções
- Seleção de profissão e clube de futebol
- Configurações de privacidade com toggles
- Validação de dados de entrada

### ⚙️ **configuracoes.html** - Configurações do Sistema
**Função**: Gestão de configurações da aplicação
**Alinhamento com enunciado**:
- Configurações de rede (WiFi Direct, GPS, Bluetooth)
- Configurações de notificações
- Configurações de privacidade
- Gestão de conta

**Características do Front-end**:
- Seções organizadas (Geral, Rede, Conta)
- Toggles para ativar/desativar funcionalidades
- Configurações de rede específicas do projeto
- Links para gestão de conta
- Interface consistente com resto da aplicação

## 🎨 Design System

### Cores
- **Primary**: #13a4ec (Azul principal)
- **Primary Dark**: #0d7bb8 (Azul escuro)
- **Secondary**: #f59e0b (Laranja)
- **Success**: #10b981 (Verde)
- **Warning**: #f59e0b (Amarelo)
- **Error**: #ef4444 (Vermelho)

### Tipografia
- **Fonte Principal**: Space Grotesk (300, 400, 500, 600, 700)
- **Ícones**: Material Symbols Outlined

### Componentes
- **Cards**: Bordas arredondadas com sombras suaves
- **Botões**: Gradientes e estados hover
- **Formulários**: Validação visual e feedback
- **Navegação**: Bottom navigation consistente

## 📱 Responsividade

- **Mobile-first**: Otimizado para dispositivos móveis
- **Breakpoints**: Adaptável a diferentes tamanhos de ecrã
- **Touch-friendly**: Elementos com tamanho adequado para toque
- **Performance**: Carregamento rápido e animações suaves

## 🌍 Contexto Local

### Locais Angolanos Implementados
- **Largo da Independência**: Centro histórico de Luanda
- **Belas Shopping**: Centro comercial principal
- **Ginásio do Camama I**: Instalação desportiva
- **Universidade Agostinho Neto**: Instituição de ensino superior
- **Mercado do Benfica**: Mercado tradicional

### Dados Fictícios Realistas
- Utilizadores com nomes angolanos
- Anúncios relevantes ao contexto local
- Estatísticas realistas do sistema
- Interações sociais autênticas

## 🔧 Tecnologias Utilizadas

- **HTML5**: Estrutura semântica
- **CSS3**: Estilos modernos com Tailwind CSS
- **JavaScript**: Interações e validações
- **Tailwind CSS**: Framework de CSS utilitário
- **Material Symbols**: Biblioteca de ícones
- **Google Fonts**: Tipografia Space Grotesk

## 🚀 Funcionalidades Avançadas

### Políticas de Visibilidade
- **Whitelist**: Apenas utilizadores específicos
- **Blacklist**: Excluir utilizadores específicos
- **Janelas de tempo**: Horários específicos
- **Atributos**: Baseado em profissão, idade, clube, etc.

### Modos de Entrega
- **Centralizada**: Através do servidor (mais rápida)
- **Descentralizada**: WiFi Direct peer-to-peer (mais privada)

### Tipos de Localização
- **GPS**: Coordenadas geográficas com raio
- **WiFi**: Identificadores de rede WiFi
- **BLE**: Beacons Bluetooth Low Energy

## 📊 Métricas de Implementação

- **11 páginas** totalmente funcionais
- **6 funcionalidades base** (F1-F6) implementadas
- **100% em português** conforme requisito
- **Design responsivo** para mobile web
- **Dados fictícios realistas** para demonstração
- **Navegação consistente** entre todas as páginas

## 🎯 Conclusão

Este front-end implementa completamente os requisitos do enunciado do projeto AnunciosLoc, proporcionando uma experiência de utilizador moderna, intuitiva e totalmente funcional. O design é profissional, responsivo e otimizado para mobile web, com dados fictícios realistas que demonstram perfeitamente as capacidades do sistema.

A aplicação está pronta para apresentação e demonstração, representando fielmente a visão do projeto especificado no enunciado PDF.
