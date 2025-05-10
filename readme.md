🏋️ Monitoramento de Treinos com Google Sheets
Este projeto realiza o monitoramento de exercícios físicos utilizando a API do Nutritionix para interpretar os treinos e registra os dados automaticamente em uma planilha online via Google Sheets (ou Sheety API).

🔧 Funcionalidades
Entrada de texto com os exercícios realizados.

Utilização da API da Nutritionix para identificar tipo de exercício, duração e calorias gastas.

Registro automático dos dados em uma planilha via API.

Armazenamento seguro das credenciais via variáveis de ambiente.

🧰 Tecnologias Utilizadas
Python

API Nutritionix (https://www.nutritionix.com/)

Sheety API ou Google Sheets como endpoint

Bibliotecas: requests, datetime, os

🚀 Como Usar
Clone o repositório:

bash
Copiar
Editar
git clone https://github.com/seu-usuario/seu-repo.git
cd seu-repo
Configure as variáveis de ambiente:
Você pode usar um arquivo .env ou definir diretamente no terminal:

bash
Copiar
Editar
export ENV_API_KEY="sua_api_key"
export ENV_APP_ID="seu_app_id"
export ENV_SHEET_ENDPOINT="sua_url_da_planilha"
export ENV_PASSWORD="sua_senha"
Execute o script:

bash
Copiar
Editar
python treino_monitoramento.py
Informe os exercícios realizados:
Quando solicitado, digite os exercícios. Exemplo:

bash
Copiar
Editar
Tell me which exercises you did: I ran for 30 minutes and did 20 minutes of yoga.
Os dados serão enviados automaticamente para sua planilha online.

📋 Exemplo de Dados Enviados à Planilha
Data	Hora	Exercício	Duração (min)	Calorias
10/05/2025	18:23:01	Running	30	240

🔒 Segurança
As credenciais da API e da planilha são acessadas via variáveis de ambiente, garantindo que dados sensíveis não sejam expostos no código-fonte.