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
3. **Tela AR Principal**: 
   - Modo de exploração livre
   - Modo guiado
   - Controles por toque
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
import reactDom from 'eslint-plugin-react-dom'

export default defineConfig([
  globalIgnores(['dist']),
  {
    files: ['**/*.{ts,tsx}'],
    extends: [
      // Other configs...
      // Enable lint rules for React
      reactX.configs['recommended-typescript'],
      // Enable lint rules for React DOM
      reactDom.configs.recommended,
    ],
    languageOptions: {
      parserOptions: {
        project: ['./tsconfig.node.json', './tsconfig.app.json'],
        tsconfigRootDir: import.meta.dirname,
      },
      // other options...
    },
  },
])
```
