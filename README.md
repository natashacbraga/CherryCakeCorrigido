# Cherry Cupcake Store 🧁

Uma aplicação de e-commerce completa e premium para a Cherry Cupcake Store, desenvolvida com React, TypeScript e Tailwind CSS. O sistema oferece uma experiência de compra sofisticada com design responsivo e funcionalidades administrativas.

## 🌟 Características Principais

- **E-commerce Completo**: Sistema de vitrine, carrinho, checkout e confirmação de pedidos
- **Painel Administrativo**: Gestão completa de pedidos com autenticação
- **Design Premium**: Interface elegante com paleta de cores cereja, branco e dourado
- **Responsivo**: Otimizado para desktop, tablet e mobile
- **Acessibilidade**: Implementação completa de boas práticas de acessibilidade
- **TypeScript**: Tipagem forte para maior confiabilidade do código

## 🎨 Design System

### Paleta de Cores
- **Cereja**: `#C21807` - Cor principal da marca
- **Dourado**: `#D4AF37` - Cor secundária para destaques
- **Branco**: `#FFFFFF` - Cor de fundo e contraste
- **Gradientes**: Tons suaves para backgrounds e transições

### Tipografia
- **Fonte Principal**: Montserrat (Google Fonts)
- **Pesos**: 300, 400, 500, 600, 700, 800, 900
- **Hierarquia**: Sistema consistente de tamanhos e espaçamentos

## 🛠️ Tecnologias Utilizadas

### Frontend
- **React 18.3.1**: Biblioteca principal para interface
- **TypeScript 5.5.3**: Tipagem estática para JavaScript
- **Tailwind CSS 3.4.1**: Framework CSS utilitário
- **Lucide React**: Biblioteca de ícones moderna e consistente

### Build Tools
- **Vite 5.4.2**: Build tool rápido e moderno
- **PostCSS**: Processamento de CSS
- **Autoprefixer**: Prefixos CSS automáticos

### Database
- **Supabase**: Backend-as-a-Service com PostgreSQL
- **Row Level Security (RLS)**: Segurança de dados implementada
- **Real-time**: Atualizações em tempo real (preparado para uso futuro)

### Desenvolvimento
- **ESLint**: Linting de código JavaScript/TypeScript
- **TypeScript ESLint**: Regras específicas para TypeScript
- **React Hooks ESLint**: Regras para hooks do React

## 📁 Estrutura do Projeto

```
src/
├── components/          # Componentes reutilizáveis
│   ├── Admin/          # Componentes específicos do admin
│   ├── Cart/           # Componentes do carrinho
│   ├── Layout/         # Header, Footer e layout
│   ├── Product/        # Componentes de produto
│   └── UI/             # Componentes base (Button, Input, Card)
├── context/            # Contextos React (Cart, Order, Auth)
├── data/               # Configurações e dados estáticos
├── hooks/              # Custom hooks para API calls
├── lib/                # Configurações de bibliotecas (Supabase)
├── pages/              # Páginas principais da aplicação
├── types/              # Definições de tipos TypeScript
├── App.tsx             # Componente principal
├── main.tsx            # Ponto de entrada da aplicação
├── index.css           # Estilos globais e Tailwind
└── supabase/           # Migrações e configurações do banco
    └── migrations/     # Scripts SQL para criação das tabelas
```

## 🚀 Como Executar

### Pré-requisitos
- Node.js 18+ 
- npm ou yarn
- Conta no Supabase (para banco de dados)

### Instalação
```bash
# Clone o repositório
git clone https://github.com/seu-usuario/cherry-cupcake-store.git

# Entre no diretório
cd cherry-cupcake-store

# Instale as dependências
npm install

# Execute em modo de desenvolvimento
npm run dev
```

### Configuração do Banco de Dados
1. Crie um projeto no [Supabase](https://supabase.com)
2. Clique no botão "Supabase" no canto superior direito da aplicação
3. Configure as variáveis de ambiente automaticamente
4. As migrações serão executadas automaticamente

### Scripts Disponíveis
```bash
npm run dev        # Servidor de desenvolvimento
npm run build      # Build para produção
npm run preview    # Preview do build de produção
npm run lint       # Verificação de código
npm run typecheck  # Verificação de tipos TypeScript
```

## 📱 Funcionalidades

### Para Clientes
- **Vitrine de Produtos**: Grid responsivo com cards elegantes
- **Busca e Filtros**: Busca por nome e filtro por categoria
- **Detalhes do Produto**: Página dedicada com informações completas
- **Carrinho de Compras**: Drawer lateral com gestão de quantidade
- **Checkout**: Formulário completo com validação
- **Confirmação**: Página de sucesso com detalhes do pedido

### Para Administradores
- **Login Seguro**: Autenticação com credenciais admin:admin
- **Gestão de Pedidos**: Lista completa com filtros e busca
- **Atualização de Status**: Controle do fluxo de pedidos
- **Detalhes Completos**: Visualização detalhada de cada pedido

## 🎯 Componentes Principais

### UI Components
- **Button**: Botão com variantes (primary, secondary, outline, danger)
- **Input**: Campo de entrada com label e validação
- **Card**: Container com hover effects e sombras

### Layout Components
- **Header**: Navegação principal com carrinho
- **Footer**: Informações da empresa e links
- **CartDrawer**: Carrinho lateral deslizante

### Product Components
- **ProductCard**: Card de produto com imagem e ações
- **ProductGrid**: Grid responsivo de produtos

## 🔐 Autenticação Admin

O sistema possui autenticação simples para demonstração:
- **Usuário**: `admin`
- **Senha**: `admin`

## 📊 Dados de Exemplo

O sistema inclui:
- **6 Produtos**: Cupcakes variados armazenados no banco
- **8 Pedidos**: Pedidos de exemplo com diferentes status
- **Clientes**: Dados fictícios para demonstração
- **Banco de Dados**: PostgreSQL via Supabase com RLS habilitado

## 🎨 Customização

### Cores
As cores podem ser customizadas no arquivo `tailwind.config.js`:
```javascript
colors: {
  cherry: {
    // Tons de cereja
  },
  gold: {
    // Tons de dourado
  }
}
```

### Componentes
Todos os componentes são modulares e podem ser facilmente customizados ou estendidos.

### Banco de Dados
As tabelas podem ser modificadas através de novas migrações SQL na pasta `supabase/migrations/`.

## 📱 Responsividade

O design é totalmente responsivo com breakpoints:
- **Mobile**: < 768px
- **Tablet**: 768px - 1024px
- **Desktop**: > 1024px

## ♿ Acessibilidade

- **Alt texts** em todas as imagens
- **Labels** em todos os inputs
- **Contraste** adequado em todos os elementos
- **Navegação por teclado** funcional
- **ARIA labels** onde necessário

## 🚀 Deploy

A aplicação está configurada para deploy automático e pode ser facilmente hospedada em:
- Vercel
- Netlify
- GitHub Pages
- Qualquer servidor estático

### Build para Produção
```bash
npm run build
```

Os arquivos otimizados serão gerados na pasta `dist/`.

## 🤝 Contribuição

1. Fork o projeto
2. Crie uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

## 📞 Contato

Cherry Cupcake Store - contato@cherrycupcake.com

Link do Projeto: [https://github.com/seu-usuario/cherry-cupcake-store](https://github.com/seu-usuario/cherry-cupcake-store)

---

Desenvolvido com ❤️ para a Cherry Cupcake Store