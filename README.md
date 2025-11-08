ShoppeCenter – Sistema Interno de Gerenciamento de Tarefas  
Desenvolvido por TechFlow Solutions

Contexto do Projeto

A ShoppeCenter é uma empresa fictícia do setor de varejo online, especializada em vender produtos de múltiplas marcas por meio de sua plataforma digital.  
Com o crescimento das operações, a empresa enfrentava dificuldades na comunicação entre setores e na organização das atividades internas.

Para resolver esses desafios, a ShoppeCenter contratou a TechFlow Solutions para desenvolver um sistema interno de gerenciamento de tarefas, com foco em otimizar fluxos de trabalho e melhorar o acompanhamento de equipes.


Objetivo do Sistema

O sistema tem como principal objetivo organizar e monitorar o andamento das tarefas internas dos seguintes setores:

- Marketing – Campanhas, promoções e conteúdo digital  
- Logística – Envio, reposição e controle de estoque  
- Atendimento – Suporte ao cliente e acompanhamento de solicitações  
- TI– Manutenção do site e infraestrutura tecnológica  

Gestores podem acompanhar o status das atividades em tempo real, priorizar tarefas críticas e avaliar o desempenho da equipe de forma prática e centralizada.

Funcionalidades Principais

1. Gerenciamento de Tarefas  
- Criar, editar e excluir tarefas  
- Categorizar tarefas por setor (Marketing, Logística, Atendimento, TI)  
- Definir prioridade (Alta, Média, Baixa)  
- Controlar o status (A Fazer → Em Progresso → Concluído)  
- Atribuir responsáveis por tarefa  

Visualização Intuitiva  
- Interface simples, responsiva e organizada  
- Exibição de tarefas em formato de lista dinâmica
- Atualização em tempo real via Fetch API

3. Controle de Desempenho  
- Visualização geral das tarefas por status  
- Possibilidade de identificar gargalos e otimizar prazos  

Tecnologias Utilizadas

Backend
- Python 3.11  
- Flask (microframework web)  
- SQLite3 (banco de dados leve e embutido)  
- Flask-Restful (estrutura de rotas REST)  

Frontend
- HTML5, CSS3 e JavaScript  
- Fetch API para integração com o backend  

Ferramentas e Gestão
- Git / GitHub (versionamento e CI/CD)  
- GitHub Projects (gestão de tarefas no modelo Kanban)  
- GitHub Actions (pipeline de testes automatizados)  

Estrutura do Projeto

techflow_ShoppeCenter/
├── backend/
│ ├── app.py # Aplicação principal Flask
│ ├── models/
│ │ └── tarefa.py # Modelo da entidade Tarefa
│ ├── routes/
│ │ └── tarefa_routes.py # Rotas CRUD
│ └── database.py # Configuração do banco de dados
│
├── frontend/
│ ├── index.html # Interface principal do sistema
│ ├── css/
│ │ └── style.css # Estilos visuais e responsividade
│ └── js/
│ └── script.js # Lógica e integração com API
│
├── docs/
│ ├── requisitos.md # Requisitos funcionais e não funcionais
│ └── casos_de_uso.md # Descrição dos casos de uso
│
├── .github/
│ └── workflows/
│ └── tests.yml # Pipeline de testes automatizados
│
├── README.md # Documentação principal
└── requirements.txt # Lista de dependências do Python


Como Executar o Projeto

-Clonar o repositório
git clone https://github.com/Trixbeadev/TechFlow-Solutions---Sistema-de-Gerenciamento-de-Tarefas.git
cd TechFlow-Solutions---Sistema-de-Gerenciamento-de-Tarefas

- Criar e ativar o ambiente virtual
python -m venv venv
source venv/Scripts/activate  # (Windows)

- Instalar dependências
pip install -r requirements.txt

- Executar o servidor Flask
python backend/app.py

- Acessar no navegador
http://127.0.0.1:5000



Metodologia de Desenvolvimento

O projeto foi conduzido com base em metodologias ágeis, aplicando elementos do Kanban:

Etapa	Descrição
- Planejamento	Criação das histórias de usuário e priorização das tarefas
- Desenvolvimento	Implementação incremental de cada módulo (frontend e backend)
- Testes	Execução automatizada com GitHub Actions
- Entrega Contínua	Deploy interno e controle de versões
- Gestão de Mudanças	Adaptação de requisitos conforme novas demandas do cliente

* Durante o desenvolvimento, a ShopEase solicitou uma alteração de requisito:

Adicionar o campo prazo de entrega às tarefas, permitindo melhor controle de deadlines e priorização de atividades.

A equipe da TechFlow Solutions atualizou:
- O modelo de dados (tarefa.py)
- O formulário do frontend (index.html)
- A documentação técnica (requisitos.md)

Desenvolvimento

Beatriz França (@Trixbeadev)
Desenvolvedora responsável – TechFlow Solutions

Projeto desenvolvido para fins acadêmicos, aplicando princípios de Engenharia de Software, metodologias ágeis e boas práticas de versionamento.
