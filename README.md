# SistemaGestaoHospitalar_Backend
💻 Sistema de Gestão Hospitalar e de Serviços de Saúde (SGHSS) desenvolvido em Python + Flask. Projeto acadêmico que implementa rotas REST para gerenciamento de pacientes, profissionais, consultas, e administração hospitalar.

Este projeto faz parte do Trabalho Multidisciplinar do curso de Análise e Desenvolvimento de Sistemas.
O objetivo é desenvolver um sistema backend em Python (Flask) para auxiliar na gestão hospitalar e de serviços de saúde, incluindo pacientes, profissionais, consultas, e administração hospitalar.

🚀 Funcionalidades principais:
• Cadastro e autenticação de usuários (JWT + criptografia de dados).
• Gerenciamento de pacientes, profissionais e administradores.
• Agendamento, cancelamento e histórico de consultas.
• Controle de internações, leitos, suprimentos e relatórios financeiros.
• Banco de dados SQLite integrado ao Flask.
• Rotas REST API documentadas para testes no Postman.

🛠️ Tecnologias utilizadas:
• [Python 3](https://www.python.org/)
• [Flask (framework web)](https://flask.palletsprojects.com/)
• [Flask-JWT-Extended](https://flask-jwt-extended.readthedocs.io/)
• [SQLite (banco de dados leve)](https://www.sqlite.org/index.html)
• [SQLAlchemy (ORM para manipulação de dados)](https://www.sqlalchemy.org/)
• [Postman](https://www.postman.com/) (para testes de API)
• JWT (JSON Web Token) para autenticação
• Passlib para criptografia de senhas

---

▶️ Como rodar o sistema (passo a passo):

0) Pré-requisitos
- Python 3.10+ instalado  
- Git (opcional, apenas se for clonar o repositório)  
- Postman ( para testar as rotas)

---

1) Obter o código
Clonar com Git
```bash
# Clonar o repositório
git clone https://github.com/sabrinads23/TrabalhoFinal_SGHSS_Backend.git
# Entrar na pasta
cd TrabalhoFinal_SGHSS_Backend
```
Ou baixar como ZIP
```bash
Em Code o arquivo SGHSS_4493981.zip → Download ZIP no GitHub.
Extraia o ZIP.
```
2) Abra o terminal CMD e entre na pasta onde o arquivo foi extraido.
```bash
Exemplo:
cd C:\Users\Usuario\Desktop\SGHSS_4493981
```
3) Criar ambiente virtual (venv)
```bash
Windows (PowerShell)
python -m venv venv
.\venv\Scripts\activate

Windows (CMD)
python -m venv venv
venv\Scripts\activate

macOS / Linux
python3 -m venv venv
source venv/bin/activate
```
Você saberá que o venv está ativo quando aparecer (venv) no início da linha do terminal.

4) Instalar dependências
```bash
pip install -r requirements.txt
```

5) Rodar a aplicação
```bash
python app.py
```
Se tudo der certo, aparecerá:
```bash
* Running on http://127.0.0.1:5000
```
6) Acessar e testar
No Postman:
```bash
Configure a URL base como http://127.0.0.1:5000
Configure os demais itens conforme a documentação anexada "Endpoints_SGHSS"
• Método HTTP (GET, POST, PUT, DELETE) 
• URL da rota 
• Parâmetros e estruturas JSON 
Comece com Registrar Administrador e depois faça login como o administrador criado para pegar o token JWT
Envie esse token como Bearer Token nas demais requisições
Dica: desative o proxy sistem em settings do Postman caso apresente algum problema ao testar a api
```
7) Parar o servidor
```bash
Ctrl + C
```
8) Rodar novamente no futuro
```bash
- Sempre que abrir o projeto em outro dia:
- Ative o venv (passo 2)
- Rode novamente:
- python app.py
```
🔧 Problemas comuns

'pip' não é reconhecido
```bash
Use python -m pip install -r requirements.txt
```
Erro ao ativar venv no PowerShell
```bash
Rode: Set-ExecutionPolicy -Scope CurrentUser RemoteSigned
```
ModuleNotFoundError: No module named 'flask'
```bash
Ative o venv antes de instalar as dependências.
```
Porta 5000 ocupada
```bash
Feche outros servidores ou rode em outra porta:
- python app.py --port=5001
```
A API rodará em:
```bash
👉 http://127.0.0.1:5000/
```
📌 Observações:
O projeto é apenas para fins acadêmicos.


👩‍💻 Autora
Sabrina Dekkers
RU: 4493981
Curso: Análise e Desenvolvimento de Sistemas - Uninter

