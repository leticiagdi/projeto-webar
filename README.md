# 🧬 Plataforma WebAR Educativa de Ciências da Vida

Uma plataforma inovadora de Realidade Aumentada via navegador (WebAR) para ensino imersivo e acessível em biologia, anatomia e bioinformática.

## 📋 Sobre o Projeto

O projeto propõe o desenvolvimento de uma **Plataforma WebAR Educativa de Ciências da Vida**, usando Realidade Aumentada via navegador (WebAR) para ensino imersivo e acessível em biologia, anatomia, e bioinformática. 

A plataforma será responsiva e permitirá a projeção e interação com modelos 3D de DNA, proteínas e partes do corpo humano (como crânio, coração e pulmões) sobre superfícies reais (mesa, parede) usando apenas um **smartphone ou tablet com câmera**, eliminando a necessidade de óculos VR dedicados.

## 🎯 Características Principais

- **WebAR Acessível**: Funciona diretamente no navegador, sem necessidade de aplicativos específicos
- **Modelos 3D Interativos**: DNA, proteínas e anatomia humana
- **Projeção em Superfícies Reais**: Mesa, parede ou qualquer superfície plana
- **Controles Intuitivos**: Rotação, escala e informações por toque
- **Feedback Multimodal**: Visual, auditivo e tátil
- **Módulos Educacionais**: Exercícios (quizzes) integrados
- **Foco em Acessibilidade**: Design inclusivo e IHC otimizada

## 🛠️ Stack Tecnológico

### Frontend (Planejado)
- **WebAR/WebXR**: Para realidade aumentada no navegador
- **Three.js**: Renderização 3D e manipulação de modelos
- **React**: Interface de usuário responsiva
- **GLTF/GLB**: Formato otimizado para modelos 3D

### Backend (Atual)
- **Node.js**: Servidor de aplicação
- **Express.js**: Framework web
- **MongoDB**: Banco de dados NoSQL
- **Mongoose**: ODM para MongoDB

## 📱 Funcionalidades Planejadas

### Seis Telas/Estados Principais:
1. **Tela Inicial**: Seleção de categorias (DNA, Proteínas, Anatomia)
2. **Tela de Conteúdos**: Lista de modelos disponíveis por categoria
4. **Tela de Informações**: Detalhes científicos dos modelos
5. **Tela de Exercícios**: Quizzes interativos
6. **Tela de Configurações**: Preferências e acessibilidade

## 🚀 Status Atual do Projeto

**🔧 Em Desenvolvimento - Fase Backend**

Atualmente, o projeto conta apenas com o **backend**, que inclui:

- ✅ Servidor Express.js configurado
- ✅ Conexão com MongoDB
- ✅ Modelos de dados (Content e User)
- ✅ Rotas CRUD para conteúdos
- ✅ Rotas de gerenciamento de usuários
- ✅ Estrutura modular organizada

### Estrutura Atual do Backend:
```
src/server/
├── index.js              # Servidor principal
├── models/
│   ├── contentModel.js   # Modelo de conteúdos 3D
│   └── userModel.js      # Modelo de usuários
└── routes/
    ├── contentRoutes.js  # CRUD de conteúdos
    └── userRoutes.js     # Gerenciamento de usuários
```

## 🗄️ Modelos de Dados

### Content (Conteúdos 3D)
- **tema**: DNA | Proteínas | Anatomia
- **titulo**: Nome do modelo
- **marker_key**: Chave para identificação AR
- **glb_file_name**: Nome do arquivo 3D
- **textoExplicativo**: Informações detalhadas

### User (Usuários)
- **nomeCompleto**: Nome do usuário
- **email**: Email único
- **password**: Senha (será criptografada)
- **role**: Papel do usuário (student/teacher/admin)

## 🚀 Como Executar (Backend)

### Pré-requisitos
- Node.js (v14+)
- MongoDB
- npm ou yarn

### Instalação
```bash
# Clone o repositório
git clone https://github.com/leticiagdi/projeto-webar.git

# Entre no diretório
cd projeto-webar

# Instale as dependências
npm install

# Configure as variáveis de ambiente
# Crie um arquivo .env com:
# MONGODB_URI=sua_string_de_conexao_mongodb

# Execute o servidor
npm run server
```

O servidor estará disponível em `http://localhost:5000`

## 📡 API Endpoints (Disponíveis)

### Conteúdos
- `GET /api/content` - Listar todos os conteúdos
- `POST /api/content` - Criar novo conteúdo
- `GET /api/content/:id` - Buscar conteúdo por ID
- `PUT /api/content/:id` - Atualizar conteúdo
- `DELETE /api/content/:id` - Remover conteúdo

### Usuários
- `POST /api/user` - Criar novo usuário
- `GET /api/user` - Listar usuários
- `GET /api/user/:id` - Buscar usuário por ID
- `PUT /api/user/:id` - Atualizar usuário
- `DELETE /api/user/:id` - Remover usuário

## 🎯 Próximos Passos

1. **Frontend React**: Desenvolvimento da interface de usuário
2. **Integração WebAR**: Implementação da realidade aumentada
3. **Modelos 3D**: Criação e otimização dos assets GLTF/GLB
4. **Sistema de Autenticação**: JWT e segurança
5. **Módulos Educacionais**: Sistema de quizzes
6. **Testes**: Implementação de testes 
7. **Deploy**: Configuração para produção

## 🤝 Contribuindo

Este projeto está em desenvolvimento ativo. Contribuições são bem-vindas!

## 👥 Equipe

- **Desenvolvedores**: Letícia de Assis Godoi, Taina Machado Selayaran
- **Orientação**: Isabel Cristina Siqueira da Silva
- **Instituição**: UFCSPA (Universidade Federal de Ciências da Saúde de Porto Alegre)

---

**🔬 Educação + 🚀 Tecnologia + 🧬 Ciências da Vida = Futuro da Aprendizagem**
