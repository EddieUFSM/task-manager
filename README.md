# Task Manager
<img src="https://img.shields.io/static/v1?label=Task%20Manager&message=Project&color=4CAF50&style=plastic"/><img src="https://img.shields.io/static/v1?label=Kanban&message=Methodology&color=0074E8&style=plastic"/><img src="https://img.shields.io/static/v1?label=Docker&message=Containerization&color=2496ED&style=plastic&logo=docker"/><img src="https://img.shields.io/static/v1?label=Python&message=Programming%20Language&color=3776AB&style=plastic&logo=python"/><img src="https://img.shields.io/static/v1?label=PostgreSQL&message=Database&color=336791&style=plastic&logo=postgresql"/><img src="https://img.shields.io/static/v1?label=Django&message=Framework&color=092E20&style=plastic&logo=django"/><img src="https://img.shields.io/static/v1?label=Status&message=Em%20Desenvolvimento&color=yellow&style=plastic"/>

## Descrição
Gerenciador de tarefas estilo Kanban, desenvolvido em Django.

## Tecnologias Utilizadas
- Django
- PostgreSQL
- Docker (opcional, para facilitar o ambiente de desenvolvimento)

## Iniciando o Projeto

### Pré-requisitos
- Python 3.x
- PostgreSQL (ou Docker, se preferir usar containers)

### Instalação
1. Clone o repositório:

```bash
git clone https://github.com/seu-usuario/task-manager.git
cd task-manager
```

2. Instale as dependências:

```sh
pip install -r requirements.txt
```
3. Configure as variáveis de ambiente (opcional):
Crie um arquivo .env na raiz do projeto e configure as variáveis de ambiente.
4. Execute as migrações do banco de dados:
```sh
python manage.py migrate
```
5. inicie o servidor de desenvolvimento:
```sh
python manage.py runserver
```
6. Acesse a aplicação em http://localhost:8000/

### Endpoints

#### Criar uma nova tarefa
URL: /api/tasks/
Método: POST
Body:
```json
{
  "title": "Nova Tarefa",
  "description": "Descrição da nova tarefa",
  "status": "TODO"
}
```

#### Atualizar uma tarefa existente
URL: /api/tasks/<id>/
Método: PUT
Body:
```json
{
  "title": "Tarefa Atualizada",
  "description": "Descrição atualizada da tarefa",
  "status": "IN_PROGRESS"
}
```

####  Obter todas as tarefas
URL: /api/tasks/
Método: GET

#### Obter uma tarefa específica
URL: /api/tasks/<id>/
Método: GET

### Instalação
1. Clone o repositório:
```bash
git clone https://github.com/seu-usuario/task-manager.git
cd task-manager
```
