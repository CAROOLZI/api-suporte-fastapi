🎫 API de Gerenciamento de Chamados de Suporte Técnico (FastAPI)

API RESTful desenvolvida em Python com o framework moderno FastAPI, projetada para simular o ciclo de vida completo de abertura, triagem, atendimento e encerramento de chamados (tickets) de Suporte Técnico de TI (N1 e N2).

💡 Contexto do Projeto: Unindo minha vivência prática de 8 meses em Suporte Técnico com desenvolvimento Backend, criei esta API para automatizar processos comuns de atendimento, controle de SLA e rastreamento de incidentes.

🚀 Funcionalidades
📌 Abertura de Chamados: Registro de tickets com título, descrição, categoria (Hardware, Software, Redes, Acessos) e nível de prioridade (Baixa, Média, Alta, Crítica).
🔍 Consulta e Filtros: Listagem geral de chamados e filtros por status (Aberto, Em Andamento, Resolvido, Cancelado).
🔄 Atualização de Status: Roteamento de chamados entre níveis de suporte (N1 -> N2) e atualização de notas técnicas.
❌ Encerramento de Tickets: Finalização do chamado com registro da solução aplicada.
📖 Documentação Interativa Automática: Interface Swagger UI integrada para testes de endpoints em tempo real.
🛠️ Tecnologias Utilizadas
Linguagem: Python 3.10+
Framework: FastAPI
Validação de Dados: Pydantic (garantia de integridade e tipos dos dados)
Servidor ASGI: Uvicorn
Documentação: Swagger UI & ReDoc (nativos do FastAPI)
🛣️ Rotas da API (Endpoints Principais)
Método	Rota	Descrição
POST	/chamados/	Cria um novo chamado de suporte
GET	/chamados/	Lista todos os chamados cadastrados
GET	/chamados/{id}	Retorna os detalhes de um chamado específico
PUT	/chamados/{id}	Atualiza status, prioridade ou informações do chamado
DELETE	/chamados/{id}	Remove um chamado da base
📦 Como Executar o Projeto Localmente
Pré-requisitos
Python instalado (versão 3.10 ou superior)
Git instalado
Passo a Passo

Clone o repositório:

bash
git clone https://github.com/CAROOLZI/api-suporte-fastapi.git
cd api-suporte-fastapi

Crie e ative um ambiente virtual (recomendado):

bash
# Windows
python -m venv venv
.\venv\Scripts\activate

Instale as dependências:

bash
pip install -r requirements.txt
# Ou diretamente:
pip install fastapi uvicorn

Inicie o servidor local:

bash
uvicorn main:app --reload

Acesse a documentação interativa: Abra o seu navegador e acerte: 👉 http://127.0.0.1:8000/docs (Swagger interativo)

👩‍💻 Autora

Desenvolvido por Carolina Fernanda

Conecte-se comigo no LinkedIn
Conheça outros projetos no meu GitHub
