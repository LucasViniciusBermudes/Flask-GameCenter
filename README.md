# 🎮 Flask GameCenter

Aplicação web desenvolvida com **Flask** para gerenciamento de jogos e usuários, incluindo autenticação, upload de arquivos e persistência em banco de dados.

Projeto desenvolvido para fins de **estudo e prática**, aplicando boas práticas de Git, organização de projeto Flask e ambiente virtual Python.

---

## 📋 Funcionalidades

- Cadastro e listagem de jogos
- Autenticação de usuários
- Upload de arquivos
- Persistência de dados em banco local
- Interface com templates HTML
- Organização MVC simplificada

---

## 🛠️ Tecnologias utilizadas

- **Python 3**
- **Flask**
- **HTML / CSS**
- **SQLite**
- **Git & GitHub**

---

## 📁 Estrutura do projeto

```
Flask-GameCenter/
├── static/             # Arquivos estáticos (CSS, etc.)
├── templates/          # Templates HTML
├── uploads/            # Uploads de arquivos (mantida com .gitkeep)
├── __pycache__/        # Cache Python (ignorado)
├── .gitignore
├── README.md
├── requirements.txt
├── config.py
├── helpers.py
├── jogoteca.py         # Arquivo principal da aplicação
├── models.py
├── prepara_banco.py    # Script de criação do banco
├── views_game.py
└── views_user.py
```
## ⚙️ Pré-requisitos
Antes de começar, você precisa ter instalado:
```
-Python 3.10 ou superior
-Git
-(Opcional) VS Code ou outro editor de código
```
Verifique a versão do Python:
```
python --version
```
---

## 🚀 Instalação e execução
1️⃣ Clonar o repositório
```
git clone https://github.com/LucasViniciusBermudes/Flask-GameCenter.git
cd Flask-GameCenter
```
---

2️⃣ Criar e ativar o ambiente virtual
▶ Windows (PowerShell)
```
python -m venv .venv
.venv\Scripts\Activate.ps1
```
Se ocorrer erro de política de execução:
```
Set-ExecutionPolicy -Scope CurrentUser RemoteSigned
```
▶ macOS / Linux
```
python3 -m venv .venv
source .venv/bin/activate
```
---

3️⃣ Instalar as dependências

Com o ambiente virtual ativo:
```
pip install -r requirements.txt
```
Caso o arquivo ainda não exista:
```
pip freeze > requirements.txt
```
4️⃣ Pasta de uploads

A aplicação utiliza a pasta uploads/ para armazenar arquivos enviados.

Essa pasta é mantida no repositório através do arquivo .gitkeep.
Caso não exista por algum motivo:
```
mkdir uploads
```
---
5️⃣ Preparar o banco de dados

Execute o script de criação do banco:
```
python prepara_banco.py
```
---

6️⃣ Executar a aplicação
▶ Opção A — Execução direta
```
python jogoteca.py
```
▶ Opção B — Flask CLI
Windows (PowerShell):
```
$env:FLASK_APP="jogoteca.py"
$env:FLASK_ENV="development"
flask run
```

macOS / Linux:
```
export FLASK_APP=jogoteca.py
export FLASK_ENV=development
flask run
```
---

7️⃣ Acessar no navegador

Abra o navegador e acesse:
```
http://127.0.0.1:5000
```
---

## 🧹 Boas práticas adotadas

❌ Ambiente virtual (.venv/) não é versionado

❌ Cache Python (__pycache__/) ignorado

✅ Dependências versionadas via requirements.txt

✅ Pasta uploads/ mantida com .gitkeep

❌ Arquivos sensíveis (.env) não versionados

✅ Commits semânticos

---

## 📌 Observações

Este projeto utiliza SQLite para desenvolvimento local

Ideal para fins educacionais e estudo de Flask

Em produção, uploads e banco devem ser adaptados para serviços externos
