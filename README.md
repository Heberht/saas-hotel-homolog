# saas-hotel-homolog
🏨 SaaS Pousadas MVP
Uma plataforma SaaS white label completa para gestão de pousadas, desenvolvida com foco em automatização operacional e potencialização de vendas diretas.

🚀 Tecnologias
Backend
Node.js - Runtime JavaScript
Express.js - Framework web
PostgreSQL - Banco de dados
Sequelize - ORM
JWT - Autenticação
bcryptjs - Criptografia
Frontend
React 18 - Biblioteca JavaScript
Vite - Build tool
Tailwind CSS - Framework CSS
Zustand - Gerenciamento de estado
React Router - Roteamento
React Hook Form - Formulários
Lucide React - Ícones
Recharts - Gráficos
📋 Funcionalidades
✅ Dashboard
KPIs visuais em tempo real
Total de acomodações e hóspedes
Reservas da semana e check-ins do dia
Receita estimada dos últimos 30 dias
Próximos check-ins
Ações rápidas
Sugestões de IA
✅ Gestão de Acomodações
CRUD completo de quartos/acessos
Definição de tarifas por tipo e período
Status de ocupação em tempo real
Filtros e busca avançada
✅ Gestão de Hóspedes
Cadastro completo com histórico
Preferências e comportamento de compra
Registro automático de interações
Visualização 360º do hóspede
Sistema de tags e segmentação
✅ Gestão de Reservas
Calendário visual com ocupação
Criação, edição e cancelamento
Check-in/check-out automatizado
Sincronização com Booking/Airbnb (mock)
✅ CRM e Pipeline
Captura de leads via formulário
Pipeline de vendas configurável
Aplicação de tags e segmentações
Conversão de leads em hóspedes
✅ Marketing e Campanhas
CRUD de campanhas
Disparo de campanhas (mock funcional)
Segmentações com filtros básicos
Estatísticas de performance
✅ Automação com IA
Sugestões automatizadas baseadas em dados
Recomendações de campanhas
Alertas de ocupação baixa
Identificação de hóspedes inativos
🛠️ Instalação
Pré-requisitos
Node.js (versão 16 ou superior)
PostgreSQL (versão 12 ou superior)
npm ou yarn
1. Clone o repositório
git clone <url-do-repositorio>
cd saas-mvp
2. Instale as dependências
npm run install-all
3. Configure o banco de dados
# Crie um banco PostgreSQL chamado 'saas_pousadas'
createdb saas_pousadas
4. Configure as variáveis de ambiente
# Backend
cd backend
cp env.example .env
# Edite o arquivo .env com suas configurações
5. Execute o projeto
# Desenvolvimento (backend + frontend)
npm run dev

# Ou execute separadamente:
npm run server  # Backend na porta 5000
npm run client  # Frontend na porta 3000
📁 Estrutura do Projeto
saas-mvp/
├── backend/                 # API Node.js/Express
│   ├── models/             # Modelos Sequelize
│   ├── routes/             # Rotas da API
│   ├── middleware/         # Middlewares
│   └── server.js           # Servidor principal
├── frontend/               # Aplicação React
│   ├── src/
│   │   ├── components/     # Componentes React
│   │   ├── pages/          # Páginas da aplicação
│   │   ├── store/          # Zustand stores
│   │   └── services/       # Serviços de API
│   └── package.json
└── package.json            # Scripts principais
🔐 Autenticação
O sistema usa JWT para autenticação. Para acessar endpoints protegidos, inclua o header:

Authorization: Bearer <seu_token_jwt>
📊 Banco de Dados
Principais Tabelas:
users - Usuários do sistema
inns - Pousadas (multi-tenant)
accommodations - Acomodações/quartos
guests - Hóspedes
reservations - Reservas
campaigns - Campanhas de marketing
leads - Leads do CRM
interactions - Interações com hóspedes
🚀 Deploy
Variáveis de Ambiente para Produção:
NODE_ENV=production
DB_HOST=seu_host_producao
DB_PORT=5432
DB_NAME=saas_pousadas_prod
DB_USER=usuario_producao
DB_PASSWORD=senha_forte_producao
JWT_SECRET=chave_super_secreta_producao
Comandos de Deploy:
# Build do frontend
cd frontend
npm run build

# Start do backend
cd backend
npm start
📱 Funcionalidades Demonstráveis
Dashboard
✅ KPIs em tempo real
✅ Ações rápidas
✅ Check-ins do dia
✅ Sugestões de IA
Gestão Operacional
✅ CRUD de acomodações
✅ CRUD de hóspedes
✅ CRUD de reservas
✅ Calendário de ocupação
CRM e Marketing
✅ Pipeline de leads
✅ Campanhas de marketing
✅ Segmentação de hóspedes
✅ Conversão de leads
Automação
✅ Sugestões baseadas em dados
✅ Alertas de ocupação
✅ Identificação de padrões
🎯 Próximos Passos
 Integração com Stripe para pagamentos
 Integração real com Booking/Airbnb
 Sistema de notificações push
 Relatórios avançados
 App mobile
 Integração com WhatsApp Business API
📝 Licença
Este projeto faz parte do MVP SaaS Pousadas.

🤝 Contribuição
Fork o projeto
Crie uma branch para sua feature (git checkout -b feature/AmazingFeature)
Commit suas mudanças (git commit -m 'Add some AmazingFeature')
Push para a branch (git push origin feature/AmazingFeature)
Abra um Pull Request
📞 Suporte
Para dúvidas ou suporte, entre em contato através dos canais disponíveis.
